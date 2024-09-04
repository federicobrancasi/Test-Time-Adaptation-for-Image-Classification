# Test-Time-Adaptation-for-Image-Classification

Deep neural networks have revolutionized the field of computer vision, achieving unprecedented performance in tasks such as image classification, object detection, and anomaly detection. However, these models face a significant challenge, called **domain shift**: this phenomenon occurs when a model encounters test data that differs substantially from the training data's distribution, leading to severe performance degradation.

Domain shift can arise in various ways:
- Changes in image style or quality
- Variations in lighting conditions or backgrounds
- Differences in object appearances or contexts

These shifts are common in real-world applications, where deployment environments often differ from controlled training scenarios.

To address this challenge, we explore the concept of **Test-Time Adaptation** (TTA). TTA is an innovative approach aimed to enhance the robustness of pre-trained neural networks for image classification when faced with out-of-distribution test data. The key aspects of TTA are:

1. **On-the-fly Adaptation**: TTA adjusts the model's behavior for each test sample individually
2. **No Retraining Required**: Unlike traditional fine-tuning methods, TTA doesn't require access to the original training data or extensive retraining
3. **Preservation of General Knowledge**: The adaptation process maintains the model's broad understanding while specializing for the current input

Recent advancements in Vision-Language Models (VLMs) have demonstrated remarkable zero-shot transfer capabilities. These models can:
- Perform a wide range of downstream tasks without task-specific training
- Utilize natural language prompts to guide their behavior

In the context of TTA, we explore two promising approaches:

1. **Prompt Engineering**: Designing effective prompts that guide the VLM to perform well on new, unseen data distributions
2. **Prompt Learning**: Automatically learning optimal prompts for specific test-time scenarios, potentially outperforming hand-crafted prompts

By combining the power of VLMs with Test-Time Adaptation techniques, we aim to develop more robust and flexible image classification systems capable of maintaining high performance across diverse and challenging real-world scenarios.

Note: the final version of the code has been developed in AWS.
