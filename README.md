
# Library & Knowledge Resource Access Control System

**Course:** CT-351 — Knowledge Representation & Reasoning  
**Assignment:** Complex Computing Problem (CCP)  
**Platform:** Google Colab / Python

## Project Overview

The Library & Knowledge Resource Access Control System is a rule-based reasoning prototype that determines whether a library patron is allowed to borrow, access, or use a particular resource.

The system uses a knowledge base containing facts about patrons, library resources, and access permissions. It applies Horn-clause rules and logical inference techniques to make transparent access-control decisions.

## Group Members

| Name | Roll Number |
|---|---|
| Anam Mansoor | AI-23304 |
| Duryab Anwar | AI-23305 |
| Hareem Aqeel | AI-23006 |
| Atika Ali | AI-23013 |

## Key Features

- **Knowledge Base:** Stores facts about patrons, resources, and their access-related attributes.
- **Horn Clauses (R1–R9):** Defines nine logical rules for access control.
- **Forward Chaining:** Derives new conclusions from available facts.
- **Backward Chaining:** Determines whether a requested permission can be logically proved.
- **Default-Deny Policy:** Access is not granted when the required permission cannot be proved.
- **Proof Tracing:** Displays the rules and supporting facts behind a decision.
- **Sample Queries:** Demonstrates both allowed and denied access requests.
- **Unit Testing:** Includes 13 automated tests to validate the reasoning engine.

## Technologies Used

- Python 3
- Google Colab
- Knowledge Representation and Reasoning
- Horn Clauses
- Forward Chaining
- Backward Chaining
- Python `unittest` module

## Repository Structure

```text
Library_Access_Control_CCP/
│
├── Library_Access_Control_CCP_Colab.ipynb
└── README.md
```

## How to Run

### Option 1: Google Colab (Recommended)

1. Open `Library_Access_Control_CCP_Colab.ipynb` from this repository.
2. Click **Open in Colab** or upload the notebook to Google Colab.
3. Select **Runtime → Run all**.
4. Execute the notebook cells to view the demonstrations, inference traces, custom queries, and unit test results.

No additional Python libraries or external database connections are required.

### Option 2: Custom Access-Control Query

The notebook allows users to test custom combinations of patrons, resources, and actions.

**Available Patrons:**
- `sara`
- `omar`
- `nida`
- `hamza`

**Available Resources:**
- `book_ai`
- `book_os`
- `atlas`
- `ebook_ml`
- `journal_faculty`
- `journal_expired`

**Available Actions:**
- `borrow`
- `onsite`
- `digital`

Change the values in the custom query cell and execute it to evaluate a different access request.

## Demonstration

The notebook demonstrates:

1. Sample access-control decisions.
2. Forward-chaining inference with step-by-step rule execution.
3. An allowed request with its proof trace.
4. A denied request where required facts are missing.
5. Custom access-control queries.
6. Automated validation through 13 unit tests.

## Important Notes

- The project uses fictional and illustrative data for educational purposes.
- It is a reasoning and decision-support prototype, not a production library management system.
- It is not connected to the NED University library, a real catalogue, authentication service, or library database.
- It does not actually issue or process book loans.
- A **DENY** decision means that permission could not be proved using the available knowledge base; it does not necessarily prove that the opposite fact is true.

## Conclusion

This project demonstrates how Knowledge Representation and Reasoning techniques can be applied to library access control. By combining Horn clauses, forward chaining, backward chaining, and proof tracing, the system provides transparent and explainable access-control decisions.

