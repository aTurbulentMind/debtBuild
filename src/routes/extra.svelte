<body>

    <h1>Extra's Page</h1>

    

  <ul>
      <p>Things you can find here</p>
  <li class="dropdown">
    <a href="#skip" class="dropbtn">Newsletter</a>
    </li>
  <li class="dropdown">
    <a href="#dePay" class="dropbtn">Events</a>
  </li>
  <li class="dropdown">
    <a href="#deCont" class="dropbtn">Request a demo</a>
  </li>
  
</ul>

    <br><br><br><br>

<h2>Newsletter</h2>

<p>Keep up to date with the goins on of the great god Amway! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam perferendis cum voluptatem. Corrupti, esse perspiciatis reprehenderit natus incidunt consequatur quos enim voluptate inventore laboriosam aperiam dicta suscipit rem ipsum eius!</p>

<h3>2021 Newsletter:</h3>

<p><a href="/pdf/20213.pdf" download> Summer 2021 </a></p>

<h3>2019 Newsletters:</h3>

<p><a href="/pdf/20213.pdf/" download> Spring 2019 </a> | <a href="/pdf/20213.pdf/" download> Summer 2019 </a></p>


<h2>Events</h2>

<p>
    Upcoming events to be anounced.
</p>


<h2>Request a demo</h2>

    <p>If you feel Debt$Net® Collection Software may meet your needs, please fill out the download request form. We can then send you a link for a fully functional copy of either Debt$Ne®t Power or Debt$Net® Prestige to explore on a 30-day trial basis. Guided Walk-Thrus of the software can also be arranged by calling <a href="tel: +8005528397/">1-800-552- 8397</a></p>


    
   
    <container>
        
        <form action="https://formsubmit.co/joelkrivers@yahoo.com" method="POST">
            <wrapper>
                <box>
                    <input type="text" name="fname" id="fname" required>
                    <label for="fname">First and Last</label>
                </box>
            </wrapper>

            <wrapper>
                <box>
                    <input type="text" name="email" id="email" required>
                    <input type="hidden" name="_next" value="https://tender-benz-1741cd.netlify.app/">
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

           

            
            <wrapper>
            <box>
            <div class="select">
            <select name="format" id="format">
            <option selected disabled>Free eval form?</option>
            <option value="yes">Yes</option>
            <option value="no">No</option>
            </select>
            </div>
            </box>
            </wrapper>

           

            
            <wrapper>
            <box>
            <div class="select">
            <select name="format" id="format">
            <option selected disabled>Type of collection agency:</option>
            <option value="legal">Legal</option>
            <option value="medical">Medical</option>
            <option value="firstparty">1stparty</option>
            <option value="retail">Retail</option>
            <option value="check">Check</option>
            <option value="commercial">Commercial</option>
            <option value="portfolio">Portfolio Purchase</option>
            <option value="precollect">Precollect</option>
            </select>
            </div>
            </box>
            </wrapper>

            

          <!-- <input type="submit" name="" value="send">--> 
            <button type="submit">Submit</button>
        </form>
    </container>

    


</body>

<style lang="scss">
    @import 'styles/components';

    *{
        
        box-sizing: border-box;
    }

    h1{
    margin-top: 5%;
}

h3{
    margin:2% 10%
}

    
ul {
  float: right;
  list-style-type: none;
  margin:4% 17%;
  overflow: hidden;
  background-color: $extra;
  border-radius: 3px;
  box-shadow: 0 3px 8px 3px $textMain;
}

li {
  float: left;
}

li a, .dropbtn {
  
  color: $backgroundMain;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
  color: $highlight;
}

li.dropdown {
  display: inline-block;
}

.dropdown:hover {
  display: block;
}



    container{
        
        color: $backgroundMain;
        

        h2{
        font-size: 3vw;
        text-align: center;
        grid-column: 1;
    }

        p{
          margin:3% 5%;
          text-transform: capitalize;
        }

    form{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(275px, 1fr));
        background: $extra;
        width: 75%;
        margin:8%;
        padding: 4%;
        border-radius:4px;
        box-shadow: 0 2px 20px 2px rgba(6, 2, 7, 0.464);
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

    .double{
        grid-column: span 3;
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

    .section1, .section2{
        checkbox{
            padding-top: 80px;
        }

        input{
            accent-color: $highlight;
            block-size: 85px;
            inline-size:20px;
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
        margin:0;
        grid-column: 1;

        &:hover {
        transition: all 0.2s ease-in-out;
        background: $textMain;
        color: $backgroundMain;
        transform: scale(1.05);
        }
 }

 select {
   -webkit-appearance:none;
   -moz-appearance:none;
   -ms-appearance:none;
   appearance:none;
   outline:0;
   box-shadow:none;
   background: $textSecond;
   background-image: none;
   flex: 1;
   padding: 0 .5em;
   color:$backgroundMain;
   cursor:pointer;
   font-size: 1em;
   font-family: 'Open Sans', sans-serif;
}
select::-ms-expand {
   display: none;
}
.select {
   position: relative;
   display: flex;
   width: 20em;
   height: 3em;
   line-height: 3;
   background: $textSecond;
   overflow: hidden;
   border-radius: .25em;
   
}
.select::after {
   content: '\25BC';
   position: absolute;
   top: 0;
   right: 0;
   padding: 0 1em;
   background: rgba(16, 15, 17, 0.616);
   cursor:pointer;
   pointer-events:none;
   transition:.25s all ease;
}
.select:hover::after {
   color: #23b499;
}

     @media (max-width: 768px) {

        container{
            form{
                width: 80%;
            }
            label{
                font-size: 3vw;
                padding: 5px;
            }

            .double{
                grid-column: span 1;
            }
        }
            
    }

    /*Extra Large screens */
      	@media only screen and (min-width: 1400px) {

            container{
                form{
        grid-template-columns: repeat(auto-fit, minmax(475px, 1fr));
    }

            label{
                font-size: 1.5vw;
                padding: 5px;
                }
            
            input,
            textarea{
                font-size: 1vw;
                }

            input:focus,
            input:valid,
            textarea:focus,
            textarea:valid{
                margin: 4% 1%;
            }

            .section1, .section2{
            checkbox{
            padding-top: 50px;
            }

            input{
            accent-color: $highlight;
            block-size: 100px;
            inline-size:20px;
            }

            input:focus,
            input:valid,
            textarea:focus,
            textarea:valid{
            padding: 0.5px;
            margin: 0.5px;
            }
    }
}
          

      	}

</style>