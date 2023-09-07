Task 2: Microservices Architecture and Deployment

1. Begin by acquainting yourself with the core projects and their purposes:
a. Saleor API: Explore the functionalities at https://github.com/saleor/saleor .
b. Saleor storefront: Understand the frontend mechanics at https://github.com/saleor/react-storefront .
c. Saleor dashboard: Dive into the dashboard intricacies at https://github.com/saleor/saleor-dashboard .
d. Saleor platform: Access the repository at https://github.com/saleor/saleorplatform , which contains essential Docker Compose elements for configuring, building, and executing Saleor components. Note that this repository references the three aforementioned repos using Git submodules.

2. Create a personal account on Github.com and proceed to fork the Saleor platform
repository.
![0cf16acaa586660d2f1d8a6b3cd56fb](https://github.com/MilloooSy/saleor-platform/assets/143394742/3b0abfb1-803a-4242-b1f6-7e179b8ad9cf)

3. Follow the step-by-step guidelines outlined in the Saleor platform repository to
effectively run a Saleor stack enriched with sample data.
![12bc7534c5b78a662695989167c887d](https://github.com/MilloooSy/saleor-platform/assets/143394742/8a5c4a95-8891-4db0-8e7c-10d4e0892e50)

![f07921ae82b86d196fdd54ca79aff14](https://github.com/MilloooSy/saleor-platform/assets/143394742/b53a19ba-4b52-48f1-b0ae-c595fbeb867c)

![19a1dc2eace62efbba765c85817e2a9](https://github.com/MilloooSy/saleor-platform/assets/143394742/823adc89-97e5-4043-b810-3ef7680de4f2)

![696dd68abc19bcb1c63b8cc8db151bb](https://github.com/MilloooSy/saleor-platform/assets/143394742/21059992-4567-4a93-b79f-12fd4a98bc98)

![8c2d41924fc2003040d546ce6da97a5](https://github.com/MilloooSy/saleor-platform/assets/143394742/e51ee898-da02-4599-a753-54d4fb7fd468)

![8882bf94341c82c5cddd5327e14b2a6](https://github.com/MilloooSy/saleor-platform/assets/143394742/2c694279-59e1-4b3b-8806-ef393991bda3)

![5825ccb1e2c640bd406e6e3a4bef7a0](https://github.com/MilloooSy/saleor-platform/assets/143394742/2d41e8a3-cbdf-4ba6-b240-b088f3bbb53d)

I also deploy the saleor-platform at GKE, and I have reference the pic below
![99af8790ac37878a7fb354b9f8121eb](https://github.com/MilloooSy/saleor-platform/assets/143394742/93978aed-8629-4857-9930-0c635d529837)

4. Tailor the Compose file to ensure optimal functionality:
a. Configure the React Storefront to operate on port 3009.
![0b3259f8e943aaf6d8962088c911f2e](https://github.com/MilloooSy/saleor-platform/assets/143394742/95adfd13-2841-4de0-aa8e-4b951109b4cb)
Due to the origin saleor-platform has removed react storefront, I have changed the port of API into 3009.

b. Assign port 9003 for the Saleor Dashboard.
![b29cd5e0a34ad31215f26d2c690b622](https://github.com/MilloooSy/saleor-platform/assets/143394742/30526e2a-66d2-4860-9a74-8f2d266e6e05)


c. Initiate the stack and verify the successful launch of all services:
o Saleor React Storefront: Accessible at http://<Your-Linux-Server-IP>:3009.
![a6e6688dbcefd73b57eea726f8929b2](https://github.com/MilloooSy/saleor-platform/assets/143394742/0a4399dc-f734-4f37-8f9a-7579f7931295)
I try to access it within using GKE

![7a231dd5dae043d52a50598e9372678](https://github.com/MilloooSy/saleor-platform/assets/143394742/7f3c672b-0de3-45d0-90e5-97f1cbe0ead4)
But it seems some error within using GKE access it. It is a security measure of Django frame, to make sure there is only specific host can via the website

![5825ccb1e2c640bd406e6e3a4bef7a0](https://github.com/MilloooSy/saleor-platform/assets/143394742/5a4a6970-5c79-40dd-be18-74f5b6289a22)
I turn to localhost for trying it

![aea047b0960f50caed04f8a1090b9af](https://github.com/MilloooSy/saleor-platform/assets/143394742/dd1d384e-34ca-47f5-9032-d6d1489f982c)
It works

o Saleor Dashboard: Reachable via http://<Your-Linux-Server-IP>:9003.
![b3208dc5f675e8dc94927f27caad6e0](https://github.com/MilloooSy/saleor-platform/assets/143394742/31aa4c4d-d97a-47b4-b8d3-cc72f190008b)
Dashboard works in the local environment as well, so I decide to try it at GKE

![2c8c4d3f06c17aea581c737a8681a2e](https://github.com/MilloooSy/saleor-platform/assets/143394742/1cd0a9b7-4941-4724-a70b-873fa2a8156c)
Dashboard can be reachable in GKE

5. Commit your modifications and push them to the forked repository, appending the
tag isec6000-assignment1.
![ff92ef2e574c02352de33e34ae2ca20](https://github.com/MilloooSy/saleor-platform/assets/143394742/b17bbf2a-eb80-4b12-ac45-960cd33989f3)

![f01ac748f5181de422f2181d4b0e8e6](https://github.com/MilloooSy/saleor-platform/assets/143394742/b02de21b-2ff4-4c39-af0f-8df9aae360e2)
This for tag

![b6a5fc3bf1c10029cd3264e68c93138](https://github.com/MilloooSy/saleor-platform/assets/143394742/5e062103-abef-4216-98f6-32284c9b17c5)
Push tag to the github

![2e41421e3c20461856fdbbfe2535696](https://github.com/MilloooSy/saleor-platform/assets/143394742/8bd3975e-5690-46c2-9b56-634f27781893)
Push all changes to the github
