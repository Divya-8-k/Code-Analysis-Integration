# Improve Prompts and Code-Analysis Integration

## 📌 Project Overview

This project demonstrates how to improve the integration between static code-analysis tools and Large Language Models (LLMs) for automated code review.

The system combines reports from multiple analysis tools such as Flake8, Pylint, and Bandit into a structured prompt. This prompt is then used to generate a detailed code-review report containing issue explanations, severity levels, and recommended fixes.

The objective is to improve the quality and clarity of automated code reviews through better prompt engineering.

---

## 🎯 Objectives

The main objectives of this project are:

* Improve prompt engineering for code review.
* Integrate outputs from multiple static-analysis tools.
* Create structured prompts for LLM-based review.
* Explain detected code issues.
* Assign severity levels to identified issues.
* Recommend fixes and best practices.
* Demonstrate an AI-assisted code-review workflow.

---

## 🛠️ Technologies Used

| Technology   | Purpose                               |
| ------------ | ------------------------------------- |
| Python       | Implementation                        |
| Flake8       | Style and formatting analysis         |
| Pylint       | Code quality analysis                 |
| Bandit       | Security vulnerability analysis       |
| LLM          | Issue explanation and recommendations |
| Google Colab | Development environment               |
| GitHub       | Version control and project hosting   |

---

## 📂 Project Structure

```text id="gq52lk"
Improve-Prompts-and-Code-Analysis-Integration/
│
├── improved_prompt_integration.py
├── README.md
```

---

## 🔍 Sample Analysis Reports

The project uses sample outputs from static-analysis tools.

### Flake8 Report

```text id="1z9ncv"
sample.py:5:13: E231 missing whitespace after ','
```

### Pylint Report

```text id="yfdj1d"
W0611: Unused import os
W0612: Unused variable 'temp'
```

### Bandit Report

```text id="ryg7d0"
B105: Possible hardcoded password
```

---

## 🤖 Improved Prompt

The reports are combined into a structured prompt:

```text id="a9yk5g"
You are an expert software engineer and security reviewer.

Analyze the following static-analysis reports.

For each issue provide:

1. Issue Name
2. Explanation
3. Severity
4. Why it matters
5. Recommended Fix
```

This structured format helps the LLM generate more consistent and useful code reviews.

---

## 📋 Example Review Output

### Issue 1: Missing Whitespace After Comma

**Severity:** Low

**Explanation:**
Function arguments should contain a space after commas.

**Recommended Fix:**

```python id="m4v8sn"
def add(a, b)
```

---

### Issue 2: Unused Import

**Severity:** Medium

**Explanation:**
Imported modules that are never used create unnecessary code clutter.

**Recommended Fix:**
Remove the unused import.

---

### Issue 3: Unused Variable

**Severity:** Medium

**Explanation:**
The variable is declared but never used.

**Recommended Fix:**
Remove the variable or use it where required.

---

### Issue 4: Hardcoded Password

**Severity:** High

**Explanation:**
Sensitive credentials are stored directly in source code.

**Recommended Fix:**
Use environment variables or a secure secret-management solution.

---

## 🔄 Workflow

```text id="7g7s9o"
      Static Analysis Reports
                 ↓
        Combined Prompt
                 ↓
         Prompt Engineering
                 ↓
            LLM Review
                 ↓
      Issue Explanations
                 ↓
      Severity Assessment
                 ↓
      Recommended Fixes
```

---

## 📚 Learning Outcomes

This project demonstrates:

* Prompt engineering techniques
* Static code analysis
* Security vulnerability awareness
* Automated code-review workflows
* LLM-assisted software engineering
* Integration of analysis tools with AI systems

---

## 🚀 How to Run

### Step 1: Open Google Colab

Create a new Colab notebook.

### Step 2: Copy the Python Code

Paste the contents of `improved_prompt_integration.py`.

### Step 3: Run the Notebook

Execute the cell.

### Step 4: View Results

The notebook will:

1. Generate a structured review prompt.
2. Simulate static-analysis results.
3. Produce an LLM-style code-review report.
4. Display issue explanations and recommendations.

---

## 👩‍💻 Author

**Divya K**

---

## 📌 Project Type

**Prompt Engineering and LLM-Assisted Code Analysis**
