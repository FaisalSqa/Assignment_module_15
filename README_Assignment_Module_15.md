# Assignment Module 15

This repository contains automated test solutions for Assignment Module 15. It includes UI automation with Playwright and API automation with Postman and Newman.

## Project Overview

### UI Automation
Solved using Playwright for the following test cases:

**Q1 [Mark 10]**  
Try logging in with `locked_out_user` and verify the error message.

**Q2 [Mark 20]**  
Log in with `standard_user`. Then, from the hamburger menu, reset the App State. Add any three items to the cart. Navigate to the final checkout page and verify the product name and total price. Finish the purchase journey and verify the successful order message. Then, reset the App State again and log out.

**Q3 [Mark 10]**  
Log in with `performance_glitch_user` and reset the App State. Then filter by name (Z to A) and select the first product into the cart. Then navigate up to the final checkout page and verify all the products' names and the total price. Then finish the purchase journey and verify the successful order message. Then, reset the App State again and log out.

### API Automation
Solved using Postman and Newman for the following test cases:

**Q3 [Mark 10]**  
Login with registered credentials and capture `authToken`.

**Q4 [Mark 10]**  
GET user by `userId` and verify name and email match.

**Q5 [Mark 10]**  
PUT updated profile and verify the `updatedAt` timestamp.

**Q6 [Mark 10]**  
PATCH a single field and verify only that field changed.

**Q8 [Mark 20]**  
Execute bad requests using stored data and assert 4xx errors.

## Tech Stack

- Playwright
- Postman
- Newman
- Node.js

## Folder Structure

```bash
Q1_Q2_Q3/
```

## How to Run Playwright Tests

First go to the `Q1_Q2_Q3` folder:

```bash
cd Q1_Q2_Q3
```

Run Q1:

```bash
npm run q1
```

Run Q2:

```bash
npm run q2
```

Run Q3:

```bash
npm run q3
```

Run all tests together:

```bash
npm run all
```

After running any test, open the HTML report to view the result.

## How to Run Postman Collection with Newman (you must be in the Assignment_module_15 folder)

Run the collection using this command:

```bash
newman run "Assignment module 15.postman_collection.json"
```

