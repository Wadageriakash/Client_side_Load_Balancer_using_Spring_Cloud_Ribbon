* Round Robin: Distributes requests sequentially to each server in a rotating manner. Simple and good for evenly distributed loads when all instances have similar capacity.
* Weighted Round Robin: Assigns weights to instances based on their capacity (e.g., a more powerful server gets a higher weight and more requests). Useful in heterogeneous environments.
* Least Connections: Directs traffic to the server with the fewest active connections. Good for services with varying request processing times.
* Least Response Time (or Least Time): Sends requests to the server with the fastest response time and fewest active connections. Prioritizes efficiency and responsiveness.
* IP Hash: Uses the client's IP address to determine which server handles the request. This ensures that a specific client consistently communicates with the same service instance, useful for session persistence.
* Random: Selects a random instance for each request. Simple but less effective for even distribution.
