# Frontend Developer Hiring Test

Welcome! This is a technical assessment for candidates applying to join our team as a **Frontend Developer**. It helps us understand how you think, structure your components, and build clean, functional user interfaces.

---

## 👨‍💻 About the Role

We’re building a small, remote team working on projects in the **fitness and sports-tech industry**. This is a **frontend role** where you’ll focus on building high-quality components using **ReactJS and TailwindCSS**, with NextJS for routing.

- This is a **remote contractor position**
- You’ll collaborate with a technical lead and other remote team members
- You manage your own hours, tools, and taxes
- We work async and expect clarity, ownership, and results

---

## 💰 Compensation

- **AUD $1,400 per month for full-time**, as a contractor  
- Part-time options available based on skills and availability

---

## ✅ What You Need To Do

1. Complete the coding task below  
2. Push your work to your **own GitHub repository**  
3. In the **root folder** of your repo, add a Markdown file with your CV:  
   `cv_{your-full-name}.md`  
4. Submit your application using this form:  
   👉 https://forms.gle/3TpyZ8uHP3L9Nyq4A

> Make sure your repo is set to public

---

## 🎯 Task: Workout Renderer Component

Using the JSON file below as input, build a **React + TailwindCSS component** that displays the workout in the **clearest, most user-friendly way**.

The JSON represents a simple running session with three segments:

**Warmup**  
5min at Z1, followed by 5min fartlek

**Main set**  
8 sets of 1min at high intensity followed by 30 sec rest before the next set

**Cool down**  
5min easy jog to recover

Your goal is to take this structure and display it in a clean and understandable format for users.

**What we're evaluating:**

- Your ability to interpret structured workout data
- Visual clarity and layout
- Reusable component structure
- How well the final result communicates the training intent

**Use this JSON as your input:**

```json
{
  "_id": "fetest",
  "name": "Running Test",
  "description": "Quick 10min warmup followed by 8 sets of 1min at high intensity and 30 sec rest between each intense interval. You then recover with a 5min easy jog.",
  "discipline": "running",
  "duration": {
    "value": 35,
    "unit": "min"
  },
  "segments": [
    {
      "title": "Warmup",
      "blocks": [
        {
          "type": "duration_interval",
          "id": "B1",
          "duration": {
            "value": 5,
            "unit": "min"
          },
          "intensity": "easy",
          "note": "don't start too hard",
          "render": "5min easy jog"
        },
        {
          "type": "duration_interval",
          "id": "B2",
          "duration": {
            "value": 5,
            "unit": "min"
          },
          "intensity": "fartlek",
          "note": "fartlek are random accelerations and decelerations at will. The purpose is to get the legs ready for the main set. Don't go too hard.",
          "render": "5min fartlek"
        }
      ]
    },
    {
      "title": "Main set",
      "blocks": [
        {
          "type": "set",
          "id": "B3",
          "reps": 10,
          "render": "10x:",
          "blocks": [
            {
              "type": "duration_interval",
              "id": "B4",
              "duration": {
                "value": 1,
                "unit": "min"
              },
              "intensity": "hard",
              "render": "1min hard"
            },
            {
              "type": "rest",
              "id": "B5",
              "duration": {
                "value": 30,
                "unit": "sec"
              },
              "intensity": "recovery",
              "render": "30sec recovery"
            }
          ]
        }
      ]
    },
    {
      "title": "Cool down",
      "blocks": [
        {
          "type": "duration_interval",
          "id": "B6",
          "duration": {
            "value": 5,
            "unit": "min"
          },
          "intensity": "easy",
          "render": "5min easy jog"
        }
      ]
    }
  ]
}
```

---

## 📁 Documentation

In your repository, include:

1. **README.md** – Brief explanation of your approach  
2. **cv_{your-full-name}.md** – Your CV in markdown format  
3. **Comments in code** – Short and useful, where it helps

If you make any assumptions, document them clearly in your `README.md`.

---

## 🧠 What We’re Really Looking For

- Clean component structure and naming  
- Thoughtful use of React and TailwindCSS  
- Basic design sensibility and UX thinking  
- Clear, proactive communication  
- Independent work mindset and consistency

We care more about clarity and usability than complex tricks or pixel-perfect visuals.

---

## 📩 Final Step

Once you're done, make sure your GitHub repo includes:
- Your completed component
- Your `cv_{your-full-name}.md` file
- A brief `README.md` with your notes and explanations

Then submit your repo through this form:  
👉 https://forms.gle/3TpyZ8uHP3L9Nyq4A

If you run into issues or have constraints, mention it in the form.

---

**Good luck. We're looking forward to seeing how you work.**
