# Automated-Network-Request-Management

Network Request Management is a ServiceNow-based application designed to simplify and automate the process of submitting, approving, and managing network-related service requests.

The system allows users to submit network requests through the Service Catalog, collects the required information, routes the request for approval, creates a corresponding database record, and sends email notifications throughout the process.

---

## Objectives

- Provide a structured way to submit network service requests.
- Collect requester and network-related information through catalog variables.
- Automate request processing using Flow Designer.
- Implement an approval process.
- Store request information in a custom database table.
- Send notifications to users about request status.
- Provide a centralized workflow for the Network team.

---

## Features

- Service Catalog based Network Request
- Requester Information collection
- New / Existing connection selection
- Existing Connection ID handling
- Network request details collection
- Mode of Payment selection
- Total Amount field
- Catalog UI Policies
- Conditional field visibility
- Flow Designer automation
- Approval workflow
- Custom Network Database Table
- Email notifications
- Request tracking

---

##  Workflow

1. User opens the **Service Catalog**.
2. User navigates to **Office → Services**.
3. User selects **Network Request**.
4. User enters requester and network details.
5. User selects the type of connection:
   - New
   - Existing
6. Required fields are displayed based on the user's selection.
7. User submits the request.
8. ServiceNow creates a request number.
9. Flow Designer processes the request.
10. The request is sent for approval.
11. After approval, the request information is stored in the Network Database Table.
12. Email notifications are sent to the relevant users.

---

## ServiceNow Components

### Service Catalog

The project contains a **Network Request** Catalog Item under:

`Service Catalog → Office → Services → Network Request`

### Catalog Variables

Some of the variables used include:

- User Name
- Email ID
- Phone Number
- Opened on Behalf of
- Address
- Type Of Connection
- Enter your Existing ID
- Mode of Payment
- Total Amount

### Question Choices

**Type Of Connection**
- New
- Existing

**Mode of Payment**
- UPI
- Card

---

## Flow Designer

The **Network Request** flow automates the request processing.

The flow includes steps such as:

- Getting Catalog Variables
- Creating a Network Database Table record
- Request approval
- Updating approval status
- Processing the submitted request

---

##  Custom Database Table

A custom **Network Database Table** is used to store the information associated with network requests.

The table stores information such as:

- Database Number
- Request Number
- Requested For
- Work Status
- Assignment Group
- Assigned To
- Device Details
- Customer Address
- Special Instructions

---

## Notifications

Email notifications are configured to keep users informed about their network requests.

Example:

- Request creation notification
- Approval/request status notification

---

##  Technologies Used

- ServiceNow
- Service Catalog
- Flow Designer
- Custom Tables
- Catalog Variables
- Catalog UI Policies
- Approvals
- Email Notifications
- Update Sets

---

