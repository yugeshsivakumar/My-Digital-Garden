---
layout: page
title: Home
id: home
permalink: /
---

# Welcome to My Digital Garden! 🌱✨  

<p style="padding: 2em 1.5em; background: linear-gradient(135deg, #e3f2fd, #f5f7ff); border-radius: 8px; text-align: center;">
  🌟 Start exploring with <span style="font-weight: bold">[[your-first-note]]</span> and grow your knowledge base!  
</p>

---

## 📌 Recently Updated Notes  

<ul style="list-style-type: none; padding: 0;">
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li style="margin: 10px 0; padding: 10px; background: #f9f9f9; border-radius: 6px; transition: 0.3s;">
      📝 <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}" style="text-decoration: none; font-weight: bold;">
        {{ note.title }}
      </a>  
      <span style="color: #666; font-size: 0.9em;">({{ note.last_modified_at | date: "%Y-%m-%d" }})</span>
    </li>
  {% endfor %}
</ul>

---

## ✨ How to Navigate?  
📂 Browse notes from the sidebar 
🔗 Use **internal links** to connect thoughts  
🧠 Build your **knowledge network**  

<style>
  .wrapper {
    max-width: 48em;
  }
  li:hover {
    background: #e3f2fd;
  }
</style>
