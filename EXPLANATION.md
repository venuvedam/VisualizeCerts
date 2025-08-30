# What is VisualizeCerts?
- VisualizeCerts is a small but useful project that focuses on one simple idea: making your certification progress easier to see. If you’ve ever tried to track which Microsoft exams you’ve passed, which certifications you hold, or which Credly badges you’ve earned, you know it can get messy. Different platforms show information in different ways, and it’s not always clear how everything connects. This repository pulls those details together and gives you a visual way to explore them.

## The Goal
- The main goal is to fix the problem of information that is spread out. Microsoft certifications often build on each other, so students need to know what they already have and what they might need to learn next. VisualizeCerts makes a map of your journey by pulling in your current exams, credentials, and badges. The value is clear: you can quickly see where you are and what you should do next. This tool saves you time and confusion, whether you're just starting out and trying to figure out the Microsoft certification paths or you're an experienced professional planning your next move.

## How It Works
- Three main sources of data are used in the project:
* Badges from your Credly account
* Passed tests from Microsoft
* MS Learn certificates

- Scripts in the repo get this data and get it ready to be shown. For instance, the fetch_* scripts are in charge of getting the data and cleaning it. When the data is ready, it is put together into one dataset that you can explore in real time. Plotly is what makes the visualization work.
a well-known Python library for graphing that lets you show connections and paths in a clear, interactive way.

- A few important files to keep in mind:
* `ai_exam_recommender.py` – a tool that helps you think of possible exams you might take next.

* `fetch_*` scripts are used to get your certification data and process it.

* `index.html` – the interactive visualization you can open locally in your browser.

## How to Use VisualizeCerts
- Usage is easy at a high level. You run the fetch scripts to get your certification data after you clone the repository. After that, you can see the visualization by opening index.html in your browser. You don't need a complicated setup or environment; the goal is to make it easy for both developers and learners to use. The `README.md` file has all the information you need to set it up.

## Current Status
- This project is still changing. At this point, it assumes that you can get to your Credly data and give it the information it needs. The visualizations are mostly about Microsoft certifications, but the method could be used for other things in the future. Some of the problems are that it relies on outside APIs and that the formatting might be different depending on where you are. These are known trade-offs, and any help you can give to make the tool more flexible and easy to use is welcome.

## How You Can Help
- If you’re a developer, you could contribute to the enhancement of the fetch scripts or include support for additional data sources. Just using the tool and giving feedback is a great way to help if you're a learner. Information about setup, usage, and contributing guidelines can be found in the README.

- In short, VisualizeCerts creates an interactive, well-organized view of your learning progress from dispersed certification data. We encourage all types of contributions to improve it, including code, ideas, and feedback.
