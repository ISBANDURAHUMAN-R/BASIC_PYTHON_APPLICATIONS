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
    subgraph Suite ["&nbsp; CodSoft Python Tasks Suite &nbsp;"]
        T1["&nbsp; TO_DO_LIST.py &nbsp;<br/>&nbsp; Task Manager &nbsp;"]
        T2["&nbsp; CALCULATOR.py &nbsp;<br/>&nbsp; Arithmetic Engine &nbsp;"]
        T3["&nbsp; PASSWORD_GEN.py &nbsp;<br/>&nbsp; Entropy Generator &nbsp;"]
        T4["&nbsp; RPS_GAME.py &nbsp;<br/>&nbsp; Game Mechanics &nbsp;"]
    end

    subgraph T1Logic ["&nbsp; To-Do Engine &nbsp;"]
        T1 --> T1In["&nbsp; Task Input &nbsp;<br/>&nbsp; Stream &nbsp;"]
        T1In --> T1Ops["&nbsp; Create • Update &nbsp;<br/>&nbsp; Delete • Status &nbsp;"]
        T1Ops --> T1Mem["&nbsp; In-Memory &nbsp;<br/>&nbsp; Task Store &nbsp;"]
    end

    subgraph T2Logic ["&nbsp; Calculator Engine &nbsp;"]
        T2 --> T2In["&nbsp; Numeric Inputs &nbsp;<br/>&nbsp; &amp; Opcode &nbsp;"]
        T2In --> T2Eval{"&nbsp; Operation &nbsp;<br/>&nbsp; + - * / &nbsp;"}
        T2Eval --> T2Div{"&nbsp; Zero &nbsp;<br/>&nbsp; Check &nbsp;"}
        T2Div -- DivZero --> T2Err["&nbsp; Math Error &nbsp;<br/>&nbsp; Guard &nbsp;"]
        T2Div -- Valid --> T2Res["&nbsp; Computed &nbsp;<br/>&nbsp; Output &nbsp;"]
    end

    subgraph T3Logic ["&nbsp; Password Generator &nbsp;"]
        T3 --> T3Len["&nbsp; Length &amp; &nbsp;<br/>&nbsp; Complexity &nbsp;"]
        T3Len --> T3Charset["&nbsp; Character Sets: &nbsp;<br/>&nbsp; Upper • Lower &nbsp;<br/>&nbsp; Digits • Punct &nbsp;"]
        T3Charset --> T3RNG["&nbsp; Pseudo-Random &nbsp;<br/>&nbsp; Sampler &nbsp;"]
        T3RNG --> T3Pass["&nbsp; Generated &nbsp;<br/>&nbsp; Password &nbsp;"]
    end

    subgraph T4Logic ["&nbsp; RPS Game Loop &nbsp;"]
        T4 --> T4User["&nbsp; User Choice &nbsp;"]
        T4 --> T4Bot["&nbsp; RNG Choice &nbsp;"]
        T4User & T4Bot --> T4Judge["&nbsp; Outcome &nbsp;<br/>&nbsp; Evaluator &nbsp;"]
        T4Judge --> T4Score["&nbsp; Cumulative &nbsp;<br/>&nbsp; Score Tracker &nbsp;"]
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
