---
id: ECO.SOTA.006
title: "EdTech Regulatory Landscape (2025-2026)"
type: sota
status: active
created: 2026-03-24
source: "6B Education GDPR/COPPA/FERPA, AI Governance Group Compliance, BigID COPPA Updates, NEA Federal AI Regulations, Global Privacy Assembly DEWG 2025"
related: [ECO.M.014, ECO.D.006]
s2r_families: [F3]
---

# ECO.SOTA.006: EdTech Regulatory Landscape (2025-2026)

## Контекст

EdTech регуляторная среда ужесточается по трём осям: детские данные (COPPA 2.0), AI governance (EU AI Act), персональные данные (GDPR/state laws). Школы используют в среднем 1,449 EdTech-инструментов — каждый подлежит compliance.

---

## Ключевые регуляции

### COPPA 2.0 (США, 2025-2026)

| Аспект | До | После (июнь 2025) |
|--------|-----|-------------------|
| Consent model | Opt-out | **Opt-in** (явное согласие родителя) |
| Данные в scope | PII | + **геолокация, биометрия** |
| Штрафы | Варьируются | До **$51,744 за ребёнка** |
| Third-party sharing | Допускалось | Явное разрешение родителя |
| Full compliance deadline | — | **22 апреля 2026** |

**Импакт для IWE:** Если работаем с <13 лет — полный COPPA compliance. Если >13 — COPPA не применяется, но state laws могут.

### EU AI Act (поэтапно, 2025-2026)

| Дата | Что вступает |
|------|-------------|
| Февраль 2025 | Запрещённые AI-практики (social scoring, real-time biometric) |
| Август 2025 | Обязательства для general-purpose AI |
| **Август 2026** | **Полные требования для high-risk AI** |
| Штрафы | До **€35M или 7% global turnover** |

**Классификация:** AI в образовании = **high-risk** (Annex III). Требования: risk management, data governance, transparency, human oversight, accuracy/robustness.

**Импакт для IWE:** Digital Twin и AI coaching → high-risk category → нужна документация, human oversight, data governance.

### GDPR (ЕС, действует)

| Требование | Применение к EdTech |
|-----------|---------------------|
| Lawful basis | Consent или legitimate interest |
| Data minimization | Собирать только необходимое |
| Right to erasure | Удаление по запросу |
| Data portability | Export данных пользователя |
| DPO | Обязателен при масштабной обработке |

### FERPA (США, образовательные учреждения)

Применяется к учреждениям, получающим федеральное финансирование. EdTech-vendor = «school official» с legitimate educational interest. Не требует consent, но требует data agreement.

---

## State-Level (США)

- **121+ законов** о защите данных учащихся (сверх FERPA)
- **620% рост** законодательства по cybersecurity/privacy с 2020
- Тренд: каждый штат добавляет свои требования (CA CCPA/CPRA, CO Privacy Act, CT, VA)

---

## Multi-Layer Compliance Stack

```
EdTech платформа
├── Международный: GDPR, EU AI Act
├── Федеральный (US): COPPA, FERPA
├── Штат (US): CCPA, state student privacy laws
└── Отраслевой: SOC 2, ISO 27001 (добровольный, но ожидаемый)
```

---

## Compliance Checklist для EdTech стартапа

### Минимум (seed stage)

- [ ] Privacy Policy опубликована, актуальна
- [ ] Cookie consent (GDPR: opt-in для EU)
- [ ] Data Processing Agreement (если B2B)
- [ ] Data encryption at rest + in transit
- [ ] Incident response plan (хотя бы basic)

### При масштабировании

- [ ] SOC 2 Type II аудит
- [ ] GDPR DPO назначен (если EU users)
- [ ] COPPA compliance (если <13)
- [ ] EU AI Act documentation (если AI = high-risk)
- [ ] Data portability (export по запросу)
- [ ] Regular penetration testing

---

## Ключевые выводы для IWE

1. **EU AI Act high-risk:** Digital Twin и AI coaching → документация, human oversight, data governance нужны к августу 2026
2. **GDPR:** Уже применяется, минимум = Privacy Policy + consent + DPA
3. **COPPA:** Не применяется если аудитория >13 лет (IWE = взрослые professionals)
4. **SOC 2:** Ожидается при B2B (университеты, корпоративные клиенты)
5. **Proactive approach:** Compliance как competitive advantage, не как бремя
