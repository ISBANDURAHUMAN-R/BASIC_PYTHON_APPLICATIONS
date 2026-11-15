<p align="center">
  <img src="assets/banner.png" alt="BASIC_PYTHON_APPLICATIONS Banner" width="100%">
</p>

# ◈ CodSoft Python Programming Tasks

[![CI](https://github.com/ISBANDURAHUMAN-R/CODSOFT_taskno_PYTHON/actions/workflows/ci.yml/badge.svg)](https://github.com/ISBANDURAHUMAN-R/CODSOFT_taskno_PYTHON/actions/workflows/ci.yml)

## ◆ About the Project
This repository contains a collection of foundational Python projects completed during the CodSoft Python Programming Internship. The projects encompass daily productivity tools, mathematical utilities, cybersecurity generators, and game logic scripts designed to reinforce core Python fundamentals.

## ❖ Key Features
- To-Do List (`TO_DO_LIST.py`): Console task manager supporting task creation, updating, deletion, and status tracking.
- Calculator (`CALCULATOR.py`): Terminal arithmetic calculator executing addition, subtraction, multiplication, and division with error handling.
- Password Generator (`PASSWORD_GENERATOR.py`): Configurable password generation utility creating secure character strings based on user-specified length and complexity.
- Rock Paper Scissors (`ROCK_PAPER_SCISSOR.py`): Turn-based game engine against computer randomness with scorekeeping and rematch loops.

## ◆ System Architecture
```mermaid
graph TD
    subgraph Suite ["CodSoft Python Tasks Suite"]
        T1["TO_DO_LIST.py<br/>Task Management"]
        T2["CALCULATOR.py<br/>Arithmetic Engine"]
        T3["PASSWORD_GENERATOR.py<br/>Entropy Generator"]
        T4["ROCK_PAPER_SCISSOR.py<br/>Game Mechanics"]
    end

    subgraph T1Logic ["To-Do Engine"]
        T1 --> T1In["Task Input Stream"]
        T1In --> T1Ops["Create • Update • Delete • Status"]
        T1Ops --> T1Mem["In-Memory Task Store"]
    end

    subgraph T2Logic ["Calculator Engine"]
        T2 --> T2In["Numeric Inputs & Opcode"]
        T2In --> T2Eval{"Operation: + - * /"}
        T2Eval --> T2Div{"Zero Check"}
        T2Div -- DivZero --> T2Err["Math Error Guard"]
        T2Div -- Valid --> T2Res["Computed Output"]
    end

    subgraph T3Logic ["Password Generator"]
        T3 --> T3Len["Complexity & Length Parameters"]
        T3Len --> T3Charset["Character Sets: Upper • Lower • Digits • Punct"]
        T3Charset --> T3RNG["Pseudo-Random String Sampler"]
        T3RNG --> T3Pass["Generated Password String"]
    end

    subgraph T4Logic ["RPS Game Loop"]
        T4 --> T4User["User Choice"]
        T4 --> T4Bot["RNG Computer Choice"]
        T4User & T4Bot --> T4Judge["Outcome Evaluator"]
        T4Judge --> T4Score["Cumulative Score Tracker"]
    end
```

## ⬢ Technologies Used
- Python 3
- Python Standard Library (`random`, `string`)

## § Requirements
- Python 3.8 or higher

## ▲ Installation & Execution
```bash
# Run individual task applications:
python TO_DO_LIST.py
python CALCULATOR.py
python PASSWORD_GENERATOR.py
python ROCK_PAPER_SCISSOR.py
```

## ※ Developer
Developer: ISBANDU RAHUMAN R  
GitHub: https://github.com/ISBANDURAHUMAN-R
