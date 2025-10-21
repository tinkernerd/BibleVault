---
title: <% tp.file.title %>
created_at: <% tp.file.creation_date('YYYY-MM-DD[T]HH:mm:ssZ') %>
modified_at: <% tp.file.last_modified_date('YYYY-MM-DD[T]HH:mm:ssZ') %>
category: Bible Study
type: Passage Study
topic: 
  - <% await tp.system.prompt("Enter primary topic (e.g., Salvation, Faith, Grace):") %>
tags:
  - bible/study
  - passage
  - <% await tp.system.prompt("Enter book name (e.g., Romans, Colossians):") %>
status: Active
---

# **<% tp.file.title %>**

> *"<% await tp.system.prompt("Enter main verse or passage (e.g., Romans 10:9–10)") %>"*  
> — **<% await tp.system.prompt("Enter Bible version (e.g., NIV, ESV, NKJV):") %>**

---

## **Context**

<% await tp.system.prompt("Summarize the background or setting of this passage (e.g., Paul writing to the Romans to explain salvation):") %>

Include historical notes, author, audience, and why the passage was written.  
If applicable, mention what comes before and after in the text for flow.

---

## **Main Themes & Key Verses**

### 📖 Verse Breakdown

| Verse | Summary | Reflection |
|-------|----------|-------------|
| <% await tp.system.prompt("Enter verse reference 1 (e.g., Romans 3:23)") %> | <% await tp.system.prompt("Summarize key idea (e.g., All have sinned)") %> | <% await tp.system.prompt("Add reflection or insight (e.g., Sin separates us from God, revealing our need for grace.)") %> |
| <% await tp.system.prompt("Enter verse reference 2 (optional)") %> |  |  |
| <% await tp.system.prompt("Enter verse reference 3 (optional)") %> |  |  |

🪜 *Optional analogy or personal illustration (e.g., “Preventive maintenance” or “Walking the narrow road”)*

---

## **Cross-References**

- 📖 **<% await tp.system.prompt("Enter related verse 1 (e.g., Ephesians 2:8–9)") %>** — <% await tp.system.prompt("Add why it's relevant (e.g., Salvation is a gift, not earned.)") %>  
- 📖 **<% await tp.system.prompt("Enter related verse 2") %>** —  
- 📖 **<% await tp.system.prompt("Enter related verse 3") %>** —  

---

## **Reflection & Application**

- 💭 **Personal Reflection:**  
  <% await tp.system.prompt("What is God teaching me through this passage?") %>

- 🛠 **Practical Application:**  
  <% await tp.system.prompt("How can I apply this truth in daily life? (e.g., Pray proactively, seek wisdom before decisions)") %>

- 🙏 **Prayer Focus:**  
  <% await tp.system.prompt("Write a short prayer related to this passage") %>

---

## **Key Takeaway**

> <% await tp.system.prompt("Summarize one or two sentences that capture the heart of this passage (e.g., The Gospel begins with honesty about our need and ends with assurance in Christ.)") %>

---

## **Notes & Insights**

<% await tp.system.prompt("Add any study notes, Greek/Hebrew words, or commentary highlights you'd like to include.") %>

---

## **References**

- [[Bible Index|🏠 Bible Index]]  
- [[Cross-References]]  
- [[Themes]]  

---
