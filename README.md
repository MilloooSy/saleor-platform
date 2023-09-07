Task 2: Microservices Architecture and Deployment
1. Begin by acquainting yourself with the core projects and their purposes:
a. Saleor API: Explore the functionalities at https://github.com/saleor/saleor .
b. Saleor storefront: Understand the frontend mechanics at
https://github.com/saleor/react-storefront .
c. Saleor dashboard: Dive into the dashboard intricacies at
https://github.com/saleor/saleor-dashboard .
d. Saleor platform: Access the repository at https://github.com/saleor/saleorplatform , which contains essential Docker Compose elements for configuring,
building, and executing Saleor components. Note that this repository references
the three aforementioned repos using Git submodules.

2. Create a personal account on Github.com and proceed to fork the Saleor platform
repository.
3. Follow the step-by-step guidelines outlined in the Saleor platform repository to
effectively run a Saleor stack enriched with sample data.
4. Tailor the Compose file to ensure optimal functionality:
a. Configure the React Storefront to operate on port 3009.
b. Assign port 9003 for the Saleor Dashboard.
c. Initiate the stack and verify the successful launch of all services:
o Saleor React Storefront: Accessible at http://<Your-Linux-Server-IP>:3009.
o Saleor Dashboard: Reachable via http://<Your-Linux-Server-IP>:9003.
5. Commit your modifications and push them to the forked repository, appending the
tag isec6000-assignment1.
