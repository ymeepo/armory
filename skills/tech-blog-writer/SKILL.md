---
name: tech-blog-writer
description: Write compelling technical blog posts. Use when creating blog posts, explaining complex topics, drafting newsletter articles, or writing educational technical content.
---

# Technical Blog Writing

Use this skill when writing technical blog posts, explaining complex topics to developers, or creating educational content.

## When to Use

- Writing technical blog posts
- Explaining complex topics to a technical audience
- Creating educational developer content
- Drafting newsletter articles
- Transforming dry technical documentation into engaging content

## Voice and Tone

### Personal and Reflective

Write in first person with a reflective voice. Ground abstract concepts in your own experience and discovery.

**Good:** "I've been building distributed systems for a few years now, and something clicked recently about how we think about consistency. It started when I was debugging a particularly stubborn race condition..."

**Bad:** "Distributed systems present unique consistency challenges. This post will explore best practices for handling race conditions."

### Conversational but Thoughtful

Write like you're explaining to a thoughtful colleague. Not overly casual, not stiff. Let your thinking show.

**Good:** "The thing that took me a while to understand is that the database isn't really the bottleneck here. It's how we're thinking about the problem in the first place."

**Bad:** "Database performance optimization requires understanding system bottlenecks and applying appropriate strategies."

### Advocacy Over Criticism

Frame ideas as discoveries and insights, not as corrections to common mistakes. You're sharing what you've learned, not pointing out what others are doing wrong.

**Good:** "I've found that starting with the simplest possible implementation tends to reveal the actual requirements more clearly than trying to anticipate everything upfront."

**Bad:** "Most developers make the mistake of over-engineering their solutions. Here's how to avoid this common trap."

### Let Ideas Flow Naturally

Avoid punchy one liners and quotable phrases. Don't try to be clever. Let the ideas carry themselves.

**Good:** "Over time, I've come to think of error handling less as a defensive measure and more as a way of understanding what the system is actually trying to do."

**Bad:** "Error handling isn't defense—it's discovery. Remember: every error is a teacher in disguise."

## Structure

### Narrative Over Bullet Points

Tell a story with a beginning, middle, and insight. Weave your points into flowing prose rather than fragmenting them into lists.

**Good:** "When I first started working on this system, the caching layer seemed like the obvious place to focus. We were seeing latency spikes during peak traffic, and the conventional wisdom pointed toward more aggressive caching. But as I dug deeper, I realized we were solving the wrong problem. The latency wasn't coming from cache misses at all. It was coming from how we were coordinating between services."

**Bad:**
- Identified latency spikes during peak traffic
- Initially focused on caching layer
- Discovered the real issue was service coordination
- Lesson: always verify assumptions before optimizing

### Minimize Subheadings

Use subheadings sparingly to mark major shifts in the narrative, not every few paragraphs. Let the prose carry the reader through without constant interruption.

### Build Toward Insight

Rather than stating your thesis upfront and defending it, let the reader discover the insight alongside you. Start with the situation, share what you observed, and let the understanding emerge.

**Good flow:**
1. Here's what I was working on
2. Here's what I noticed
3. Here's what I tried
4. Here's what I came to understand

**Avoid:**
1. Here's my main point
2. Here's why I'm right
3. Here are three supporting arguments
4. In conclusion, I was right

### Weave Examples Into Prose

Rather than calling out examples as separate sections, integrate them into the narrative. They should feel like natural illustrations of what you're describing.

**Good:** "I ran into this recently when building a notification system. The obvious approach would be to process notifications synchronously, but I kept hitting edge cases where messages would get lost during deployments. It wasn't until I separated the intent to notify from the notification itself that things started working reliably."

**Bad:**

**Example: Notification System**

Consider a notification system with the following requirements:
- Must handle deployments gracefully
- Messages cannot be lost
- ...

## Content

### Lead with Personal Experience

Ground abstract concepts in specific, personal experience. Start with the moment of confusion, discovery, or realization that led you to the insight.

**Good:** "I spent most of last month refactoring a service that had grown unwieldy. Somewhere around the third day, staring at a function that had accumulated fifteen parameters over two years, I started thinking about what makes code actually maintainable versus what we just tell ourselves makes code maintainable."

### Focus on the Why

Emphasize the reasoning and the insight rather than step by step instructions. You're helping the reader understand how to think about something, not giving them a recipe to follow.

### Keep Examples Conceptual

Unless explicitly requested, keep examples language agnostic and focused on concepts rather than framework specific implementations. The ideas should transfer across technologies.

**Good:** "The key insight is separating the command from its execution. You capture what the user wants to do, validate it, and only then commit to doing it."

**Bad:** "In Rails, you can implement this pattern using ActiveJob with the following configuration..."

### Describe Constraints and Principles

Rather than prescribing specific solutions, describe the constraints you were working within and the principles that guided your decisions. Let readers apply these to their own contexts.

### End with a Clear Takeaway

Leave the reader with something concrete to think about, but avoid wrapping up too neatly. Real insights don't come with tidy bows.

**Good:** "I'm still not sure this is the right approach for every situation. But for systems where correctness matters more than raw throughput, I keep coming back to this pattern. There's something to it."

**Bad:** "In conclusion, always use event sourcing for distributed systems. Your future self will thank you!"

## What to Avoid

### Bullet Point Lists in the Body

Reserve bullet points for reference material or appendices. The main body should flow as prose.

### Framework Specific Examples

Keep examples conceptual and transferable unless the reader specifically asks for implementation in a particular technology.

### Contrarian Framing

Avoid positioning your insight as a correction to what everyone else is doing wrong. Share what you've learned, not what others should stop doing.

**Avoid:** "We've been thinking about caching wrong this whole time."

**Prefer:** "I've started thinking about caching differently."

### Over Structured Formats

Don't fragment your thinking into many subheadings. Trust the reader to follow your narrative.

### Punchy Closing Lines

Don't try to end with something memorable or quotable. Let the ideas speak for themselves.

**Avoid:** "Because at the end of the day, the best architecture is the one you don't have to think about."

**Prefer:** Just end when you're done. The insight is enough.

## Hyphen Avoidance

Hyphens often make writing feel stiff and overly formal. Prefer natural, flowing prose.

### Rewrite to Avoid

| Hyphenated | Better Alternative |
|------------|-------------------|
| real-time data | data in real time |
| high-performance system | system with high performance |
| user-friendly interface | interface that's friendly to users |
| well-known pattern | pattern that's well known |
| open-source project | open source project |
| built-in feature | feature that's built in |
| cutting-edge technology | technology on the cutting edge |

### When Hyphens Are Acceptable

- Established compound words: "e-commerce", "self-service"
- Prefixes where omission causes confusion: "re-sign" vs "resign"
- Numbers: "21 year old developer"

If you can restructure the sentence to avoid the hyphen without losing clarity, do it. Your prose will read more naturally.
