
# Data Redundancy and Distributed Computing Workshop

This workshop explores the concepts of distributed and decentralized computing, focusing on their differences, applications, and practical implementations. Additionally, it covers the importance of redundancy in e-commerce systems.

## Overview

### Distributed Computing
Distributed computing involves dispersing software system elements across multiple computers to enhance efficiency and performance. It aims to achieve a collective objective by allocating tasks among several computers, often requiring central oversight for functions like job scheduling and resource allocation.

### Decentralized Computing
Decentralized computing extends the distributed model by eliminating central governance. Each node functions independently, with decision-making distributed across nodes. This model is often associated with blockchain technology, where each participant holds a ledger copy for independent transaction validation.

## Practical Exercise: From Local to Decentralized Computation

### Activities

1. **Develop Predictive Models**
   - **Q1:** Create diverse predictive models for a selected dataset (e.g., Iris, Housing Market, Titanic). Each group member should develop a distinct model.
   - Evaluate the accuracy and performance of your model.
   - Adapt your model for API access, including a `GET /predict` route that accepts model arguments and returns a prediction.
   - Determine a standardized API response format within your group.

2. **Generate Consensus Prediction**
   - **Q2:** Aggregate predictions from the group's models using tools like ngrok for inter-computer connectivity. Assess the performance of this meta-model.

3. **Introduce Weighting System**
   - **Q3:** Implement a weighting system to refine the meta-model's predictions based on individual model accuracy.

4. **Implement Proof-of-Stake with Slashing**
   - **Q4:** Develop a proof-of-stake consensus mechanism with a slashing protocol. Models must make an initial deposit to participate, with penalties for actions undermining network accuracy.
   - Track model balances using a JSON database.

## E-commerce: Importance of Redundancy

### Objectives
Understand the principles of service and data redundancy, their importance in system reliability, and data integrity.

### Exercises

1. **Simple Hello World Server**
   - **Q1:** Create a simple "Hello, World!" server.
   - **Q2:** Create a DNS registry using an Express server with a `GET /getServer` route that returns the server URL.

2. **Simple E-commerce API**
   - Implement the following routes for product and order management:
     - **Products Routes:** `GET /products`, `GET /products/:id`, `POST /products`, `PUT /products/:id`, `DELETE /products/:id`
     - **Orders Routes:** `POST /orders`, `GET /orders/:userId`
     - **Cart Routes:** `POST /cart/:userId`, `GET /cart/:userId`, `DELETE /cart/:userId/item/:productId`

3. **Database Implementation**
   - **Q3:** Create a database to store various fields using a JSON-based DB, SQL, PostgreSQL, MongoDB, etc.
   - **Q4:** Modify the server implementation to match API requirements.
   - **Q5:** Create a simple front-end to interact with the server.
   - **Q6:** Simulate an API server issue and fix it.

4. **Redundancy Implementation**
   - **Q7:** Implement synchronous mirroring to ensure real-time data availability.
   - **Q8:** Implement asynchronous replication for periodic data copying to a secondary location.
   - **Q7-bis:** Implement synchronous mirroring using two different database structures.
   - **Q8-bis:** Implement asynchronous replication using two different database structures.

## General Considerations

- **Validation and Error Handling:** Implement validation for all inputs and provide meaningful error messages.
- **Data Format:** All responses should be in JSON format.
- **Statelessness:** Ensure the API is stateless for easy scaling and reliability.

## Hints

- Consider the impact of server or database failures on e-commerce operations.
- Explore synchronous mirroring and asynchronous replication to enhance data redundancy and system reliability.
