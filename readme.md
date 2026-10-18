# [DOA Estimation] University of Electronic Science and Technology degree thesis: Analysis of Approximately Increasing Multi-signal Classification Doppler Radar Performance [with MATLAB Code]

I. Research Background and Significance of Doppler Direction Estimation (DOA) is one of the core research directions in array signal processing, and has important applications in radar, communication, sonar, and other fields. The Multiple Signal Classification (MUSIC) algorithm, proposed in 1979, has become a classic method for direction finding in space spectrum estimation due to its good balance between precision and computational complexity. However, the MUSIC algorithm has a clear threshold effect, and its performance will drop sharply when the signal-to-noise ratio or the number of fast sweeps is below the critical value.
To overcome this limitation, the Universal Multi-Signal Classification Algorithm (g-MUSIC) based on Random Matrix Theory (RMT) and g-estimation theory emerged. This algorithm not only optimizes performance but also adapts to complex application scenarios such as large antenna arrays. It particularly demonstrates significant advantages in scenarios with small signal intervals and low sample volumes, where resolution and accuracy are prominent. This paper focuses on the performance characterization of both algorithms in the threshold region, delving into the asymptotic random behavior of the cost function, providing theoretical support for algorithm optimization and application.
II. Core Algorithm Principles
Construct the spatial spectrum function, where is the direction vector and is the noise subspace matrix. By searching for the peak position of the spectrum function, the direction of arrival can be estimated. However, the algorithm performs excellently only when the number of fast shots far exceeds the number of elements (), and its estimation accuracy significantly drops when it is comparable in magnitude.
2. The g-MUSIC algorithm, addressing the limitations of the MUSIC algorithm, introduces a weighted processing to optimize the cost function. Its cost function is defined as follows: where weights are obtained by solving the eigenvalue-related equations, achieving an adjustment to the estimation bias of the sample covariance matrix.
The algorithm ensures consistent estimation of the cost function for true values as the number of elements and the number of snapshots approach infinity at the same rate (and), effectively mitigating threshold effects. It performs better in scenarios with low sample sizes and close-spaced sources.

III. Theoretical Analysis: Asymptotic Behavior of the Cost Function
1. Under asymptotically Gaussian distribution and fixed ratio conditions, both algorithms converge to zero mean Gaussian random vectors with their covariance matrices characterizing their fluctuation characteristics. This conclusion is proven through Cramer-Wold theorem and convergence of characteristic functions, providing a theoretical foundation for performance analysis of the algorithms.
2. Asymptotic Equality and Second-Order Behavior
The asymptotic equality of the cost function for MUSIC algorithm relies on the asymptotic behavior of eigenvectors of the sample covariance matrix. By introducing Stieltjes transformation and g-estimation theory, the g-MUSIC algorithm achieves asymptotic equality with real values and has an order of convergence. Second-order asymptotic analysis indicates that the g-MUSIC algorithm has smaller variance under finite sample size and more stable estimation.
IV. Simulation Verification
1. Recognition Probability Comparison
Through Monte Carlo simulations, the recognition capabilities of the two algorithms against nearby sources are compared under different numbers of snapshots, signal-to-noise ratios, and angle differences:
• Number of Snapshots Impact: Recognition probability increases with the number of snapshots. g-MUSIC significantly outperforms MUSIC at low snapshots (e.g., 50% recognition probability requires fewer snapshots by about 30% than MUSIC).
• Signal-to-Noise Ratio Impact: Under high signal-to-noise ratios, the performance of both algorithms converges, but at low signal-to-noise ratios (e.g., 20%-30% improvement in recognition probability), g-MUSIC enhances recognition probability by about 20%-30%.
• Angle Difference Impact: At extremely small angle differences (e.g., MUSIC essentially fails, while g-MUSIC still maintains some recognition probability, demonstrating stronger near-source recognition capability.
2. Mean Square Error Analysis
The mean square error (MSE) decreases with an increase in the number of samples and an improvement in signal-to-noise ratio. In scenarios with small numbers of samples, g-MUSIC's MSE is reduced by more than 50% compared to MUSIC; when the number of samples is sufficiently large (e.g.), the MSE of both algorithms converges, verifying the optimization effect of g-MUSIC under limited sample conditions.
V. Conclusion and Future Prospects
1. Research Conclusion: This paper, through theoretical derivation and simulation verification, clarifies the performance advantage of the g-MUSIC algorithm in the threshold region: its asymptotic joint high-order statistics of the cost function ensures estimation consistency, and weighted processing effectively reduces bias caused by insufficient samples. It achieves better resolution and accuracy in low-speed sampling, low-signal-to-noise ratio, and near-source scenarios.
2. Future Directions
• Algorithm Optimization: Integrate machine learning techniques to further enhance the robustness and real-time performance of the algorithm in complex environments.
• Scenario Expansion: Promote g-MUSIC to scenarios involving non-uniform arrays, unknown source numbers, etc., expanding its application fields.
• Hardware Compatibility: Design dedicated chip architectures to reduce algorithm computational complexity, meeting engineering needs.
• Multi-source Fusion: Merge multi-sensor data to improve DOA estimation performance in complex electromagnetic environments.
Through a deep analysis of the MUSIC and g-MUSIC algorithms, this paper provides a theoretical reference for the development of direction finding technology and offers important basis for algorithm selection and optimization in practical engineering applications.
End

## Images

![[DOA Estimation] University of Electronic Science and Technology degree thesis: Analysis of Approximately Increasing Multi-signal Classification Doppler Radar Behavior [with MATLAB code attached]](01.jpg)
![[DOA Estimation] University of Electronic Science and Technology degree thesis: Analysis of Approximately Increasing Multi-signal Classification Doppler Radar Behavior [with MATLAB code attached]](02.jpg)
![[DOA Estimation] University of Electronic Science and Technology degree thesis: Analysis of Approximately Increasing Multi-signal Classification Doppler Radar Behavior [with MATLAB code attached]](03.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
