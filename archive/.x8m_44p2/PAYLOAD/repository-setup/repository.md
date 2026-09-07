ai-research-sdk/
│ 
├── README.md
├── LICENSE
├── pyproject.toml
├── requirements.txt
├── setup.cfg
├── .gitignore
│
├── cli/                         # CLI entrypoints + command routing
│   ├── __init__.py
│   ├── main.py                  # `ai-sdk` root command
│   ├── commands/
│   │   ├── weave.py             # InfoWeave commands
│   │   ├── aiol.py              # AIOL commands
│   │   ├── agents.py            # agent orchestration commands
│   │   ├── datasets.py
│   │   ├── experiments.py
│   │   └── plugins.py
│   └── utils/
│       └── io.py
│
├── sdk/                         # Core Python SDK
│   ├── __init__.py
│   ├── config/
│   │   ├── settings.py
│   │   └── defaults.yaml
│   ├── weave/                   # InfoWeave integration layer
│   │   ├── client.py
│   │   ├── parser.py
│   │   └── adapters/
│   ├── aiol/                    # AIOL integration layer
│   │   ├── runtime.py
│   │   ├── scheduler.py
│   │   └── protocols/
│   ├── agents/                  # Agentic abstractions
│   │   ├── base.py
│   │   ├── memory.py
│   │   ├── planning.py
│   │   ├── tools.py
│   │   └── registry.py
│   ├── datasets/
│   │   ├── loaders.py
│   │   ├── transforms.py
│   │   └── registry.py
│   ├── experiments/
│   │   ├── runner.py
│   │   ├── tracking.py
│   │   └── metrics.py
│   └── plugins/
│       ├── base.py
│       ├── registry.py
│       └── examples/
│
├── research/                    # Reproducible research workflows
│   ├── notebooks/
│   │   ├── intro.ipynb
│   │   ├── weave_examples.ipynb
│   │   └── aiol_agents.ipynb
│   ├── papers/
│   │   └── methodology.md
│   └── experiments/
│       ├── exp1.yaml
│       ├── exp2.yaml
│       └── results/
│
├── examples/                    # Example CLI + SDK usage
│   ├── weave_pipeline.py
│   ├── aiol_agent.py
│   └── hybrid_research_loop.py
│
├── tests/                       # Full test suite
│   ├── test_cli.py
│   ├── test_weave.py
│   ├── test_aiol.py
│   ├── test_agents.py
│   ├── test_experiments.py
│   └── fixtures/
│
├── docs/                        # Documentation site
│   ├── index.md
│   ├── cli.md
│   ├── sdk.md
│   ├── agents.md
│   ├── weave.md
│   ├── aiol.md
│   └── plugins.md
│
└── .github/
    ├── workflows/
    │   ├── tests.yml
    │   ├── publish.yml
    │   └── lint.yml
    └── ISSUE_TEMPLATE.md
