# GMIL CM Benchmark - Math Reasoning as an 11-Year-Old

This repository contains the dataset, benchmark results, and analysis from the blog post [**"How AI Models Stack Up Against My 11-Year-Old?"**](https://blog.michalprzadka.com/posts/gmil-benchmark/). The benchmark evaluates the mathematical reasoning capabilities of advanced AI models using puzzles from the [**GMIL 2025** competition](https://gmil.pwr.edu.pl/) (Category CM).

## Benchmark Overview

The benchmark compares the performance of several AI models against human performance (my 11-year-old daughter, Anika) on 8 math puzzles. Models tested:

- **GPT-4o**  
- **GPT-o3-mini**  
- **DeepSeek-R1**  
- **Sonnet-3.5**  
- **Gemini-Flash**  

Read more about the methodology and results in the [blog post](https://blog.michalprzadka.com/posts/gmil-benchmark/).

## Repository Structure

```
gmil-cm-benchmark/
├── README.md
├── data/
│   ├── gmil_cm_puzzles_2025.csv
│   └── gmil_cm_solutions_2025.csv
├── notebooks/
│   └── benchmark_analysis.ipynb
└── transcripts/
    ├── gpt-4o_two_dates.md
    ├── gpt-4o_aquarium.md
    ├── gpt-o3-mini_two_dates.md
    ├── deepseek-r1_two_dates.md
    ├── sonnet-3.5_two_dates.md
    ├── gemini-flash_two_dates.md
    └── ...
```

## Datasets

- **Puzzles:** Math puzzles from GMIL 2025 (Category CM), translated into English.  
- **Solutions:** AI model responses with correctness annotations.

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-github-username/gmil-cm-benchmark.git
   cd gmil-cm-benchmark
   ```

2. **Explore the Data:**
   - Open the `data/` folder to view the puzzles and benchmark results.

3. **Review transcripts:**
   - Open the `transcripts/` folder to view the transcripts of the model responses.

## License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this project with proper attribution.  

## Acknowledgments

- Inspired by the **GMIL Competition** organized by Wrocław University of Science and Technology.  
- Special thanks to Michał Warda, Łukasz Wróbel, and Tomek Gancarczyk for the inspiration.  
- And of course, a huge shout-out to **Anika** for her amazing puzzle-solving skills!