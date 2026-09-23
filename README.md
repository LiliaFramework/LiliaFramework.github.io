<p align="center">
 <strong>Lilia Documentation — Framework Guides & Reference</strong><br/>
 The documentation site for the Lilia roleplay framework, covering installation, configuration, APIs, hooks, modules, and development workflows.<br/>
 Built with MkDocs and published as the central reference for the Lilia ecosystem.
</p>

<p align="center">
 <img src="https://bleonheart.github.io/Samael-Assets/lilia.png?raw=true" alt="Lilia Logo" width="220" />
</p>

<p align="center">
 <a href="./License">
  <img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="GPLv3" />
 </a>
 <a href="https://liliaframework.github.io">
  <img src="https://img.shields.io/badge/Documentation-liliaframework.github.io-blue?logo=readthedocs&logoColor=white" alt="Documentation Website" />
 </a>
 <img src="https://img.shields.io/badge/Built%20with-MkDocs-526CFE?logo=materialformkdocs&logoColor=white" alt="MkDocs" />
</p>

---

## Overview

This repository publishes the Lilia documentation site.

The documentation covers:

- Framework installation and setup
- Configuration
- Core concepts and definitions
- Libraries and APIs
- Hooks and events
- Meta tables
- Modules
- Developer workflows
- Generators and reference material

Documentation website:

https://liliaframework.github.io

## Documentation Source

Canonical documentation work should be made through the main Lilia repository:

https://github.com/LiliaFramework/Lilia/tree/main/documentation

When contributing documentation, make changes there and open the pull request against the main Lilia repository rather than treating this publishing repository as the primary source.

## Local Development

Clone the main Lilia repository:

```bash
git clone https://github.com/LiliaFramework/Lilia.git
cd Lilia/documentation
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it, then install the documentation dependencies:

```bash
pip install mkdocs mkdocs-material mkdocs-awesome-pages-plugin
```

Start the local development server:

```bash
mkdocs serve
```

Then open:

```text
http://127.0.0.1:8000
```

## Repository Structure

```text
LiliaFramework.github.io/
├── docs/
├── scripts/
├── mkdocs.yml
├── modules.json
├── version.json
└── README.md
```

## Contributing

Documentation improvements are welcome through the main Lilia repository.

Useful contributions include:

- Clearer explanations
- Additional examples
- New guides
- Missing API reference material
- Hook documentation
- Corrections to outdated information
- Typo and formatting fixes

Test documentation locally before submitting changes.

## License

The documentation repository is distributed under the GNU General Public License v3.0.

See [License](./License) for details.