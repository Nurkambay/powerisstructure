# 🧠 Power Is Structure

> A mathematical framework to analyze organizational power structures and assess their potential for corruption and opacity.

---

## 🔍 What Is It?

**Power Is Structure** is an open-source engine that allows you to represent organizations as **graphs of authority and communication**, then evaluate them using **corruption-prone patterns**, **information flow asymmetry**, and **control bottlenecks**.

The project introduces a novel concept:  
> **Corruption is not random — it emerges from structure.**  
By modeling hierarchies as graphs and identifying specific anti-patterns, we can calculate a **Power Transparency Index** — an estimate of how robust or fragile a structure is in terms of abuse risk.

---

## 🎯 Use Cases

- 🏛️ Government bodies and ministries
- 🏢 Corporations and large departments
- 🧩 NGOs and multi-level organizations
- 🧠 Research in governance and transparency
- 🧪 Experimental simulations of authority systems

---

## ⚙️ How It Works

You provide a graph of your organization (in DOT format), and the engine analyzes it to detect:

- ⚠️ **Opacity Triangles** – chains of command with no alternative feedback paths
- 🚨 **Control Monopolies** – nodes that receive all input but aren't supervised
- 🕸️ **One-way Subgraphs** – no way for data to flow back up
- 📉 **Information Cascade Weakness** – upper management isolated from reality

The result is a **Power Transparency Index** along with a visual graph report.

---

## 🛠 Example

```dot
digraph structure {
    A [label="CEO"]
    B [label="Deputy"]
    C [label="Staff"]

    C -> B
    B -> A
}

⚠️ This is an opacity triangle — CEO receives filtered data from Deputy only.

🔓 License

This project is released under the Mozilla Public License 2.0 (MPL-2.0).
You’re free to use, extend, and integrate the code.
Changes to the core logic must be published under the same license.

👤 Author

Created by Leonid Baranov,
software architect and organizational analysis enthusiast.

Inspired by real-world structures and challenges encountered while studying governance models in post-Soviet and Western systems.

---

🚀 Roadmap
	•	Core index calculation
	•	Visualization patterns
	•	Graph playground (web)
	•	Public scoring API
	•	Integration with HR and audit systems
	•	Community plugin framework

---

🧑‍💻 Contributing

Contributions are welcome! Feel free to:
	•	Submit new graph patterns
	•	Improve the API
	•	Share examples from real-world orgs (anonymized)
	•	Build visual tools

See CONTRIBUTING.md for details.

---

🧠 Philosophy

Structure matters.

The way we connect people, roles, and responsibilities defines the risk of miscommunication, opacity, and abuse.

By making power visible, we make it accountable.

---

🌐 Website

🔗 https://powerisstructure.com
