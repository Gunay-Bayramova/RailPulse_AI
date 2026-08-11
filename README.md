# RailPulse_AI

RailPulse_AI/
├── app.py                         # Streamlit interface only
├── railpulse/
│   ├── __init__.py
│   ├── config.py                  # Environment configuration
│   ├── models.py                  # Structured LLM responses
│   ├── orchestrator.py            # Complete question-to-answer flow
│   ├── llm_client.py              # Ollama or Groq integration
│   ├── prompts.py                 # Required SQL + consultant prompts
│   ├── schema_context.py          # Tables, columns, relationships, units
│   ├── guardrails.py              # SQL validation and allow-list
│   ├── database.py                # Read-only query execution
│   └── formatting.py              # Seconds-to-minutes conversion
├── config/
│   ├── schema.yaml                # Exact database schema and descriptions
│   └── few_shot_examples.yaml     # Question → correct SQL examples
├── evals/
│   └── text_to_sql_cases.yaml     # Evaluation questions and expectations
├── scripts/
│   ├── check_connection.py
│   └── generate_weekly_report.py  # Nice-to-have
├── tests/
│   ├── fixtures/
│   │   ├── schema.sql
│   │   └── sample_data.sql        # Synthetic data only
│   ├── test_guardrails.py
│   ├── test_formatting.py
│   ├── test_sql_generation.py
│   └── test_pipeline.py
├── docs/
│   ├── architecture.md
│   └── demo-guide.md
├── .github/
│   └── workflows/
│       └── ci.yml
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md