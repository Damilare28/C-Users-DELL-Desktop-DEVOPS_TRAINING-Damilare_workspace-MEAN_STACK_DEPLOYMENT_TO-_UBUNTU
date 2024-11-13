# Load Balancing

**Load balancing**: is the process of distributing network or application traffic across multiple servers to ensure no single server becomes a bottleneck, which optimizes resource use, minimizes response time, and improves overall service reliability. Load balancers manage incoming requests and distribute them to different servers based on specific algorithms, improving the system's scalability, fault tolerance, and performance.

## Types of Load Balancing

1.  **Network Load Balancing (NLB):**

    - Balances traffic across network resources, such as routers and switches.
    - Used primarily for distributing IP traffic.

2.  **Application Load Balancing (ALB):**

    - Works at the application layer (Layer 7 in the OSI model).
    - Manages HTTP and HTTPS traffic based on application-specific data (like URL paths).

3.  **Global Server Load Balancing (GSLB):**

    - Distributes traffic across data centers in different geographic locations.
    - Improves performance by directing users to the nearest or most responsive data center.

4.  **Hardware vs. Software Load Balancing:**

    - Hardware Load Balancers: Physical devices for high-volume traffic, offering robust but expensive solutions.
    - Software Load Balancers: Software-based solutions deployed on virtual machines or servers, which are flexible, cost-effective, and scalable.

## Techniques of Traffic Load Balancing

1. Round Robin:

   - Distributes requests sequentially across servers.
   - Suitable for systems with similar server capabilities.

2. Least Connections:

   - Routes new requests to the server with the fewest active connections.
   - Effective when server load varies significantly.

3. IP Hash:

   - Uses the client’s IP address to assign a consistent server for requests, helping with session persistence.
   - Ideal for applications requiring a user to connect to the same server consistently.

4. Weighted Load Balancing:

   - Assigns weights to servers based on their capacity or power.
   - Servers with higher weights handle more traffic.

5. Least Response Time:

   - Directs requests to the server with the fastest response time.
   - Ensures users are directed to the most responsive servers.

6. Health Checks:

   - Periodically checks server health and redirects traffic from failed servers to operational ones.
   - Enhances reliability and uptime by avoiding unresponsive servers.

7. Geo-Location Based:

   - Routes requests based on the user’s geographic location.
   - Improves latency by directing users to the nearest data center.
