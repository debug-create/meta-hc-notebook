# 🏎️ ☀️ Racing with the Sun: How we built an AI Brain for Solar EVs

Imagine you're in the middle of a desert, driving a car powered entirely by sunlight. There’s no gas station for 500 miles. Suddenly, a massive cloud blocks the sun, and the road starts climbing a steep 6% grade. 

**What do you do?**
- Speed up to clear the hill before the battery dies? 
- Slow down to save energy and hope you don't stall? 
- Crank the cooling system so the battery doesn't melt in the 40°C heat?

Most humans would guess. We built an AI that **knows.**

---

## 🧠 The Project: Solar EV PMU Strategist

We built a **Power Management Unit (PMU) Strategist**. It’s an AI brain that sits inside a Solar Electric Vehicle and makes split-second decisions about speed, energy routing, and cooling. 

It doesn't just "drive"; it **strategizes.** It looks at the track 3 segments ahead, checks the weather forecast, and balances physics-based constraints to win the race without breaking the car.

---

## 🛠️ How it Works (The "Secret Sauce")

We used a technique called **Policy Distillation**. 
1. **The Simulator**: We built a high-fidelity physics environment (using the **OpenEnv** framework) that simulates everything from air resistance to solar panel efficiency.
2. **The Teacher**: We created an expert "Heuristic" policy that knows the math of the track perfectly.
3. **The Student**: We took a cutting-edge Language Model (**Qwen2.5-1.5B**) and taught it to think like the expert.

By using **Supervised Fine-Tuning (SFT)**, we reduced the AI's "error rate" (loss) by **99%**! It went from being a confused chatbot to a world-class racing strategist.

---

## 📊 The Proof is in the Data

Our AI didn't just learn to follow instructions; it mastered the hardest tasks we could throw at it.

- **Night Runs**: Navigating 25km with **ZERO** solar power by managing the battery like a pro.
- **Thermal Races**: Blasting through heatwaves while keeping the battery temperature stable.
- **Dynamic Routing**: Adjusting speed in real-time as clouds and hills change the energy budget.

![Improvement Chart](improvement_chart.png)
*(The 99% Loss Reduction Curve)*

---

## 🚀 Why This Matters

This isn't just about winning a hackathon. This is about the future of **Sustainable Transportation.** 

As we move toward a world powered by renewable energy, we need AI that understands the "rhythm" of the environment—when to save, when to spend, and how to stay safe. Our PMU Strategist is a proof-of-concept for a world where our cars are as smart as the grid they run on.

---

## 🔗 Try it Yourself!

Check out our live environment and see the AI in action:
👉 **[Live Demo on Hugging Face](https://debug180906-solar-ev-env.hf.space)**

Built with ❤️ for the Advanced Agentic Coding Hackathon. 
**If you like the project, give us a ⭐ on GitHub!**
