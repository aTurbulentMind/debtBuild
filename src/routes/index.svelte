<body>

	<div class="art-banner" id="art-banner">
    <div class="art-banner-bg"></div>
    <!-- <div class="banner-text">Debt$Net</div>-->
    <div class="badge">
    	<p><a href="https://www.linkedin.com/company/debt-net/"> LinkedIn</a></p>
    </div>

	<div class="form">
        
        <form action="https://formsubmit.co/joelkrivers@gmail.com" method="POST">
            <wrapper>
                <box>
                    <input type="text" name="email" id="email" placeholder="Ask a question" required>
                    <input type="hidden" name="_next" value="https://www.lanternlightdevelopment.com/contact">
                    
                </box>
            </wrapper>
            <br>
            <button type="submit">Contact</button>
        </form>
        
    </div>

    </div>

	<h1>Debt collection software by The Computer Manager, inc.</h1>

	<p>
		Debt$Net®, has provided collection agencies, law firms, debt buyers and in-house collection
		departments with one of the most comprehensive debt collection systems in the industry. Proven
		in the field, Debt$Net® collection software has satisfied the debt recovery requirements for
		over 1,000 companies specializing in Retail, Commercial, Medical, Receivables Management and
		Check Collections.
	</p>

	<div class="contBar">
		<h2>Contact Us</h2>
		<div class="mail">
        <h2>Our postal address is:</h2>
        <p>The Computer Manager, Inc. <br>
            4110 Kitsap Way Suite 101 <br>
            Bremerton, WA 98312 <br>
            P.O. Box 4091</p>
    	</div>
		<p>Whether a comment or question, we could love to hear from you.</p>
		<p><a sveltekit:prefetch href="/contact/">Here</a></p>
	</div>

	
	<img class="indi" src="img/PrestigeLogo.jpg" alt="the debt net power logo" />
	<p>
		Debt$Net® Prestige is the latest product by Debt$Net® Collection Software. This version of the
		award-winning collection agency software is SQL based using the powerful SQL Server by
		Microsoft. Developed with mid-sized to large agencies in mind, Debt$Net® Prestige offers the
		flexibility and business features requested by established agencies along with the security and
		stability required by high capacity business.
	</p>

	<img class="indi" src="img/PowerLogo.jpg" alt="the debt net prestige logo" />

	<p>
		Debt$Net® Power is the heritage product by Debt$Net® Collection Software. For over 20 years,
		Debt$Net® has provided collection agencies, law firms, debt buyers and in-house collection
		departments with one of the most comprehensive debt collections systems in the industry. Now
		with even more functionality, Debt$Net® Power offers all the features, flexibility and
		sophistication of mainframe packages at an affordable price.
	</p>

  <h2>Some Kind Words From Our Wonderful Patrons:</h2>
  
	<div>
		<h2>Capital Recovery Systems</h2>
		<h3 id="subSpace">
			"My agency has been using Debt$Net™ for 5 years and we have been very satisfied with both the
			product and the service."
		</h3>
		<p>
			I would like to pay my compliments to Debt$Net® and The Computer Manager for their very user
			friendly software. My agency has been using Debt$Net™ for 5 years and we have been very
			satisfied with both the product and the service. The product is easy to learn and has many
			useful tools for both collectors and administrators. Debt$Net® also has excellant customer
			service. We are on the East Coast, and although there is a time difference, they have tech
			support available for all times of the day. In summary, I would strongly recommend Debt$Net®
			for any Collection Agency trying to gain an edge in the industry.
			<br><br>
			<span> Joseph Tammaro</span>
		</p>
		
	</div>

<div class="testim">
		<h2>Remit Corporation</h2>
		<h3 id="subSpace">"I feel like we hit the jackpot when we found Debt$Net®."</h3>
		<p>
			I have been in the collection industry for 30 years, since the age of 12, when my family
			opened a collection system. I feel like we hit the jackpot when we found Debt$Net®. We have
			been Debt$Net® users since the start of our new operation, Remit Corporation, in June of 1992
			and have developed a very valuable relationship with this software firm. They have been
			instrumental in our growth and success and remain loyal partners in our company's progress. We
			have been highly involved in the continuing development and improvement of their system and
			have found no other software firm that offers the flexibility, functionality and
			responsiveness and cost effectiveness of Debt$Net®. We look optimistically toward a future of
			many more years with our friend at the Computer Manager.
			<br><br>
			<span> Harry Strausser</span>
		</p>
		
	</div>

	<div>
		<h2>CEO - Receivables Management Solutions, Inc. (RMS)</h2>
		<h3 id="subSpace">
			"Throughout the 8 years that RMS has been using Debt$Net®,we have consistant product quality,
			annual updates, and improvements to the Debt$Net® software."
		</h3>
		<p>
			The collection software product Debt$Net® has met every expectation RMS has needed. The
			customized programming RMS required has allowed us to service any client we pursued.
			Throughout the 8 years that RMS has been using Debt$Net®,we have consistant product quality,
			annual updates, and improvements to the Debt$Net® software. The technical support and
			customized programmers provide great services and support in a timely manner. TIME is money,
			Debt$Net® understands this fact. Over the years Debt$Net® has developed a strategy to handle
			their clients through organized systems/operations which prevents serious issues. I have
			learned over the years that software does what you program it to do. With Debt$Net®, the
			programmers have made my wishes come true. Ask and will receive! That's the approach I use
			when making business decisions that focus on growth and success. I support Debt$Net and
			recommend it to anyone who is looking for a produvt that works as well as a big product,
			without big cost. <br> <br> <span> Robert Dunham</span>
		</p>
		
    
	</div>

</body>

<style lang="scss">
	@import 'styles/components';

	

	h3 {
		font-style: italic;
		font-weight: 600;
		margin: 2% 9%;
	}

	span {
		margin: 0 0 4% 18%;
	}

	
.art-banner {
    background-color: rgb(0, 80, 112);
    height: 100vh;
    display: grid;
    grid-template-columns: 20px 1fr 1fr 1fr 20px;
    grid-template-rows: 20px 1fr 1fr 1fr 20px;

	input,
    textarea{
        width: 100%;
        font-size: 3vw;
        background: $backgroundSecond;
        border: none;
        border-radius:2px;
        outline: none;
        border-bottom: 1px solid $textMain;
        transition:0.3s linear;
    }

    input:focus,
    input:valid,
    textarea:focus,
    textarea:valid{
        padding: 10px;
        color: $textMain;
        background: $backgroundSecond;
        margin: 10px;
        border-radius:4px;
        font-size: 2.5vw;
    }
}

.art-banner-bg {
    background: url(img/Mt.jpg);
    background-size: cover;
    grid-column: 1 / -1;
    grid-row: 1 / -1;
	
}

.banner-text {
	@include glassBack();

    color: #fff;
    font-size: 6vw;
    font-weight: bold;
    grid-column: 1 / span 2;
    grid-row: 2 /* no need to type one*/;
    align-self: center;
    justify-self: center;
}

.form {
    grid-column: 2;
    grid-row: 4;
    z-index: 10;
	margin: 12%;

	button{
		background: $extra;
        outline: none;
        font-weight: 500;
        letter-spacing: 4px;
        border: 1px solid $extra;
        border-radius:4px;
        color: $backgroundMain;
        text-transform: uppercase;
        padding: 5px;
        margin: 14%;
        font-family: $mainFont;


        &:hover {
        transition: all 0.3s ease-in-out;
        background: $textMain;
        color: $backgroundMain;
        font-weight: 800;
        transform: scale(1.05);
        cursor: pointer;
        }
}
}

.badge {
    display: grid;
    align-self: center;
    justify-self: center;
    grid-column: 4 / 5;
    grid-row: 4 / 4;
    background-color: $backgroundMain;
    font-size: 2.5vw;
    font-weight: bold;
    width: 10vw;
    height: 10vw;
    border-radius: 50%;
    transform: rotate(15deg);

	p {
    margin:auto;
}
}

	.contBar {
		background: $extra;
		color: $backgroundMain;
		margin: 10% 0;
		overflow: hidden;

		a {
			background: $textSecond;
			border-radius: 4px;
			padding: 1%;
			margin: 60%;
			color: $backgroundMain;

			&:hover {
				color: $textSecond;
				background: $backgroundMain;
				transition: $transitSpeed;
			}
		}

		p{
			margin: 6% 10%;
		}
	}

	.mail{
        h2{
			margin: -5% 10%;
		}
    }

	.testim {
		background: $extra;
		color: $backgroundMain;
		padding: 4% 0;
	}

	.centered {
		background: #0a327681;
    }

	#subSpace{
		margin-bottom: -8%;
	}

	.indi{
		max-width:30%;
		margin:0 15%;
	}

	@media (max-width: 991px) {      }

	@media (max-width: 768px) {

		.contBar{
			margin: 4% 0;
		}
	}

		/*Extra Large screens */
      	@media only screen and (min-width: 1400px) {}
</style>


