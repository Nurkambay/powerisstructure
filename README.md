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
