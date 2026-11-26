# Day 4 – Tools, Pydantic and Google Sheets

## Objective
Learn how to give LLM agents tools, validate structured data using Pydantic and save business records to Google Sheets.

## Topics Learned
- Why AI agents need tools
- Function calling
- LangChain `@tool`
- Tool names and docstrings
- Agent creation using `create_agent`
- Rate limits and HTTP 429
- Retry handling
- Pydantic BaseModel
- Structured output
- Google Sheets integration using gspread
- Agent execution traces

## Main Practical – Sweet Crumbs Home Bakery

Created a bakery assistant with three tools:

1. `get_price` – Calculates menu prices.
2. `is_open` – Checks opening hours.
3. `log_order` – Validates and saves orders to Google Sheets.

Created an `Order` Pydantic model containing customer name, item, quantity, pickup date and eggless preference.

## Individual Project – Travel & Tour Booking Platform

Created two travel tools:

1. `get_package_price` – Calculates sample package prices.
2. `check_travel_details` – Checks destination and travel date details.

Created a `TravelBooking` Pydantic model and tested structured output using five customer messages.

Created a separate Google Sheet and a `log_travel_booking` tool to save validated booking enquiries.

## Experiments
- Tested a poorly named tool called `tool1`.
- Compared tool names and descriptions.
- Inspected agent execution traces.
- Counted model calls and tool calls.
- Studied HTTP 429 and retry handling.

## Day 5 Preparation
Created `business_facts.txt` containing 20 travel business facts for RAG preparation.

## Technologies Used
- Python
- Google Colab
- Groq API
- LangChain
- Pydantic
- Google Sheets
- gspread

## Files
- `Day4_Tools_Pydantic_GoogleSheets.ipynb` – Day 4 practical and individual tasks.
- `business_facts.txt` – Business facts for RAG.

## How to Run
1. Open the notebook in Google Colab.
2. Add `GROQ_API_KEY` to Colab Secrets.
3. Enable access to the secret.
4. Run the notebook cells in order.
5. Authenticate Google Sheets when prompted.

## Learning Outcome
Learned how to create tool-enabled agents, validate structured records, save data to Google Sheets and inspect the interaction between an LLM and its tools.
