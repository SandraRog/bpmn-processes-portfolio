# 🚗 Automotive EDI-Based Order-to-Invoice Process (BPMN 2.0)

## 📖 Overview
This project presents a **BPMN 2.0 process model** illustrating the *Order-to-Invoice* flow in the **automotive industry**.  
It focuses on **EDI message exchange** between a customer and an ERP system, covering the entire business process —  
from **forecasting and planning** through **production**, **shipment**, and **invoicing**.

Although the workflow could be implemented in systems such as **ERP Panthera**,  
the main goal of this model is to visualize the **business process**, not system architecture.

---

## 🧭 Process Flow Summary
1. **Forecast (DELFOR)** – Customer sends forecast data via EDI, imported automatically into ERP for planning.  
2. **Delivery Schedule (DELJIT)** – Updates short-term delivery expectations.  
3. **Customer Order (ORDERS)** – Formal customer order triggers production planning.  
4. **Availability Check** – ERP verifies component availability.  
   - If components are missing → replenishment and customer notification.  
   - If available → proceed to production order creation.  
5. **Order Confirmation (ORDRSP)** – ERP sends order confirmation to the customer.  
6. **Production Process** – Manufacturing, quality control, and packaging.  
7. **Shipment (DESADV)** – Dispatch advice sent via EDI after shipping.  
8. **Invoicing (INVOIC)** – Sales invoice generated and sent to the customer.  

---

## 💬 EDI Messages Involved
| Direction | EDI Message | Description |
|------------|--------------|--------------|
| Customer → ERP | DELFOR | Forecast schedule |
| Customer → ERP | DELJIT | Delivery schedule (call-off) |
| Customer → ERP | ORDERS | Sales order |
| ERP → Customer | ORDRSP | Order confirmation |
| ERP → Customer | DESADV | Dispatch advice |
| ERP → Customer | INVOIC | Invoice |

---

## 🧰 Tools & Technology
- Modeled in **ADONIS BPM**
- Exported to **BPMN 2.0 (XML + PNG)**
- Viewable in **Bizagi**, **Camunda Modeler**, or **Signavio**

---

## 🖼 Diagram Preview
![BPMN Automotive Order-to-Invoice Process](diagrams/automotive-production-workflow.png)

---

## 🧩 Context
The model represents a **typical automotive ERP process**, where customer EDI messages drive production and logistics.  
While the diagram could reflect processes executed in systems like **ERP Panthera**, it is **system-agnostic**,  
focusing on the universal business logic of EDI-based manufacturing and order handling.

---

## 📜 License
Released under the **MIT License** — free for learning and documentation purposes.

---

### 👩‍💻 Author
**Sandra Rog**  
Business Process & ERP Analyst | BPMN | EDI | Automotive ERP Systems
