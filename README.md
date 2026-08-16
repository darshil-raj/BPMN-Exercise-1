# BPMN-Exercise-1

This repository contains BPMN models created in Camunda Modeler for three business-process scenarios. Each model uses basic BPMN elements such as Start Events, Tasks, Exclusive Gateways, Sequence Flows, and End Events.

## Files

| File | Scenario |
|---|---|
| `Employee Leave Portal.bpmn` | Employee Leave Approval |
| `Online Purchase Order Processing.bpmn` | Online Purchase Order Processing |
| `IT Service Request.bpmn` | IT Service Request |

## BPMN Elements Used

- **Start Event:** Shows where a process begins.
- **Task:** Represents an activity performed by a person or system.
- **Exclusive Gateway:** Represents a decision where only one path is selected, such as Yes/No.
- **Sequence Flow:** Arrows showing the order of activities.
- **End Event:** Shows where a process finishes.

---

## Scenario 1: Employee Leave Approval

The process starts when an employee submits a leave request. The HR system checks the employee’s leave balance using an exclusive gateway.

- If the balance is insufficient, the system sends an insufficient-balance notification and the process ends.
- If sufficient leave is available, the request is sent to the manager for approval.
- If the manager approves, the system updates the employee’s leave balance and sends an approval notification.
- If the manager rejects, the system sends a rejection notification.
- The process ends after the appropriate notification is sent.

---

## Scenario 2: Online Purchase Order Processing

The process starts when a customer places an online order. The system checks whether the product is available.

- If the product is out of stock, the customer receives an out-of-stock notification and the process ends.
- If the product is available, the system processes the payment.
- If payment fails, the customer receives a payment-failure notification and the process ends.
- If payment is successful, the system confirms the order, prepares the product for shipment, and ships the order.
- Finally, the customer receives a shipping confirmation and the process ends.

---

## Scenario 3: IT Service Request

The process starts when an employee submits an IT support request. The IT help desk registers the request and checks the severity of the problem.

- If the problem has low severity, it is assigned to a support technician.
- If the problem has high severity, it is assigned to a senior technician.
- The technician investigates the problem.
- If the problem can be resolved internally, the technician fixes the problem.
- If it cannot be resolved internally, the problem is escalated to an external service provider.
- After resolution, the help desk updates the request status and sends a resolution notification to the employee.
- The process then ends.

## Tool Used

All BPMN diagrams were created using **Camunda Modeler**.
