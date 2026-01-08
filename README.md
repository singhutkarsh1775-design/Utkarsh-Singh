# Utkarsh-Singh
Solution for Travel, Navigation and Mobility During Maha Kumbh In Nashik
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Community Navigation System | Nashik Kumbh Mela - Pilgrim Mobility Solution</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: #f7f7f7;
      color: #222;
      line-height: 1.8;
    }
    header {
      background: linear-gradient(135deg, #ff7a00 0%, #ff9500 100%);
      color: white;
      padding: 3rem 1rem;
      text-align: center;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
      font-weight: 700;
    }
    header p {
      font-size: 1.2rem;
      opacity: 0.95;
    }
    nav {
      background: white;
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 1.5rem;
      max-width: 1200px;
      margin: 0 auto;
    }
    nav a {
      color: #ff7a00;
      text-decoration: none;
      font-weight: 500;
      padding: 0.5rem 1rem;
      border-radius: 5px;
      transition: background 0.3s;
    }
    nav a:hover {
      background: #fff5e6;
    }
    section {
      padding: 3rem 1rem;
      max-width: 1200px;
      margin: 0 auto 2rem;
      background: white;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    h2 {
      color: #ff7a00;
      font-size: 2rem;
      margin-bottom: 1.5rem;
      font-weight: 600;
      border-left: 5px solid #ff7a00;
      padding-left: 1rem;
    }
    h3 {
      color: #333;
      font-size: 1.5rem;
      margin-bottom: 1rem;
      margin-top: 1.5rem;
      font-weight: 600;
    }
    h4 {
      color: #555;
      font-size: 1.2rem;
      margin-bottom: 0.5rem;
      margin-top: 1rem;
      font-weight: 500;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 1.5rem;
    }
    .card {
      padding: 1.5rem;
      background: linear-gradient(135deg, #fff5e6 0%, #ffffff 100%);
      border: 2px solid #ffe0b3;
      border-radius: 10px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 6px 12px rgba(255,122,0,0.2);
    }
    .card h3 {
      color: #ff7a00;
      margin-top: 0;
      font-size: 1.3rem;
    }
    ul {
      padding-left: 1.5rem;
      margin: 1rem 0;
    }
    ul li {
      margin-bottom: 0.8rem;
      line-height: 1.8;
    }
    .highlight-box {
      background: linear-gradient(135deg, #fff5e6 0%, #ffe0b3 100%);
      padding: 1.5rem;
      border-radius: 10px;
      border-left: 5px solid #ff7a00;
      margin: 1.5rem 0;
    }
    .solution-approach {
      background: #f0f8ff;
      padding: 1.5rem;
      border-radius: 10px;
      margin: 1rem 0;
      border-left: 5px solid #4a90e2;
    }
    .solution-approach h4 {
      color: #4a90e2;
    }
    .revenue-item {
      background: #f9f9f9;
      padding: 1rem;
      border-radius: 8px;
      margin: 0.8rem 0;
      border-left: 4px solid #ff7a00;
    }
    .payment-method {
      background: #e8f5e9;
      padding: 1rem;
      border-radius: 8px;
      margin: 0.8rem 0;
      border-left: 4px solid #4caf50;
    }
    .benefit-item {
      background: #fff3e0;
      padding: 1rem;
      border-radius: 8px;
      margin: 0.8rem 0;
      border-left: 4px solid #ff9800;
    }
    footer {
      background: #222;
      color: #ccc;
      text-align: center;
      padding: 2rem 1rem;
      margin-top: 3rem;
    }
    .cta {
      background: linear-gradient(135deg, #ff7a00 0%, #ff9500 100%);
      color: white;
      padding: 2rem;
      text-align: center;
      border-radius: 12px;
      margin-top: 2rem;
    }
    .cta h2 {
      color: white;
      border: none;
      padding: 0;
      margin-bottom: 1rem;
    }
    .cta p {
      font-size: 1.1rem;
      margin-bottom: 1.5rem;
    }
    .btn {
      background: white;
      color: #ff7a00;
      padding: 0.8rem 2rem;
      border: none;
      border-radius: 25px;
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1.5rem;
      margin: 2rem 0;
    }
    .stat-box {
      text-align: center;
      padding: 1.5rem;
      background: linear-gradient(135deg, #ff7a00 0%, #ff9500 100%);
      color: white;
      border-radius: 10px;
    }
    .stat-box h3 {
      color: white;
      font-size: 2.5rem;
      margin: 0;
    }
    .stat-box p {
      margin-top: 0.5rem;
      opacity: 0.95;
    }
    @media (max-width: 768px) {
      header h1 {
        font-size: 1.8rem;
      }
      nav ul {
        flex-direction: column;
        gap: 0.5rem;
      }
      h2 {
        font-size: 1.5rem;
      }
      .grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>🚶 Community Navigation System</h1>
  <p>People-Powered Mobility Solution for Nashik Kumbh Mela</p>
  <p style="font-size: 1rem; margin-top: 0.5rem; opacity: 0.9;">No Government Support • No Digital Dependency • Pure Community Power</p>
</header>

<nav>
  <ul>
    <li><a href="#problem">Problem</a></li>
    <li><a href="#solution">Solution</a></li>
    <li><a href="#benefits">Benefits</a></li>
    <li><a href="#revenue">Revenue</a></li>
    <li><a href="#payment">Payment</a></li>
    <li><a href="#scalability">Scalability</a></li>
    <li><a href="#prototype">Prototype</a></li>
     <li><a href="#Main Location"> Main Location</a></li>
  </ul>
</nav>

<section id="problem">
  <h2>🚨 Visitor Problem: Travel Navigation & Mobility</h2>
  <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
    During the Nashik Kumbh Mela, one of the most serious and real problems faced by pilgrims is difficulty in navigation and mobility within the crowded city and mela area.
  </p>
  
  <h3>Key Challenges:</h3>
  <div class="grid">
    <div class="card">
      <h3>🚧 Road Diversions</h3>
      <p>Roads are frequently diverted or closed, but pilgrims do not receive clear or real-time information.</p>
    </div>
    <div class="card">
      <h3>📍 Location Confusion</h3>
      <p>Visitors struggle to locate parking zones, temporary bus stops, railway station exits, ghats (Ramkund), akhada camps, and medical help centers.</p>
    </div>
    <div class="card">
      <h3>👴 Vulnerable Groups</h3>
      <p>Elderly pilgrims, women, and first-time visitors often get confused and lost in dense crowds.</p>
    </div>
    <div class="card">
      <h3>🚌 Transport Information</h3>
      <p>Information about local transport services (shuttle buses, e-rickshaws), including exact pick-up and drop-off points, is unclear.</p>
    </div>
    <div class="card">
      <h3>📱 Network Congestion</h3>
      <p>Mobile networks become congested, making digital maps unreliable, especially for non-tech-savvy pilgrims.</p>
    </div>
    <div class="card">
      <h3>⚠️ Safety Risks</h3>
      <p>Pilgrims face long walking distances, time loss, physical exhaustion, and safety risks, particularly on peak bathing days.</p>
    </div>
  </div>
</section>

<section id="solution">
  <h2>💡 Proposed Solution</h2>
  <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
    A hybrid on-ground and low-tech digital navigation system designed specifically for the high-density, low-connectivity environment of the Nashik Kumbh Mela.
  </p>

  <div class="solution-approach">
    <h3>🎨 Color-Coded Route System (Offline Friendly)</h3>
    <ul>
      <li>Divide the entire Kumbh area into color zones (Red Zone – Ramkund Ghats, Blue Zone – Akhada Camps, Green Zone – Parking & Bus Terminals)</li>
      <li>Paint the same colors on roads, barricades, poles, and signboards so pilgrims can follow routes without using phones</li>
    </ul>
  </div>

  <div class="solution-approach">
    <h3>🏪 Temporary Navigation Help Booths</h3>
    <ul>
      <li>Set up navigation kiosks at railway station exits, bus stands, parking areas, and major entry points</li>
      <li>Trained volunteers provide verbal directions, printed route maps, and walking-time estimates</li>
    </ul>
  </div>

  <div class="solution-approach">
    <h3>🚌 Dedicated Shuttle & Drop Points</h3>
    <ul>
      <li>Introduce clearly marked shuttle bus routes with fixed pick-up/drop points near ghats and camps</li>
      <li>Display large boards showing route name, color, destination, and frequency</li>
    </ul>
  </div>

  <div class="solution-approach">
    <h3>📱 Low-Data Mobile Navigation (Optional)</h3>
    <ul>
      <li>A lightweight offline map (QR-code based) that works even with poor network</li>
      <li>Shows current location, nearest ghat, toilets, medical aid, and lost-and-found centers</li>
    </ul>
  </div>

  <div class="solution-approach">
    <h3>📢 Public Announcements & Audio Guidance</h3>
    <ul>
      <li>Use loudspeakers at regular intervals to announce route updates, diversions, and peak crowd warnings in Hindi, Marathi, and English</li>
    </ul>
  </div>

  <div class="solution-approach">
    <h3>♿ Special Assistance for Elderly & Disabled Pilgrims</h3>
    <ul>
      <li>Separate assistance lanes, battery-operated vehicles, and volunteer escorts from entry points to ghats</li>
    </ul>
  </div>

  <h3 style="margin-top: 2rem;">🔄 Solution Approaches</h3>
  
  <div class="highlight-box">
    <h4>✅ With Data Analytics</h4>
    <ul>
      <li><strong>Crowd Density Analysis:</strong> Data from CCTV, drones, entry/exit counters analyzed to identify high-density zones</li>
      <li><strong>Real-Time Route Optimization:</strong> Analytics-driven dashboards show congested routes, enabling dynamic diversions</li>
      <li><strong>Predictive Crowd Flow:</strong> Historical data helps predict peak hours and high-risk locations</li>
      <li><strong>Smart Shuttle Planning:</strong> Usage data analyzed to adjust frequency and routes in real-time</li>
      <li><strong>Decision Support:</strong> Centralized dashboard provides live insights to administrators and emergency teams</li>
    </ul>
  </div>

  <div class="highlight-box">
    <h4>🌿 Without Digital Technology</h4>
    <ul>
      <li><strong>Manual Crowd Observation:</strong> Police, volunteers count crowd flow at fixed intervals and mark congestion on printed maps</li>
      <li><strong>Color-Coded Physical Routes:</strong> Entire area divided into color zones marked on roads, flags, poles, barricades</li>
      <li><strong>Flag & Board Control:</strong> Colored flags and flip boards (Green = open, Red = blocked, Yellow = slow)</li>
      <li><strong>Human Information Relay:</strong> Information moves person-to-person: Observation → supervisors → volunteers → pilgrims</li>
      <li><strong>Printed Maps & Symbols:</strong> Simple maps updated daily based on previous day's crowd behavior</li>
      <li><strong>Scheduled Flow Windows:</strong> Time-based movement slots based on observed data patterns</li>
    </ul>
  </div>

  <div class="highlight-box">
    <h4>👥 Without Government Help (Community-Driven)</h4>
    <ul>
      <li><strong>Volunteer-Based Teams:</strong> Local residents, shopkeepers, akhada members, NGOs form navigation teams</li>
      <li><strong>Community-Created Routes:</strong> Cloth ribbons, flags, ropes, painted arrows mark paths (Orange → Ramkund, Blue → Camps, White → Exit)</li>
      <li><strong>Handmade Signboards:</strong> Wooden/cardboard boards with arrows and symbols (footsteps, temple, water tap)</li>
      <li><strong>Human Information Chain:</strong> Volunteers pass information verbally about crowd density and safe alternatives</li>
      <li><strong>Observation-Based Management:</strong> Crowd pressure judged by walking speed, stopping points, visible discomfort</li>
      <li><strong>Temporary Rest Points:</strong> Local people offer shaded rest spots, water points outside homes/shops</li>
      <li><strong>Guided Group Movement:</strong> Small guided batches led by volunteers, especially during peak hours</li>
    </ul>
  </div>
</section>

<section id="benefits">
  <h2>✨ Direct Benefits to Visitors</h2>
  
  <div class="benefit-item">
    <h4>🧭 Easy Navigation Without Confusion</h4>
    <p>Visitors can quickly find ghats, camps, transport points, and facilities using color-coded routes and clear signage, even without smartphones.</p>
  </div>

  <div class="benefit-item">
    <h4>🚶 Reduced Walking & Physical Strain</h4>
    <p>Clear routes and shuttle services help pilgrims avoid unnecessary long walks, especially beneficial for elderly people, women, and children.</p>
  </div>

  <div class="benefit-item">
    <h4>⏱️ Time Saving</h4>
    <p>Visitors reach bathing ghats and accommodation faster, avoiding wrong turns and repeated backtracking during peak crowd hours.</p>
  </div>

  <div class="benefit-item">
    <h4>🛡️ Improved Safety in Crowded Areas</h4>
    <p>Organized movement reduces overcrowding, panic, and the risk of stampede-like situations.</p>
  </div>

  <div class="benefit-item">
    <h4>📶 Less Dependence on Mobile Network</h4>
    <p>Offline navigation and on-ground guidance work even when mobile networks fail due to heavy congestion.</p>
  </div>

  <div class="benefit-item">
    <h4>😌 Stress-Free Pilgrimage Experience</h4>
    <p>Pilgrims can focus on spiritual activities instead of worrying about directions or transport.</p>
  </div>

  <div class="benefit-item">
    <h4>🚨 Better Access to Emergency Services</h4>
    <p>Faster location of medical help, toilets, and help desks during emergencies.</p>
  </div>

  <div class="benefit-item">
    <h4>🤝 Inclusive & Visitor-Friendly</h4>
    <p>First-time visitors and non-tech-savvy pilgrims feel confident and supported throughout their journey.</p>
  </div>

  <div class="highlight-box" style="margin-top: 2rem;">
    <h3>💬 Why Visitors Will Pay</h3>
    <ul>
      <li><strong>Saves Physical Effort:</strong> Avoids unnecessary walking - especially valuable for elderly pilgrims</li>
      <li><strong>Reduces Stress & Fear:</strong> Human guidance provides certainty in dense crowds</li>
      <li><strong>Improves Safety:</strong> Controlled routes reduce congestion and safety risks</li>
      <li><strong>Respects Time Constraints:</strong> Saves hours of confusion for small fee</li>
      <li><strong>Human Help Builds Trust:</strong> Real volunteers talk, walk with them, answer questions</li>
      <li><strong>Feels Like Seva:</strong> Payment seen as seva/daan, not commercialization</li>
      <li><strong>Clear Value vs Low Cost:</strong> Small amount feels fair for visible benefits</li>
    </ul>
  </div>
</section>

<section id="revenue">
  <h2>💰 Revenue Generation Model</h2>
  <p style="margin-bottom: 1.5rem;">Sustainable and ethical revenue through community participation:</p>

  <div class="revenue-item">
    <h4>1. Sponsored Route Branding</h4>
    <p>Color-coded routes sponsored by local businesses (hotels, dharamshalas, medical stores, food stalls). Example: "Blue Route supported by XYZ Dharamshala" on flags/signboards.</p>
    <p><strong>Revenue:</strong> Fixed sponsorship fee per route or zone</p>
  </div>

  <div class="revenue-item">
    <h4>2. Printed Pilgrim Map & Guide (Low-Cost)</h4>
    <p>Sell simple printed navigation map (₹10–₹20) at railway stations, bus stands, and entry points. Includes routes, ghats, toilets, water points, rest areas.</p>
    <p><strong>Revenue:</strong> High volume × low price = steady income</p>
  </div>

  <div class="revenue-item">
    <h4>3. Volunteer-Led Group Navigation Service</h4>
    <p>Offer guided group movement (especially for elderly pilgrims, families, first-timers). Small charge per group (₹100–₹200).</p>
    <p><strong>Revenue:</strong> Service fee while ensuring safety and comfort</p>
  </div>

  <div class="revenue-item">
    <h4>4. Local Business Listings on Signboards</h4>
    <p>Nearby lodges, bhojanalayas, medical shops can list names on community signboards. Only location-based, no misleading ads.</p>
    <p><strong>Revenue:</strong> Listing fees from local vendors</p>
  </div>

  <div class="revenue-item">
    <h4>5. Rest & Help Points (Community Managed)</h4>
    <p>Community-run shaded rest spots with water, seating, first aid. Optional donation box or small usage fee.</p>
    <p><strong>Revenue:</strong> Voluntary donations from pilgrims</p>
  </div>

  <div class="revenue-item">
    <h4>6. NGO / CSR Partnerships</h4>
    <p>NGOs and corporates fund volunteer uniforms, signboards, printed maps as CSR. Their name appears as supporter.</p>
    <p><strong>Revenue:</strong> One-time or seasonal funding</p>
  </div>

  <div class="revenue-item">
    <h4>7. Training & Replication Model</h4>
    <p>After success, model sold as framework to other religious events, temple towns, large festivals.</p>
    <p><strong>Revenue:</strong> Training fees, manuals, consultancy</p>
  </div>

  <div class="revenue-item">
    <h4>8. Merchandise (Optional)</h4>
    <p>Simple items: route-color wristbands, badges, caps. Helps pilgrims remember route and supports volunteers.</p>
    <p><strong>Revenue:</strong> Merchandise sales</p>
  </div>

  <div class="stats">
    <div class="stat-box">
      <h3>Low</h3>
      <p>Setup Cost</p>
    </div>
    <div class="stat-box">
      <h3>High</h3>
      <p>Footfall = Scalable Income</p>
    </div>
    <div class="stat-box">
      <h3>Ethical</h3>
      <p>Non-Exploitative</p>
    </div>
  </div>
</section>

<section id="payment">
  <h2>💳 How Will Users Pay?</h2>
  <p style="margin-bottom: 1.5rem;">Simple, non-digital payment methods:</p>

  <div class="payment-method">
    <h4>1. Cash Payment at Help Points</h4>
    <p>Users pay small cash amounts directly at map counters, guided group navigation points, rest & help points. Clear rate cards displayed (e.g., Printed Map – ₹10, Group Guide – ₹100).</p>
    <p><strong>Why it works:</strong> Cash is universally accepted and easy for pilgrims of all ages.</p>
  </div>

  <div class="payment-method">
    <h4>2. Token / Coupon System</h4>
    <p>After payment, users receive colored paper token or wristband. Color matches route or service paid for. Tokens shown to volunteers during guided movement.</p>
    <p><strong>Why it works:</strong> Prevents confusion, avoids repeated payments, easy to verify.</p>
  </div>

  <div class="payment-method">
    <h4>3. Donation Boxes (Voluntary Payment)</h4>
    <p>Placed at rest points, exit routes, major ghats. Clearly labeled: "Support Volunteer Navigation Service".</p>
    <p><strong>Why it works:</strong> Pilgrims often prefer daan (donation) over compulsory fees.</p>
  </div>

  <div class="payment-method">
    <h4>4. Group-Based Payment</h4>
    <p>Families or yatri groups make one combined payment. One token issued for entire group.</p>
    <p><strong>Why it works:</strong> Feels fair, affordable, encourages adoption.</p>
  </div>

  <div class="payment-method">
    <h4>5. Pay-at-Entry Model</h4>
    <p>At main entry points, pilgrims can buy a map or opt for guided movement. No pressure—optional service.</p>
  </div>

  <div class="payment-method">
    <h4>6. Sponsored / Free for Users</h4>
    <p>In some zones, sponsors cover costs, so users pay nothing. Signboards mention: "Free service supported by local sponsors".</p>
  </div>

  <div class="highlight-box">
    <h4>Key Principle</h4>
    <ul>
      <li>No forced payment</li>
      <li>Low cost or donation-based</li>
      <li>Transparent pricing</li>
      <li>Cash-first, people-managed</li>
    </ul>
  </div>
</section>

<section id="scalability">
  <h2>🌍 Scalability Beyond Kumbh Mela</h2>
  
  <div class="highlight-box">
    <h3>✅ Yes - Highly Scalable</h3>
    <p style="font-size: 1.1rem; margin-bottom: 1rem;">
      This solution is highly scalable beyond the Kumbh Mela because it is low-cost, technology-independent, and community-driven.
    </p>
  </div>

  <h3>Can Scale To:</h3>
  <div class="grid">
    <div class="card">
      <h3>🕉️ Other Pilgrimages</h3>
      <p>Amarnath Yatra, Vaishno Devi, Tirupati, Pandharpur Wari</p>
    </div>
    <div class="card">
      <h3>🎉 Large Religious Events</h3>
      <p>Religious fairs, festivals, spiritual gatherings</p>
    </div>
    <div class="card">
      <h3>🏛️ Tourism-Heavy Cities</h3>
      <p>Heritage sites, crowded temple towns, tourist destinations</p>
    </div>
    <div class="card">
      <h3>🌐 International Mass Gatherings</h3>
      <p>Festivals, cultural events, sporting crowds globally</p>
    </div>
  </div>

  <div class="highlight-box" style="margin-top: 2rem;">
    <h4>Why It's Scalable:</h4>
    <ul>
      <li>Low-cost setup</li>
      <li>No technology dependency</li>
      <li>Community-driven model</li>
      <li>Simple operational playbooks</li>
      <li>Minimal customization needed</li>
      <li>Works without government support</li>
      <li>No digital infrastructure required</li>
    </ul>
  </div>
</section>

<section id="prototype">
  <h2>🔧 Working Prototype</h2>
  
  <div class="highlight-box">
    <h3>✅ Yes — We Have a Working Prototype</h3>
    <p style="font-size: 1.1rem; margin-bottom: 1rem;">
      While we do not rely on digital tools, we have a functional, real-world prototype that demonstrates how the solution works in practice.
    </p>
  </div>

  <h3>What the Prototype Includes:</h3>
  
  <div class="grid">
    <div class="card">
      <h3>🎨 Color-Coded Route Marking</h3>
      <p>Sample cloth flags, ribbons, and painted arrows used to mark routes. Each color represents a clear destination (ghats, camps, exits).</p>
    </div>
    <div class="card">
      <h3>📋 Handmade Signboards</h3>
      <p>Physical signboards with arrows and symbols (temple, footsteps, water). Designed to be readable from distance and usable by non-literate visitors.</p>
    </div>
    <div class="card">
      <h3>👥 Volunteer Navigation Setup</h3>
      <p>A small team of trained volunteers positioned at junctions. Volunteers use hand signals and verbal guidance to direct movement.</p>
    </div>
    <div class="card">
      <h3>🗺️ Printed Navigation Map</h3>
      <p>A simple black-and-white map showing routes, rest points, and key locations. Tested for clarity with first-time visitors.</p>
    </div>
    <div class="card">
      <h3>🚶 Guided Group Movement</h3>
      <p>Trial runs where small groups are guided from entry points to destinations, reducing confusion and congestion.</p>
    </div>
  </div>

  <div class="highlight-box" style="margin-top: 2rem;">
    <h4>How It Has Been Tested:</h4>
    <ul>
      <li>Tested in local religious gatherings and busy temple surroundings</li>
      <li>Observed outcomes: Reduced wrong turns, faster movement, higher confidence among elderly visitors</li>
      <li>Positive feedback and voluntary contributions received</li>
    </ul>
  </div>

  <div class="highlight-box">
    <h4>Why This Counts as a Working Prototype:</h4>
    <ul>
      <li>It physically exists, not just an idea</li>
      <li>It operates without government support or technology</li>
      <li>It proves that human-led navigation works in high-crowd environments</li>
    </ul>
  </div>

  <div class="highlight-box" style="background: #e3f2fd; border-left-color: #2196f3;">
    <h4 style="color: #2196f3;">Next Step:</h4>
    <p>We currently have a low-cost, on-ground prototype. The next phase is a pilot deployment at a mid-scale pilgrimage to measure flow time, congestion reduction, and visitor satisfaction before large-scale rollout.</p>
  </div>
</section>

<section id="main-spots">
  <h2>📍 Main Spots – Nashik Kumbh Mela</h2>
  <p style="margin-bottom: 1rem;">Key locations for pilgrims with quick map links.</p>
  <div class="grid">
    <div class="card">
      <h3>Ramkund</h3>
      <p>Main Shahi Snan ghat.</p>
      <a href="https://maps.google.com/?q=Ramkund,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Godavari Ghat</h3>
      <p>Extended bathing and crowd movement area.</p>
      <a href="https://maps.google.com/?q=Godavari+Ghat,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Trimbakeshwar Temple</h3>
      <p>Jyotirlinga & origin of Godavari.</p>
      <a href="https://maps.google.com/?q=Trimbakeshwar+Temple" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Tapovan</h3>
      <p>Sadhu-sant camps & temporary stay.</p>
      <a href="https://maps.google.com/?q=Tapovan,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Sadhugram</h3>
      <p>Akhada Parishad area.</p>
      <a href="https://maps.google.com/?q=Sadhugram,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Kalaram Mandir</h3>
      <p>Major religious landmark.</p>
      <a href="https://maps.google.com/?q=Kalaram+Mandir,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Panchavati</h3>
      <p>Mythological & spiritual zone.</p>
      <a href="https://maps.google.com/?q=Panchavati,Nashik" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>Nashik Road Railway Station</h3>
      <p>Main arrival point for pilgrims.</p>
      <a href="https://maps.google.com/?q=Nashik+Road+Railway+Station" target="_blank">View Location</a>
    </div>
    <div class="card">
      <h3>CBS Bus Stand, Nashik</h3>
      <p>Main bus terminal.</p>
      <a href="https://maps.google.com/?q=CBS+Bus+Stand+Nashik" target="_blank">View Location</a>
    </div>
  </div>
</section>

<section class="cta">
  <h2>🚀 Want to Pilot This Solution?</h2>
  <p>Join us in creating safer, smoother pilgrim experiences.</p>
  <p style="margin-top: 1rem; font-size: 0.95rem; opacity: 0.9;">Community Navigation Initiative | People • Safety • Seva</p>
</section>

<footer>
  <p>© 2024 Community Navigation Initiative | Nashik Kumbh Mela</p>
  <p style="margin-top: 0.5rem; font-size: 0.9rem;">People • Safety • Seva</p>
</footer>

</body>
</html>
