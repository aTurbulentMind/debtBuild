<body>

    <div class="entryImg">
		<img class="bigger" src="img/Ferry.jpg" alt="" />
  
        <div class="centered"> <h1>Contact Us</h1></div>
    </div>

    <div class="call">
        <h2>Give us a call at:</h2>
        <p>Toll free: <a href="tel: +8005528397">+1(800)552-8397</a> <br>
        Fax: <a href="+2532042349">1-253-204-2349</a> </p>
</div>
    
    

    <div class="mail">
        <h2>Our postal address is:</h2>
        <p>The Computer Manager, Inc. <br>
4110 Kitsap Way Suite 101 <br>
P.O. Box 4091 <br>
Bremerton, WA 98312</p>
    </div>

    <div class="social">
        <h2>We have an active LinkedIn account</h2>
        <a href="https://www.linkedin.com/company/debt-net/">  <img class="socImg" src="img/linked.png" alt=""></a> 
    </div>

    <div class="form">
   <h3>Our contact form is a great way to reach us:</h3>
    <form action="https://formsubmit.co/joelkrivers@yahoo.com" method="POST">
     <input type="hidden" name="_subject" value="Client submission">    
     
     <p>Your email:</p>
     <input type="email" name="email" placeholder="Email" required>
     <input type="hidden" name="_next" value="https://tender-benz-1741cd.netlify.app/">
     
     <p>Tell us about how we can help you:</p>
     <textarea name="t1" id="plan_for_art" cols="55" rows="8" required></textarea>
     <br>
     
     <button type="submit">Submit</button>
    </form>

    </div>

    <h2>We have a support plan set up to know we will be here the moment you need it.</h2>
        <p  id="bottom20" >
            Debt$Net® technical support plans suit different purposes. Initial Purchase Support provides 90 days of technical phone support and comes as part of the purchase price of Debt$Net®. Other support plans, such as Hour Based Plans and the Unlimited Support plan provide technical support services for agencies after the Initial Purchase Support time expires. The paragraphs below explain each support plan.
<br><br><br><br>
<span> Initial Purchase Support:</span> The initial purchase of Debt$Net® includes telephone technical support. It provides five hours of time for the multi-user version, and three hours for the single-user version. This 90 day phase of technical support provides assistance to new customers for the installation and configuration of Debt$Net® software. Technicians log all time spent on the telephone with the Technical Support Department against the initial support hours, regardless of the nature of the problem. When 90 days has elapsed, or when the support time has been consumed, TCM offers continued support through one of the Debt$Net® support plans described below.
<br><br><br><br>
<span> Hour Based Plans: </span>The Hour Based Plans provide agencies with hour blocks of telephone technical support per quarter. The hour based blocks are available at a 2 hour level, 4 hour level and 8 hour level. This plan type benefits experienced agencies with consistent support requirements. The Technical Support Department tracks support time and deducts it from the agency's quarterly time allocation. Technicians provide support during normal TCM business hours. Time deducts from the quarterly allocation regardless of the nature of the problem. When needed, agencies purchase additional support time at the published hourly rate for their level. Agencies must pay for additional time in advance and all time expires at the end of the quarter.
<br><br><br><br>
<span>Unlimited Support Plan:</span>  The Unlimited Support Plan provides "as required" technical support during normal business hours. Technicians do not track support time and time allocations do not apply. The Technical Support Department provides services directly covered by the support plan without requiring additional time purchases. Under this plan, the agency pays a flat fee once per quarter. The plan covers only assistance with Debt$Net®. This plan benefits large agencies or agencies with high support requirements that do not want to face unplanned additional support expenses.
        </p>
</body>

<style lang="scss">
    @import 'components';

    

    .call{

        p{
            padding-left: 25%;
        }
    }

    .socImg {
    width: 60%;
    height: 60%;
    margin: 0 18% 10% 18%;
    border: 1px solid $extra;
    border-radius: 8px;
    box-shadow: 0 3px 12px 3px $textMain;
 }

    span{
        font-weight: 600;
    }

    .mail{
        background: $extra;
        color: $backgroundMain;

        p{
            padding-left: 25%;
        }
    }

    .form {
      @include glassBack();
      margin: 0 13% 25% 13%;
      padding: 6%;
      contain: content;
      border-radius: 8px;

      h3, p {
          margin: 4% 0;
      }
   }

    button{
    background: rgba(16, 15, 17, 0.616);
        outline: none;
        font-weight: 100;
        letter-spacing: 2px;
        border: 1px solid $extra;
        color: $textMain;
        text-transform: uppercase;
        padding: 10px;
        margin:15% 0 10% 0;

        &:hover {
           transition: all 0.2s ease-in-out;
        background: $textMain;
        color: $backgroundMain;
        transform: scale(1.05);
        }
 }

    

  @media (max-width: 768px) {
      .form {
      @include glassBack();
      margin: 0 3%;
      padding: 6%;
      contain: content;
      border-radius: 8px;

      h3, p {
          margin: 4% 0;
      }
   }

   .socImg {
    width: 90%;
    height: 90%;
    margin: 10% 5%;
 }
  }

  

</style>