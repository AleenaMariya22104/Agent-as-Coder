# Agent-as-Coder


## AI Agent: Bank Statement Parser Generator 
Agent Logic<br>
This agent follows a Plan-Generate-Test workflow. It plans a parsing strategy for a given bank statement PDF, generates a Python parser script based on that plan, and then tests the new parser by comparing its output against a known-good CSV file to verify its accuracy.<br>

## How to Run
1. Clone the Repository <br>
git clone Agent-as-Coder <br>
cd Agent-as-Coder <br>
2. Set Up Directories <br>
Create the data/icici/ directory and place the icici sample.pdf and result.csv files inside. <br>
3. Install Dependencies <br>
pip install pandas pdfplumber numpy <br>
4. Run the Agent <br>
python3 agent.py --target icici <br>
5. Verify Output <br>
A new parser is created at custom_parsers/icici_parser.py, and a "✅ Test Passed" message appears in the terminal. <br>
