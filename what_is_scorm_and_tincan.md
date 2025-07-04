# SCORM, xAPI, and cmi5: What They Actually Are and What You Actually Get

I've been talking about one of the key challenges in this space being this: SCORM is understood by businesses and is a sunk cost. An LMS that says it doesn't support SCORM is probably as well not bothering! What we've ended up with is a market of LMSes that market that they support xAPI/CMI5 but they only do in principle — i.e., you can upload content formatted that way, but it doesn't mean it'll use it any differently to SCORM.

The big challenge is that LMS vendors just want to sell solutions to pain points; educating their customers that _in order to use this tool properly you need to completely reimagine how you spec, design, and develop learning_ isn't a great sales point.

### Why Adoption of Modern Standards Is Stuck

One of the biggest blockers in moving beyond SCORM isn’t technology — it’s business incentives and culture.

LMS vendors *know* SCORM is limited, but it’s a sunk cost for many organizations. SCORM support is a checkbox on their sales deck. Saying “our LMS doesn’t support SCORM” is a death sentence. So they keep supporting it — often half-heartedly — while adding “xAPI/CMI5 support” mostly as a buzzword.

The hard truth is: educating customers that embracing xAPI or cmi5 means completely reimagining how learning is designed, built, and measured is *not* a great sales pitch. It’s complicated, costly, and threatens the status quo.

As a result, many vendors promote modern standards as features in principle, but don’t help customers actually adopt them. For business leaders, this creates a catch-22: the tech is there, but the organizational mindset, processes, and skills aren’t.

Ultimately, the real challenge isn’t the specs themselves — it’s shifting the culture and expectations around learning development and measurement. Without that, changing standards is just swapping one box-ticking exercise for another.

This is the challenge I see business leaders facing. Although we're talking standards and protocols, it's really in how people see learning development that's the issue.

---

## SCORM (Sharable Content Object Reference Model)

### What It Is

A legacy standard from the late 1990s/early 2000s, SCORM is a packaging and tracking format that lets you launch eLearning content from an LMS and track basic completion data.

### What You Actually Get

- Content that can launch and run inside an LMS  
- Tracking for:  
  - Completion  
  - Pass/fail  
  - Score  
  - Time spent  
- Bookmarking (i.e., resume where you left off)  
- Widespread LMS support

### What You *Don’t* Get

- Any tracking outside the LMS/browser  
- Insight into what learners are actually doing beyond “completed” or “passed”  
- Compatibility with modern learning formats (apps, VR, offline use)  
- Custom tracking or extensibility  
- Analytics that are meaningful in modern L&D

SCORM is *stable and known*, but extremely limited. It assumes learning only happens in tidy packages behind login screens. That’s not how people learn.

---

## xAPI (Experience API, aka Tin Can API)

### What It Is

xAPI is a flexible data format (JSON) and communication standard for tracking *any* learning experience. It moves beyond the LMS and can capture informal, offline, and experiential learning.

### What You Actually Get

- Tracking of learning anywhere: mobile, VR, in-person, simulations, etc.  
- Storage of learning records in a Learning Record Store (LRS)  
- Custom action verbs like “watched”, “repaired”, “mentored”, etc.  
- Decoupling of content from the LMS  
- Extensibility for bespoke tracking needs

### What You *Don’t* Get

- A standardized way to launch or structure content  
- Completion/pass/fail logic (you have to define it yourself)  
- Cohesion — without strict implementation and significant development, an xAPI defined environment becomes a wild west of inconsistent data  
- Simplicity — implementing xAPI well requires significant dev effort and requires a ground up reimagining of instructional design

xAPI is powerful, but it’s *a toolset, not a solution*. You get raw capability, not plug-and-play usefulness.

---

## cmi5 (Computer Managed Instruction — 5th attempt)

### What It Is

cmi5 is a specification built on top of xAPI that **reintroduces structure and launchability**, effectively acting as a proper replacement for SCORM.

### What You Actually Get

- LMS-based launch and tracking of content, just like SCORM  
- Standardized tracking using xAPI statements (completion, score, pass/fail)  
- A defined course structure and start/stop rules  
- Cleaner data in the LRS  
- Compatibility with modern content while retaining LMS delivery  
- Reusable xAPI statements and verbs with expected structure

### What You *Don’t* Get

- SCORM backward compatibility (you’ll need new content)  
- A silver bullet — your learning content still needs to be modular and well-structured, the requirement for reimagining learning strategy from xAPI still remains  
- Broad adoption — cmi5 is emerging, but not yet universal

cmi5 is the spec xAPI should’ve shipped with. It closes the gaps and gives you the structure needed for real-world implementation.

---

## Quick Comparison Table

| Feature                       | SCORM       | xAPI                 | cmi5                       |
|------------------------------|-------------|----------------------|----------------------------|
| LMS launch support            | ✅          | ❌                   | ✅                         |
| Browser-based content         | ✅          | ✅                   | ✅                         |
| Non-browser tracking          | ❌          | ✅                   | ✅                         |
| Completion/pass/fail tracking | ✅          | ❌ (manual setup)    | ✅                         |
| Course structure             | ✅          | ❌                   | ✅                         |
| Real-world/offline learning   | ❌          | ✅                   | ✅                         |
| Data flexibility             | ❌          | ✅                   | ✅                         |
| Developer friendly           | ❌          | ⚠️ (needs setup)     | ⚠️ (better, still very technical) |
| Plug-and-play simplicity      | ✅          | ❌                   | ⚠️ (moderate effort)       |

---

## The Real Issue: It’s Not Technical, It’s Cultural

The problem isn’t just SCORM vs xAPI vs cmi5. The real problem is that **modern learning standards only shine when paired with modern learning practices**.

These standards were designed to support:

- Modular, reusable content  
- Microlearning and just-in-time delivery  
- Data-driven L&D decision making  
- Blended, multi-platform learning experiences

But none of that works if you’re still churning out 45-minute courses packed into a single file.

### Bottom line:

> **SCORM is dying, xAPI is misunderstood, and cmi5 is underused because we’re still designing for 2004.**

Switching specs without changing process is like switching your pen and hoping your writing improves.

---

## Final Thought

If your team is exploring these standards, don’t just ask *what* they do — ask what you're actually trying to achieve.  

- Need modern, flexible tracking? **xAPI** is your base but comes with significant costs in development.  
- Want to replace SCORM responsibly? **cmi5** is the only realistic candidate but is poorly understood and requires significant changes in design mindset.  
- Still building traditional eLearning modules with no tracking needs beyond "completed"? **SCORM still works**, but it's not future-proof.

---

*This article is part of a practical series on learning standards and infrastructure. If you're trying to move beyond buzzwords into meaningful learning tech decisions — you're in the right place.*
