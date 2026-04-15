---
permalink: /members/
title: "Members"
excerpt: ""
author_profile: true
---

<style>
  .member-section {
    margin-bottom: 40px;
  }

  .member-section h2 {
    border-bottom: 2px solid #eee;
    padding-bottom: 5px;
    margin-bottom: 15px;
  }

  .member-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }

  .member-card {
    flex: 0 0 calc(33.333% - 20px); /* 三个一行 */
    box-sizing: border-box;
    border: 1px solid #eee;
    border-radius: 8px;
    padding: 15px;
    background: #fff;
  }

  .member-card img {
    width: 100%;
    aspect-ratio: 3 / 4; /* 强制统一照片比例 */
    object-fit: cover;
    border-radius: 8px;
    display: block;
    margin-bottom: 10px;
  }

  .member-name {
    font-weight: bold;
    margin-bottom: 5px;
    font-size: 1.1em;
  }

  .member-meta {
    font-size: 0.9em;
    color: #555;
    line-height: 1.4;
  }

  @media (max-width: 768px) {
    .member-card {
      flex: 0 0 calc(50% - 20px); /* 手机端两个一行 */
    }
  }
  @media (max-width: 480px) {
    .member-card {
      flex: 0 0 100%; /* 极窄屏幕一个一行 */
    }
  }
</style>

# Team Members

{% assign m2023 = site.data.members.masters_2023 %}
{% assign m2024 = site.data.members.masters_2024 %}
{% assign m2025 = site.data.members.masters_2025 %}
{% assign m2026 = site.data.members.masters_2026 %}
{% assign alumni_m2022 = site.data.members.alumni_masters_2022 %}
{% assign u2024 = site.data.members.undergrads_2024 %}

<!-- 2023级硕士生 -->
<div class="member-section">
  <h2>硕士生（2023级）</h2>
  <div class="member-grid">
  {% if m2023 %}
    {% for m in m2023 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>

<!-- 2024级硕士生 -->
<div class="member-section">
  <h2>硕士生（2024级）</h2>
  <div class="member-grid">
  {% if m2024 %}
    {% for m in m2024 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>

<!-- 2025级硕士生 -->
<div class="member-section">
  <h2>硕士生（2025级）</h2>
  <div class="member-grid">
  {% if m2025 %}
    {% for m in m2025 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>

<!-- 2026级硕士生 -->
<div class="member-section">
  <h2>硕士生（2026级）</h2>
  <div class="member-grid">
  {% if m2026 %}
    {% for m in m2026 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>

<!-- 已毕业：2022级硕士生 -->
<div class="member-section">
  <h2>已毕业 · 硕士生（2022级）</h2>
  <div class="member-grid">
  {% if alumni_m2022 %}
    {% for m in alumni_m2022 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.employer %}工作单位：{{ m.employer }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>

<!-- 2024级本科生 -->
<div class="member-section">
  <h2>本科生（2024级）</h2>
  <div class="member-grid">
  {% if u2024 %}
    {% for m in u2024 %}
    <div class="member-card">
      {% if m.photo %}
      <img src="{{ m.photo | relative_url }}" alt="{{ m.name }}">
      {% endif %}
      <div class="member-name">{{ m.name }}</div>
      <div class="member-meta">
        {% if m.research %}研究方向：{{ m.research }}<br>{% endif %}
        {% if m.email %}邮箱：{{ m.email }}{% endif %}
      </div>
    </div>
    {% endfor %}
  {% else %}
    <p>暂无信息</p>
  {% endif %}
  </div>
</div>