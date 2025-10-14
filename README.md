# 🚗 Automotive Production Workflow (ERP Panthera + EDI Integration)

## 📋 Overview
This BPMN diagram represents a **complete production and delivery workflow** in an **automotive manufacturing company** using **ERP Panthera** with **EDI integration**.  
The process covers the entire cycle — from receiving customer orders via EDI to generating invoices and transmitting EDI INVOICE messages.

---

## 🧱 Main Steps

1. **📨 Order Reception (EDI)**
   - Customer sends an **EDI message (ORDERS)**.
   - ERP Panthera imports and validates the EDI file.
   - If the order is correct → proceed to planning.  
     If validation fails → send error report to customer.

2. **🗓️ Production Planning**
   - The order is automatically added to the **production schedule**.
   - Planner verifies material availability (BOM check).
   - A **Production Order (Executive Order)** is generated.

3. **🏭 Production Execution**
   - Operators execute the order according to production plan.
   - Progress is reported in real time to ERP Panthera.
   - Quality control (QC) tests are performed.

4. **🧾 Production Documentation**
   - Upon completion, the system generates a **Production Document** and **Quality Test Report**.
   - Documents are stored in ERP and linked to the production batch.

5. **📦 Shipment**
   - Logistics prepares a **Delivery Note (DDT)**.
   - Shipment is dispatched and confirmed in ERP.
   - The system may send an **EDI DESADV (Dispatch Advice)** message to the customer.

6. **💰 Invoicing**
   - Based on the DDT, ERP automatically issues an **Invoice**.
   - EDI **INVOICE** message is transmitted to the customer’s system.
   - Process ends when the confirmation is received.

---

## 🧠 Tools
- Modeled in [ADONIS BPM](https://www.boc-group.com/adonis/)
- Exported as BPMN 2.0 XML and PNG

---

## 💡 Business Context
This workflow is typical for **Tier 1 suppliers** in the automotive industry.  
It ensures **traceability**, **data consistency**, and **automated EDI communication** between systems — from production planning to financial integration.

---

## 🏷️ Keywords
`BPMN` · `ADONIS` · `ERP Panthera` · `Automotive` · `EDI` · `DESADV` · `INVOICE` · `Production` · `Quality Control`

---

## 🖼️ Diagram Preview
![Automotive Production Workflow](your-diagram-file.png)
*(my diagram)*

---

### 📁 Repository Structure
