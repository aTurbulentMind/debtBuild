<body>
    
    <h1>Contact page</h1>

    <div class="call">
        <h2>Give us a call at:</h2>
        <p>Toll free: <a href="tel: +8005528397/">+1(800)552-8397</a> <br>
        Fax: <a href="+2532042349/">1-253-204-2349</a> </p>
</div>


<h2>We have a support plan set up to know we will be here when you need it.</h2>
        <p  id="bottom20" >
            Debt$Net® technical support plans suit different purposes. Initial Purchase Support provides 90 days of technical phone support and comes as part of the purchase price of Debt$Net®. Other support plans, such as Hour Based Plans and the Unlimited Support plan provide technical support services for agencies after the Initial Purchase Support time expires. The paragraphs below explain each support plan.
<br><br><br><br>
<span> Initial Purchase Support:</span> The initial purchase of Debt$Net® includes telephone technical support. It provides five hours of time for the multi-user version, and three hours for the single-user version. This 90 day phase of technical support provides assistance to new customers for the installation and configuration of Debt$Net® software. Technicians log all time spent on the telephone with the Technical Support Department against the initial support hours, regardless of the nature of the problem. When 90 days has elapsed, or when the support time has been consumed, TCM offers continued support through one of the Debt$Net® support plans described below.
<br><br><br><br>
<span> Hour Based Plans: </span>The Hour Based Plans provide agencies with hour blocks of telephone technical support per quarter. The hour based blocks are available at a 2 hour level, 4 hour level and 8 hour level. This plan type benefits experienced agencies with consistent support requirements. The Technical Support Department tracks support time and deducts it from the agency's quarterly time allocation. Technicians provide support during normal TCM business hours. Time deducts from the quarterly allocation regardless of the nature of the problem. When needed, agencies purchase additional support time at the published hourly rate for their level. Agencies must pay for additional time in advance and all time expires at the end of the quarter.
<br><br><br><br>
<span>Unlimited Support Plan:</span>  The Unlimited Support Plan provides "as required" technical support during normal business hours. Technicians do not track support time and time allocations do not apply. The Technical Support Department provides services directly covered by the support plan without requiring additional time purchases. Under this plan, the agency pays a flat fee once per quarter. The plan covers only assistance with Debt$Net®. This plan benefits large agencies or agencies with high support requirements that do not want to face unplanned additional support expenses.
        </p>
    
    

    <div class="mail">
        <h2>Our postal address is:</h2>
        <p>The Computer Manager, Inc. <br>
            4110 Kitsap Way Suite 101 <br>
            Bremerton, WA 98312 <br>
            PO Box 4091</p>
    </div>

    <div class="social">
        <h2>Social media:</h2> 
        
        <p><a href="https://www.linkedin.com/company/debt-net/">  Follow us on Linkedin.</a> </p>

        <p><a href="https://www.linkedin.com/company/debt-net/">  Follow us on Facebook.</a> </p>
    </div>

   
    <container>
        
        <form action="https://formsubmit.co/joel@debtnet5.com" method="POST">
            <h2 class="double">Contact:</h2>
            
            <wrapper>
                <box>
                    
                    <label for="fname"></label>
                </box>
            </wrapper>
            
            <wrapper>
                <box>
                    <input type="text" name="fname" id="fname" required>
                    <label for="fname">First and Last Name</label>
                </box>
            </wrapper>

            <wrapper>
                <box>
                    <input type="text" name="email" id="email" required>
                    <input type="hidden" name="_next" value="https://debtnet5build.netlify.app/">
                    <label for="email">Email</label>

                </box>
            </wrapper>

           

            <wrapper>
                <box>
                    <input type="text" name="tel" id="tel" required>
                    <label for="tel">Telephone</label>
                </box>
            </wrapper>

            <wrapper>
                <box>
                    <input type="text" name="comp" id="comp" required>
                    <label for="comp">Company Name</label>
                </box>
            </wrapper>

            <wrapper>
                <box>
                    <input type="text" name="sta" id="sta" required>
                    <label for="tel">State</label>
                </box>
            </wrapper>

            
            <!--
            <div class="section1">
            <wrapper>
                <box>
                    <div class="flex-row">
                    <input type="checkbox" name="check1" id="chk" required>
                    <label for="chk">option</label>
                    </div>
                </box>
                <box>
                    <div class="flex-row">
                    <input type="checkbox" name="check1" id="chk" required>
                    <label for="chk">option2</label>
                    </div>
                </box>
                <box>
                    <div class="flex-row">
                    <input type="checkbox" name="check1" id="chk" required>
                    <label for="chk">option3</label>
                    </div>
                </box>
                <box>
                    <div class="flex-row">
                    <input type="checkbox" name="check1" id="chk" required>
                    <label for="chk">option4</label>
                    </div>
                </box>
            </wrapper>
            </div>
        -->
            <wrapper>
                <box>
                    <textarea id="mes" required></textarea>
                    <label for="mes">Anything else?</label>
                </box>
            </wrapper>

          <!-- <input type="submit" name="" value="sedn">--> 
            <button type="submit">Submit</button>
        </form>
    </container>

</body>

<style lang="scss">
    @import 'styles/components';

    *{
        
        box-sizing: border-box;
    }

    .call{

        p{
            padding-left: 25%;
        }
    }

    .social {

        float: left;
        margin: 2%;

        h2{
            margin-bottom: 5%;
        }
        
        a{ 
            color: $backgroundMain;
            font-size: 1.75vw;
        }

        p{
            background: $extra;
            border-radius: 5px;
            width: fit-content;
            text-align: center;
            overflow-x: hidden;
            padding: 2%;
            box-shadow: 0 2px 20px 2px $extraExtra;
            cursor: pointer;
            

            &:hover{
                transform: scale(1.1);
                box-shadow: 0 3px 8px 3px $textMain;
                border: 1px solid $textMain;
            }
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

    .mail{
        background: $extra;
        color: $backgroundMain;

        h2{
            padding: 8%;
        }
        p{
            padding: 25%;
            margin: -30% 0 5% 0;
        }
    }

    //form
    container{
        
        

    h2{
        color: $backgroundMain;
        font-size: 3vw;
        text-align: center;
        grid-column: 1 ;
    }

    form{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(275px, 1fr));
        background: $extra;
        width: 65%;
        margin:8%;
        padding: 4%;
        border-radius:4px;
        box-shadow: 0 2px 20px 2px $extraExtra;
    }
    
    wrapper{
        width: 100%;
        display: grid;
        grid-gap:30px;
        gap:30px;
    }

    box{
        width: 100%;
        position: relative;
        padding: 20px;
    }

    input,
    textarea{
        width: 100%;
        font-size: 2vw;
        background: transparent;
        border: none;
        outline: none;
        border-bottom: 1px solid $textMain;
        transition:0.3s linear;
    }

    input:focus,
    input:valid,
    textarea:focus,
    textarea:valid{
        padding: 10px;
        background: $backgroundSecond;
        margin: 10px;
        border-radius:4px;
    }

    label{
        position: absolute;
        top: 0;
        left: 0;
        color: $backgroundSecond;
        font-size: 2vw;
        font-weight: bold;
        padding: 20px;
        transition: 0.3s linear;
    }

    input:focus ~ label,
    input:valid ~ label,
    textarea:focus ~ label,
    textarea:valid ~ label{
        padding: 0;
    }

    .section1{
        input{
            accent-color: hotpink;
            block-size: 45px;
            inline-size:18px;
        }

        input:focus,
        input:valid,
        textarea:focus,
        textarea:valid{
        padding: 0.5px;
        margin: 0.5px;
    }
    }

    .flex-row{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;

        label {
            padding: 0 10px;
        }
    }
    }


    button{
    background: rgba(16, 15, 17, 0.616);
        outline: none;
        font-weight: 100;
        letter-spacing: 2px;
        border: 1px solid $extra;
        border-radius:4px;
        color: $backgroundMain;
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

        container{
            form{
                width: 85%;
            }
            label{
                font-size: 3vw;
                padding: 5px 10px;
            }
        }
            .social{
                float: none;
            }

            .socImg {
             width: 90%;
             height: 90%;
             margin: 10% 5%;
            }
    }

    	/*Extra Large screens */
      	@media only screen and (min-width: 1400px) {

            body{
            container{
                form{
                grid-template-columns: repeat(auto-fit, minmax(475px, 1fr));
                }

                label{
                font-size: 1.5vw;
                padding: 5px;
                }

                input, textarea{
                font-size: 1vw;
                }

                input:focus,
                input:valid,
                textarea:focus,
                textarea:valid{
                    margin: 4% 1%;   
                }
            }
      	}
    }
</style>