# IPGA

Helping experts turn their expertise into impactful and profitable online education.

IPGA is a set of AI skills (for Claude Code, Claude, or any agent that reads `SKILL.md` files) plus fill-in templates that walk an expert through three stages:

| Stage | What happens | Skill | Templates |
|---|---|---|---|
| 1. Vision & Curriculum | Streamline the idea, define the learner and outcome, build the curriculum | `skills/curriculum-design` | `templates/vision.md`, `templates/curriculum.md` |
| 2. Course Production | Turn the curriculum into scripts, lessons, assets and a recording schedule | `skills/course-production` | `templates/lesson-script.md`, `templates/production-plan.md` |
| 3. Back-End Setup | Sales funnel, pricing, platform, community hosting, launch | `skills/backend-setup` | `templates/sales-funnel.md`, `templates/community-setup.md`, `templates/launch-checklist.md` |

## Quick start

### With Claude Code
```bash
git clone https://github.com/Jayyvro/IPGA.git
cd IPGA
claude
```
Then say: *"Use the curriculum-design skill. My expertise is ___."*

To install the skills globally:
```bash
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/
```

### Without AI
Copy the files in `templates/` and fill them in, in order (vision → curriculum → lesson scripts → production plan → funnel → community → launch).

## Repository layout
```
IPGA/
├── .claude-plugin/plugin.json   # Claude Code plugin manifest
├── skills/
│   ├── curriculum-design/SKILL.md
│   ├── course-production/SKILL.md
│   └── backend-setup/SKILL.md
├── templates/                   # Fill-in worksheets for each stage
└── examples/                    # A worked example course
```

## Workflow
```
Expert idea ──► Vision brief ──► Curriculum ──► Lesson scripts ──► Production plan
                                                                         │
             Launch ◄── Community ◄── Sales funnel ◄── Pricing & platform ◄┘
```

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md).

## License
MIT
