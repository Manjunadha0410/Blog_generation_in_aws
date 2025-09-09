# Blog Generation with AWS Bedrock (Lambda)

This Lambda function generates a blog using **Amazon Bedrock** (Meta Llama2-13b) and saves it to an **S3 bucket**.

---

## How it Works

1. Accepts an event with a `blog_topic`.
2. Calls **Bedrock Runtime** to generate a blog (\~200 words).
3. Saves the output in **S3** under `blog-output/<timestamp>.txt`.
4. Returns a success message.

---
