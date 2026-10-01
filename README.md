# Auto Ticket Classification using Flow Designer

## Project Title
Auto Ticket Classification using Flow Designer

## Problem Statement
The school IT helpdesk receives multiple incidents daily from students and teachers, such as Wi-Fi issues, projector problems, password issues, and slow computers. Manually reviewing and categorizing each ticket takes time and effort.

This project automates ticket classification using ServiceNow Flow Designer based on keywords in the short description and description.

## Objective
- Automatically classify incidents when they are created.
- Reduce manual effort in ticket classification.
- Improve ticket routing efficiency.
- Use a no-code and maintainable solution.

## Technology Used
- ServiceNow
- Flow Designer
- Custom Tables
- Update Sets
- Email Notifications

## Key Features
- Automatic ticket classification
- Category and subcategory assignment
- Dependent choice logic
- Email notification to the caller
- Structured ticket storage
- Maintainable and scalable workflow

## Ticket Classification

| Keywords / Issue | Category | Subcategory |
|---|---|---|
| WiFi / Network | Network | Wi-Fi |
| Projector | Hardware | Projector |
| Password / Login / Forgot Password | Access | Forgot Password |
| Slow / Hanging / Slow Computer | Performance | Slow Computer |

## Modules
1. Custom Incident Workflow Table
2. Category and Subcategory Configuration
3. Flow Designer Automation
4. Ticket Classification
5. Email Notification
6. Testing and Deployment

## Database / Table Fields

- Number – Auto Number
- Caller – Reference to sys_user
- Category – Choice
- Subcategory – Choice
- Short Description – String
- Description – String
- State – Choice
- Assigned Group – Reference to sys_user_group
- Assigned To – Reference to sys_user

## Automation Workflow

1. A new incident is created.
2. Flow Designer detects the newly created record.
3. The system checks the ticket description.
4. Keywords are identified.
5. Category and subcategory are automatically assigned.
6. An email confirmation is sent to the caller.

## Testing

### Test Case 1
**Input:** WiFi not working in library

**Expected Result:**
- Category: Network
- Subcategory: Wi-Fi
- Email notification sent to caller

### Test Case 2
**Input:** Projector not turning on

**Expected Result:**
- Category: Hardware
- Subcategory: Projector
- Email notification sent to caller

## Expected Outcome
The system automatically classifies school IT helpdesk tickets, reduces manual work, and improves ticket handling efficiency.

## Conclusion
The project provides an end-to-end automation solution for a school IT helpdesk using ServiceNow Flow Designer. It reduces manual classification effort and improves response efficiency. The solution can also be extended with assignment automation, SLA tracking, and predictive intelligence.
