# PROPHET
PROPHET: An Inferable Future Forecasting Benchmark with Causal Intervened Likelihood Estimation 

*A Benchmark for Evaluating AI Systems in Predicting Real-World Events*  🚀

### **Overview**  

PROPHET is a benchmark designed to evaluate the future forecasting capabilities of AI systems, focusing on **inferability**—ensuring predictions are grounded in sufficient supporting evidence. Unlike existing benchmarks, PROPHET rigorously filters questions using proposed **Causal Intervened Likelihood (CIL)**, a statistical measure that quantifies how news articles support answers.  

<div align="center">
  <img src="https://github.com/TZWwww/PROPHET/blob/main/IMG/overview.png" width="500"/>
</div>

---

### **Key Contributions**  
1. **CIL (Causal Intervened Likelihood)**

   $$CIL_i = P(y=\hat{y}|do(X_i=1)) - P(y=\hat{y}|do(X_i=0))$$
   - A causal inference-based metric to estimate whether a question is answerable using retrieved news articles.
   - Models the impact of "intervening" on news events (e.g., "What if this event did not happen?") to measure their supportiveness to the prediction.  
   - Validated via experiments showing strong correlation with model performance.  

3. **PROPHET Benchmark**  
   - **Inferable Dataset**: inferable (L1) and non-inferable (L2) questions sourced from Metaculus and Manifold platforms.  
   - **Real-World Focus**: Questions span diverse domains (politics, finance, climate) paired with 100+ news articles per question.  
   - **Reproducibility**: Static news retrieval ensures consistent evaluation.
   - **Updating Dataset**: We will keep updating by collecting trending data.

<div align="center">
  <img src="https://github.com/TZWwww/PROPHET/blob/main/IMG/validation.jpg" width="700"/>
</div>

---

### **Usage**  
- First version dataset is available for reproducibility.  
- Ideal for researchers developing RAG systems, causal reasoning models, or forecasting tools.  

---  
We are now addressing the Arxiv issue, the paper is coming soon!!!
