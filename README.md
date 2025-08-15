# Mojo-sales-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Launch Your Aviation Career in 9-12 Months | Lookup Flight Academy</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            overflow-x: hidden;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #0B1929 0%, #1E3A8A 50%, #3B82F6 100%);
            min-height: 100vh;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 800"><path d="M100,400 Q300,200 600,350 T1100,300" stroke="rgba(255,255,255,0.1)" stroke-width="2" fill="none"/><path d="M0,500 Q400,300 800,450 T1200,400" stroke="rgba(255,255,255,0.1)" stroke-width="2" fill="none"/></svg>');
            opacity: 0.3;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            padding: 80px 0;
            text-align: center;
            color: white;
        }

        .preheader {
            background: rgba(59, 130, 246, 0.2);
            color: #60A5FA;
            padding: 8px 16px;
            border-radius: 20px;
            display: inline-block;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 30px;
            border: 1px solid rgba(59, 130, 246, 0.3);
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 900;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero .subheader {
            font-size: 1.3rem;
            margin-bottom: 40px;
            color: #E5E7EB;
            font-weight: 400;
            line-height: 1.5;
        }

        .vsl-container {
            margin: 40px 0;
        }

        .vsl-icon {
            display: inline-block;
            position: relative;
            background: linear-gradient(45deg, #EF4444, #DC2626);
            border-radius: 20px;
            padding: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        .vsl-icon:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        .play-button {
            width: 80px;
            height: 80px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 15px;
            position: relative;
        }

        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 25px solid #333;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 5px;
        }

        .vsl-text {
            color: white;
            font-weight: bold;
            font-size: 1.1rem;
        }

        .primary-cta {
            background: linear-gradient(45deg, #F59E0B, #D97706);
            color: white;
            padding: 18px 40px;
            font-size: 1.2rem;
            font-weight: bold;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-top: 30px;
            box-shadow: 0 8px 25px rgba(245, 158, 11, 0.3);
        }

        .primary-cta:hover {
            transform: translateY(-2px);
            box-shadow: 0 12px 35px rgba(245, 158, 11, 0.4);
        }

        /* Section Styling */
        .section {
            padding: 80px 0;
            background: white;
        }

        .section:nth-child(even) {
            background: #F8FAFC;
        }

        .section h2 {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 30px;
            text-align: center;
            color: #1E293B;
        }

        .section-content {
            font-size: 1.1rem;
            line-height: 1.8;
            max-width: 800px;
            margin: 0 auto;
        }

        .section-content p {
            margin-bottom: 25px;
        }

        /* Problem Section */
        .problem {
            background: linear-gradient(135deg, #DC2626 0%, #991B1B 100%);
            color: white;
        }

        .problem h2 {
            color: white;
        }

        /* Bullets */
        .bullets {
            margin: 40px 0;
        }

        .bullet {
            background: white;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-left: 5px solid #3B82F6;
        }

        .bullet h3 {
            color: #1E40AF;
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        /* Testimonial */
        .testimonial {
            background: linear-gradient(135deg, #1E40AF 0%, #1E3A8A 100%);
            color: white;
            padding: 40px;
            border-radius: 20px;
            margin: 40px 0;
            text-align: center;
        }

        .testimonial-quote {
            font-size: 1.3rem;
            font-style: italic;
            margin-bottom: 20px;
        }

        .testimonial-author {
            font-weight: bold;
            color: #93C5FD;
        }

        /* CTA Buttons */
        .cta-button {
            background: linear-gradient(45deg, #F59E0B, #D97706);
            color: white;
            padding: 16px 35px;
            font-size: 1.1rem;
            font-weight: bold;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
            display: inline-block;
            text-decoration: none;
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(245, 158, 11, 0.4);
        }

        /* FAQ */
        .faq-item {
            background: white;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .faq-question {
            font-weight: bold;
            font-size: 1.2rem;
            color: #1E40AF;
            margin-bottom: 15px;
        }

        .faq-answer {
            line-height: 1.7;
        }

        /* Mobile Responsiveness */
        @media (max-width: 1024px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .section {
                padding: 60px 0;
            }
        }

        @media (max-width: 768px) {
            .container {
                padding: 0 15px;
            }

            .hero h1 {
                font-size: 2.2rem;
            }

            .hero .subheader {
                font-size: 1.1rem;
            }

            .section h2 {
                font-size: 2rem;
            }

            .section-content {
                font-size: 1rem;
            }

            .primary-cta, .cta-button {
                padding: 14px 25px;
                font-size: 1rem;
            }

            .play-button {
                width: 60px;
                height: 60px;
            }

            .play-button::after {
                border-left: 20px solid #333;
                border-top: 12px solid transparent;
                border-bottom: 12px solid transparent;
            }
        }

        /* Emphasis Styles */
        .bold { font-weight: bold; }
        .caps { text-transform: uppercase; }
        .italic { font-style: italic; }
        .highlight { background: #FEF3C7; padding: 2px 6px; border-radius: 4px; }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="preheader">For Aspiring Pilots Ages 17-35</div>
                
                <h1>Launch Your Aviation Career in Just <span class="highlight" style="color: #F59E0B;">9-12 Months</span> Without Going Broke or Wasting Years</h1>
                
                <p class="subheader">Go from zero flight hours to commercial pilot ready... even if you've never touched aircraft controls before</p>
                
                <div class="vsl-container">
                    <a href="https://docs.google.com/document/d/1-PoarB65-clK8_qadhc1GSyrKJQyR-dA5_nNgeJ4qlU/edit?usp=sharing" class="vsl-icon" target="_blank">
                        <div class="play-button"></div>
                        <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                    </a>
                </div>
                
                <button class="primary-cta">Schedule Your Demo Flight Today</button>
            </div>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="section problem">
        <div class="container">
            <h2>The Dirty Truth About Why 90% of Aspiring Pilots Never Make It...</h2>
            
            <div class="section-content">
                <p>Picture this...</p>
                
                <p>You're sitting at your desk right now, scrolling through job postings that make you want to bang your head against the wall.</p>
                
                <p>Same boring routine. Same paycheck that barely covers the bills. Same <span class="italic">soul-crushing</span> realization that you're stuck in a career that feels like prison.</p>
                
                <p>Meanwhile, your buddy from high school just posted another photo from the cockpit of a 737... flying to Hawaii... again.</p>
                
                <p><span class="bold">And you KNOW you could do that job.</span></p>
                
                <p>You've researched flight schools...</p>
                
                <p>You've calculated the costs...</p>
                
                <p>You've even called a few places...</p>
                
                <p>But every single time, you hit the same brick walls:</p>
                
                <div class="bullets">
                    <div class="bullet">
                        <h3>💸 Insane Upfront Costs</h3>
                        <p>$80,000... $120,000... some places want $200,000+ just to START. Who has that kind of cash lying around?</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>⏰ Years of Your Life Gone</h3>
                        <p>Most programs drag on for 3-5 years. You'll be middle-aged before you even get your first real flying job.</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>🎓 Cookie-Cutter Training</h3>
                        <p>They pump you through like cattle, focusing on minimum hours instead of actual competence. You graduate scared to fly solo.</p>
                    </div>
                </div>
                
                <p>So you keep putting it off...</p>
                
                <p>Another year passes...</p>
                
                <p>Another birthday where you blow out candles wishing you were 30,000 feet up instead of stuck in traffic.</p>
                
                <p><span class="caps bold">But what if I told you there's a proven way to break through ALL of these barriers?</span></p>
            </div>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="section">
        <div class="container">
            <h2>How a Small Georgia Flight School Cracked the Code on Fast-Track Pilot Training</h2>
            
            <div class="section-content">
                <p>Three years ago, the team at Lookup Flight Academy was fed up.</p>
                
                <p>They watched student after student walk through their doors with big dreams... only to drop out six months later when reality hit.</p>
                
                <p>The problem wasn't lack of desire.</p>
                
                <p>The problem wasn't lack of ability.</p>
                
                <p><span class="bold">The problem was the entire flight training industry was broken.</span></p>
                
                <p>Schools were designed to milk students for years... not actually get them into cockpits FAST.</p>
                
                <p>So they did something radical.</p>
                
                <p>They threw out the "traditional" training model completely.</p>
                
                <p>Instead of spreading training over 3-5 years like everyone else...</p>
                
                <p>Instead of demanding massive upfront payments...</p>
                
                <p>Instead of treating students like numbers...</p>
                
                <p>They created something entirely different:</p>
                
                <p><span class="italic">A structured, accelerated program that gets you from zero hours to commercial pilot in just 9-12 months... with financing options that won't bankrupt you... in an environment where you're actually SUPPORTED instead of abandoned.</span></p>
                
                <div class="testimonial">
                    <div class="testimonial-quote">"I went from never touching aircraft controls to landing my first airline job in under 11 months. The traditional schools wanted 4 years and $180,000. Lookup got me there faster, cheaper, and with confidence I never thought possible."</div>
                    <div class="testimonial-author">— Mariah Ervin, Commercial Pilot</div>
                </div>
            </div>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="section">
        <div class="container">
            <h2>The "Accelerated Competency Method" That's Getting Pilots Job-Ready in Record Time</h2>
            
            <div class="section-content">
                <p>Here's what makes Lookup's approach completely different...</p>
                
                <p>While other schools focus on hitting minimum FAA hours (and nothing else), Lookup uses what they call the <span class="bold">"Accelerated Competency Method."</span></p>
                
                <p>Instead of dragging training out over years...</p>
                
                <p>You get <span class="caps">intensive, daily flight training</span> in modern, technically advanced aircraft with avionics you'll actually use in professional cockpits.</p>
                
                <p>Instead of generic classroom lectures...</p>
                
                <p>You get specialized ground sessions covering real-world scenarios: weather systems that'll try to kill you, engine failures at the worst possible moments, and navigation in conditions that would make seasoned pilots sweat.</p>
                
                <p>Instead of being treated like just another student...</p>
                
                <p>You get personalized attention in an inclusive environment that actually WANTS you to succeed.</p>
                
                <p><span class="bold">The result?</span></p>
                
                <p>Students who graduate not just with licenses... but with the confidence and competence to handle whatever the skies throw at them.</p>
                
                <div class="bullets">
                    <div class="bullet">
                        <h3>🎯 Precision Training Timeline</h3>
                        <p>Private Pilot: 3-6 months (not 2+ years like traditional schools) → You're flying solo while your friends are still sitting in ground school</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>✈️ Professional-Grade Aircraft</h3>
                        <p>Modern light sport aircraft with advanced avionics proven in flight schools → You train on equipment that mirrors what airlines actually use</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>🏠 All-Inclusive Support System</h3>
                        <p>Private furnished housing 15 minutes from airport + all supplies included → You focus on flying, not logistics</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>💰 Flexible Financing That Actually Works</h3>
                        <p>Low monthly payments or full deferment up to 20 years → Start training now, pay as your career takes off</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="section">
        <div class="container">
            <h2>Introducing the Complete Pilot Training System That Gets You Job-Ready FAST</h2>
            
            <div class="section-content">
                <p>This isn't just another flight school.</p>
                
                <p>This is a complete career transformation system designed for people who are <span class="caps">serious</span> about becoming professional pilots.</p>
                
                <p><span class="bold">Here's exactly what you get:</span></p>
                
                <div class="bullets">
                    <div class="bullet">
                        <h3>Private Pilot License (PPL) Track</h3>
                        <p><span class="bold">3-6 months, 80 flight hours, $24,840</span> → Perfect for those wanting to fly for personal enjoyment or as stepping stone to commercial</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>Commercial Pilot Career Track</h3>
                        <p><span class="bold">9-12 months, up to 260 flight hours</span> → Takes you from zero to Commercial Pilot License + Certified Flight Instructor rating</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>Modern Aircraft Fleet</h3>
                        <p>Technically advanced light sport aircraft with thousands of logged training hours → You'll feel confident in any cockpit</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>Student Housing Included</h3>
                        <p>Private furnished bedrooms, shared amenities, high-speed Wi-Fi, 15 minutes from airport → Focus on training, not finding a place to live</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>All Equipment Provided</h3>
                        <p>iPad with ForeFlight, headsets, all necessary supplies, PLUS all FAA test fees covered → No surprise costs or hidden fees</p>
                    </div>
                    
                    <div class="bullet">
                        <h3>Flexible Financing Options</h3>
                        <p>Wurthy (low monthly payments) or Stratus (full deferment up to 20 years) → Pre-approval in minutes, funds paid directly to academy</p>
                    </div>
                </div>
                
                <p>Compare that to traditional flight schools that...</p>
                
                <p>❌ Drag training out 3-5 years</p>
                <p>❌ Demand $100,000+ upfront</p>
                <p>❌ Leave you scrambling for housing and equipment</p>
                <p>❌ Graduate you with minimum skills and maximum debt</p>
                
                <p><span class="bold">Lookup gives you everything you need to succeed... in a fraction of the time... at a price that won't destroy your financial future.</span></p>
            </div>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="section problem">
        <div class="container">
            <h2>Here's How to Secure Your Spot and Start Flying This Month</h2>
            
            <div class="section-content">
                <p>Private Pilot License: <span class="bold caps">$24,840</span> (all-inclusive, no hidden fees)</p>
                
                <p>Commercial Pilot Career Track: <span class="bold">Contact for current pricing and financing options</span></p>
                
                <p><span class="italic">But here's the thing...</span></p>
                
                <p>Lookup can only accept a limited number of students each quarter due to aircraft availability and instructor ratios.</p>
                
                <p>They could easily pack 100+ students into each class... but then you'd get the same mediocre experience as everywhere else.</p>
                
                <p>Instead, they cap enrollment to ensure every student gets the personalized attention they deserve.</p>
                
                <p><span class="bold">Which means spots for the next quarter are filling up fast.</span></p>
                
                <div style="text-align: center; margin: 40px 0;">
                    <a href="#" class="cta-button">Schedule Your Demo Flight & Tour</a>
                </div>
                
                <p style="text-align: center;"><span class="italic">Last 3 enrollment periods sold out in under 2 weeks</span></p>
            </div>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="section">
        <div class="container">
            <h2>Everything You're Wondering (And Why None of It Should Stop You)</h2>
            
            <div class="faq-item">
                <div class="faq-question">"What if I can't afford the upfront cost?"</div>
                <div class="faq-answer">That's exactly why Lookup partnered with Wurthy and Stratus financing. You can start with low monthly payments or even defer payments completely while you train. Pre-approval takes minutes, and funds go directly to the academy. Stop letting money be an excuse to stay stuck in a job you hate.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">"I've never flown before. What if I'm not cut out for this?"</div>
                <div class="faq-answer">Perfect. That means you won't have any bad habits to break. Lookup specializes in taking complete beginners and turning them into confident pilots. Their instructors focus on building competence, not just checking boxes. If you can drive a car, you can learn to fly.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">"How do I know I'll actually get hired after graduation?"</div>
                <div class="faq-answer">The aviation industry is desperate for qualified pilots right now. Airlines are offering signing bonuses and fast-track programs for new graduates. Lookup doesn't just get you licensed – they get you <span class="italic">competent</span>. Competent pilots get hired. Period.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">"What if I fail the FAA checkride?"</div>
                <div class="faq-answer">Lookup's students have one of the highest first-time pass rates in Georgia. Why? Because they train you beyond minimums. You'll be overprepared, not underprepared. Plus, all test fees are included – no additional cost if you need a retry.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">"Can I really finish in 9-12 months?"</div>
                <div class="faq-answer">Yes, but only if you're committed. This isn't a part-time hobby program. It's intensive, daily training designed for people serious about changing their lives. If you're looking for something casual, this isn't for you. If you want results fast, this is exactly what you need.</div>
            </div>
            
            <div style="text-align: center; margin: 50px 0;">
                <p style="font-size: 1.3rem; margin-bottom: 30px;"><span class="bold">Your dream of flying professionally is closer than you think.</span></p>
                <a href="#" class="cta-button">Book Your Demo Flight Now</a>
                <p style="margin-top: 20px; font-style: italic;">650 Airport Rd, Lawrenceville, GA | Call 1-770-341-4277</p>
            </div>
        </div>
    </section>
</body>
</html>
