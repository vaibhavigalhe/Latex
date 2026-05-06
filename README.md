**Practical 10: Neural Style Transfer**

Objective:
To generate an image that combines the content of one image with the style of another image.

Concept:
Neural Style Transfer is based on Convolutional Neural Networks (CNNs).
A pretrained network (commonly VGG19) is used to extract:

Content features (object structure)
Style features (textures, colors)

Real Technique Used:

CNN feature extraction
Gram Matrix for style representation
Optimization using gradient descent

Explanation:
In real implementation, both content and style images are passed through a deep CNN.
The network extracts feature maps from different layers.

Content loss is calculated by comparing feature maps of the generated image with the content image.
Style loss is calculated using Gram matrices, which capture texture information from the style image.

An initial image (random or content image) is iteratively updated using gradient descent to minimize:

Content loss
Style loss

The final output preserves the structure of the content image while applying the style patterns.

In this program, the same idea is demonstrated in a simplified way using image blending.
Both images are resized and combined using a fixed ratio to simulate mixing of content and style.

The images are displayed side by side, and the final output is saved.

Result:
A new image that visually combines structure and appearance.

Conclusion:
Neural Style Transfer uses deep learning and optimization to merge content and style features.



**Practical 3: Fuzzy Set Operations and Relations**

Objective:
To perform fuzzy set operations and apply fuzzy relations with max-min composition.

Concept:
Fuzzy logic handles uncertainty using values between 0 and 1 instead of binary values.

Real Techniques Used:

Min–Max operators
Cartesian product for relations
Max–Min composition for reasoning

Explanation:
Fuzzy sets are defined with membership values representing the degree of belonging.

Union is computed using the maximum operator, representing the highest degree of membership.
Intersection uses the minimum operator, representing common membership.
Complement is calculated as (1 − value), indicating inverse membership.
Difference is computed using minimum of A and complement of B.

Fuzzy relations are formed using the Cartesian product.
Each element in one set is compared with elements of another set using the minimum operator.
This produces a matrix representing relationships between elements.

Max-min composition is used to combine two fuzzy relations.
For each pair, minimum values are calculated and the maximum among them is selected.
This method is widely used in fuzzy inference systems to propagate uncertainty.

Result:
Fuzzy operations and relations are computed and displayed in matrix form.

Conclusion:
Fuzzy logic provides a mathematical framework for reasoning under uncertainty using min-max operations.

**Practical 4: Load Balancing**

Objective:
To simulate distribution of client requests across multiple servers.

Concept:
Load balancing improves system performance by distributing workload efficiently.

Real Techniques Used:

Round Robin Scheduling
Least Load (Greedy algorithm)

Explanation:
A set of servers is initialized, each representing available resources.
Incoming requests simulate tasks from clients.

In the Round Robin algorithm, requests are assigned sequentially to servers in a cyclic manner.
This ensures equal distribution but does not consider current load.

In the Least Load algorithm, each request is assigned to the server with the minimum current load.
This is a greedy approach that dynamically balances workload.

After assigning each request, the load of the selected server is updated.
This ensures that future decisions consider current system state.

These techniques are commonly used in real distributed systems, web servers, and cloud platforms.

Result:
Requests are distributed across servers, and final load is displayed.

Conclusion:
Load balancing algorithms ensure efficient resource utilization and improve system reliability.

**Final Quick Viva Lines**

Neural Style Transfer:
“Uses CNN feature extraction and optimization to combine content and style.”

Fuzzy Logic:
“Uses min-max operations and max-min composition for reasoning under uncertainty.”

Load Balancing:
“Uses round robin and least load algorithms to distribute workload efficiently.”
