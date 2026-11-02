# Video Presentation Script & Viva Preparation Guide
**Project:** ProcureEase – Construction Material Procurement System  
**Team:** The `<body>` Builders  
**Team Leader:** Rudra Rastogi (Reg No: 12607319)  
**Member 2:** Reg No: 12606268  
**Member 3:** Reg No: 12615445  

---

## 🎬 Part 1: Video Presentation Script (Target Duration: ~3 to 5 Minutes)
*All 3 members must speak during the video recording.*

### ⏱️ 0:00 - 1:00 | Speaker 1: Rudra Rastogi (Team Leader - 12607319)
**Visual on screen:** Dashboard Page (`page-dashboard`)

> "Good day, Respected Evaluators and Faculty. I am Rudra Rastogi, Registration Number 12607319, representing team 'The <body> Builders'. 
>
> Our assigned problem focuses on **Construction Material Procurement**. In real-world construction projects, teams face critical delays because material requirements are scattered across WhatsApp messages, emails, and manual paperwork. There is often no easy way to track quantities, compare competitive vendor quotations, or monitor real-time shipment status across different construction sites.
>
> To solve this, we developed **ProcureEase**, a streamlined web-based procurement workflow system built using clean HTML5, modern CSS3 styling, and client-side JavaScript.
>
> As shown on screen, our **Procurement Dashboard** serves as the central control room. It provides instant key metrics—such as total requisitions, approved purchases, pending shipments, and material spending breakdown charts. I was responsible for the core application architecture, overall UI/UX structure, and the integration of the dashboard analytics."

---

### ⏱️ 1:00 - 2:30 | Speaker 2: Member 2 (Reg No: 12606268)
**Visual on screen:** Switch to Material Requests (`page-requests`) and then Quotation Comparison (`page-quotations`).

> "Hello everyone, I am Member 2, Registration Number 12606268. My contribution centered on the **Material Requisitions** and **Quotation Comparison** modules.
>
> Let us look at the **Material Requests** screen. Site engineers on the ground can quickly create a formal request by selecting materials like Cement, TMT Steel Rods, or Aggregate, specifying precise quantities, choosing the construction site, setting required dates, and assigning priority levels like High or Urgent. Clicking 'Submit Request' dynamically validates the input and prepends a new record to our requests table in real time.
>
> Moving to the **Quotation Comparison** module: once a request is logged, procurement teams receive bids from multiple suppliers. Our system displays these quotes side-by-side with unit rates, delivery timelines, payment terms, and vendor quality ratings, automatically highlighting the best market offer so the team can award the purchase order transparently and save capital."

---

### ⏱️ 2:30 - 4:00 | Speaker 3: Member 3 (Reg No: 12615445)
**Visual on screen:** Switch to Cost Simulator (`page-simulator`) and then Delivery Status (`page-delivery`).

> "Hello, I am Member 3, Registration Number 12615445. I worked on the **Procurement Cost Simulator** and the **Delivery Tracking** subsystem.
>
> One of our standout functional features is the **Cost Simulator**. Before committing to purchase orders, project managers need an accurate financial projection. In our simulator, users can add multiple material line items, adjust order quantities, and define overhead parameters like GST rate, transit freight, and labor handling charges. When I click 'Calculate Total Cost', the algorithm instantly computes item sub-totals, applies the exact GST tax brackets, adds logistical overheads, and calculates the comprehensive Grand Total in Indian Rupees.
>
> Furthermore, on the **Delivery Status** page, teams can monitor shipment milestones with a step-by-step visual tracker—from warehouse loading to live transit and final on-site receipt—drastically reducing site downtime."

---

### ⏱️ 4:00 - End | Conclusion by Rudra Rastogi
**Visual on screen:** Team Info Page (`page-team`) with GitHub and Deployment links shown.

> "To conclude, ProcureEase delivers a complete, responsive, and intuitive solution tailored specifically to our problem statement. Our source code is organized in our GitHub repository and live deployed for online evaluation. Thank you for your time and guidance."

---

## 🎯 Part 2: Viva Voce Preparation Guide (10 Marks)

### Q1: Why did you choose HTML, CSS, and JavaScript for this project?
- **Answer:** HTML5 provides semantic, accessible structure for forms, navigation, and tabular data. CSS3 allows us to create responsive Grid and Flexbox layouts without heavy third-party CSS frameworks. JavaScript powers the reactive client-side simulator calculations, input validation, and tab transitions without requiring a complex backend setup.

### Q2: How does the Cost Simulator calculate the total price?
- **Answer:** The simulator queries all active material rows from the DOM, retrieves the unit price from the selected `<option>` dataset, multiplies it by the quantity input, sums them to form the subtotal, calculates the GST using `(subtotal * gstRate / 100)`, adds transport, labor, and miscellaneous overheads, and formats the output using `toLocaleString('en-IN')`.

### Q3: How is the application organized for responsive viewing on mobile screens?
- **Answer:** We implemented CSS media queries (`@media (max-width: 768px)` and `(max-width: 1100px)`) that collapse the fixed sidebar into a fluid layout, change multi-column grids into single-column vertical stacks, and wrap data tables in horizontal scroll containers.

### Q4: What happens when an invalid request is submitted?
- **Answer:** The input fields are validated by JavaScript functions. If required fields like material name, quantity, or due date are left blank, an interactive warning banner is dynamically injected to notify the user without refreshing the page.
