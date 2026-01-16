# Kepler-s-Eye
Kepler’s Eye is a distributed, near–real-time digital twin of Low Earth Orbit (LEO). The system ingests Two-Line Element (TLE) data for 25,000+ space objects, computes their orbital trajectories using distributed processing (Apache Spark), identifies potential collision risks, and visualizes results on an interactive 3D globe.

## Proper Structure

keplers-eye/
├── .gitignore                     # (Functional) Git ignore rules
├── PROJECT_MASTERPLAN.md          # (Doc) The full idea/roadmap you pasted earlier
├── requirements.txt               # (Functional) Python dependencies
│
├── airflow/
│   └── dags/
│       └── DAG_REGISTRY.md        # (Doc) List of active workflows & schedules
│
├── backend/
│   ├── app/
│   │   └── API_ARCHITECTURE.md    # (Doc) Explains models, endpoints, & logic
│   └── Dockerfile                 # (Functional) Backend container build
│
├── frontend/
│   ├── .streamlit/
│   │   └── config.toml            # (Functional) Streamlit theme settings
│   └── app.py                     # (Functional) Main dashboard script
│
├── infrastructure/
│   ├── docker-compose.yaml        # (Functional) Infrastructure definition
│   ├── minio/
│   │   └── BUCKET_POLICIES.md     # (Doc) Explains bucket names & access rules
│   └── postgres/
│       └── init.sql               # (Functional) SQL to run on startup
│
├── notebooks/
│   └── EXPERIMENT_LOG.md          # (Doc) Rules for prototyping vs production code
│
└── spark/
    ├── jobs/
    │   └── JOB_CATALOG.md         # (Doc) Explains what each Spark job calculates
    └── Dockerfile                 # (Functional) Spark container build