
# Task 4: Optimise Your Own Site

## NEXLEVR Cloud Security Internship — Intermediate Level

### Objective

Run Google Lighthouse on a website I created, identify performance and usability issues, apply improvements, and compare before-and-after results.

### Website Tested

**Website:** Cloud Security Portfolio

**Live Website:** https://kruthajnashankar27-sudo.github.io/NEXLEVR-Cloud-Security-Internship/Task-01-Launch-Website/

**Source Code:** https://github.com/kruthajnashankar27-sudo/NEXLEVR-Cloud-Security-Internship/tree/main/Task-01-Launch-Website

### Tools Used

- HTML5 and CSS3
- GitHub and GitHub Pages
- Google PageSpeed Insights
- Google Lighthouse
- Chrome browser

## 1. Initial Website Analysis

The website was originally created for Task 1 and deployed using GitHub Pages.

During Task 3, I performed a mobile Lighthouse audit and recorded these baseline scores:

| Category | Before |
|---|---:|
| Performance | 100 |
| Accessibility | 100 |
| Best Practices | 100 |
| SEO | 90 |

The website was already lightweight, with no JavaScript, external fonts, or images.

Because its Performance score was already 100, Lighthouse did not identify ten significant performance issues to fix.

## 2. Improvements Implemented

### Improvement 1: SEO Meta Description

Added a descriptive meta tag to the HTML head.

```html
<meta name="description"
      content="Cloud Security Portfolio showcasing secure static website deployment, GitHub Pages hosting, and cybersecurity learning projects.">
```

**Purpose:** Help search engines understand the page's content.

### Improvement 2: Keyboard Accessibility

Added a skip link that allows keyboard users to jump directly to the main content.

```html
<a class="skip-link" href="#main-content">Skip to main content</a>
```

Updated the main element:

```html
<main id="main-content" class="container">
```

Added CSS to show the link when it receives keyboard focus.

**Verification:** Tested the link using the Tab and Enter keys. It appeared and successfully navigated to the main content.

### Improvement 3: Content Correction

Corrected a punctuation error in the Project Status section.

## 3. Before-and-After Lighthouse Results

| Category | Before | After | Result |
|---|---:|---:|---|
| Performance | 100 | 100 | Maintained |
| Accessibility | 100 | 100 | Maintained |
| Best Practices | 100 | 100 | Maintained |
| SEO | 90 | 100 | Improved by 10 points |

### Mobile Performance Metrics

| Metric | Before | After |
|---|---|---|
| First Contentful Paint | 0.8 s | 0.8 s |
| Largest Contentful Paint | 0.8 s | 0.8 s |
| Total Blocking Time | 0 ms | 0 ms |
| Cumulative Layout Shift | 0 | 0 |
| Speed Index | 0.8 s | 0.8 s |

The updated report was captured on November 17, 2026.

## 4. Lighthouse Insights

The updated Lighthouse report included an unscored Largest Contentful Paint (LCP) breakdown.

- LCP element: Paragraph in the About This Project section
- Element render delay: 350 ms
- Overall LCP: 0.8 seconds

The report did not demonstrate ten actionable performance problems. The site already used lightweight HTML and CSS without external images, fonts, or JavaScript.

## 5. Lessons Learned

- Lighthouse can measure performance, accessibility, best practices, and SEO.
- A website with simple HTML and CSS can load quickly.
- Meta descriptions can improve SEO audit results.
- Keyboard navigation should be tested manually.
- Performance optimization should address real issues rather than invent problems.
- Before-and-after measurements help verify changes.

## 6. Evidence

The PDF below contains the original before-and-after
Google Lighthouse screenshots, performance metrics,
and diagnostic findings.

[View Task 4 Lighthouse Evidence](NEXLEVR_Task_04_Before_After_Lighthouse_Evidence.pdf)

## 7. Conclusion

The website maintained a 100/100 Performance score while
improving its SEO score from 90 to 100.

A working keyboard skip link was implemented and tested.

The website was already highly optimized, so Lighthouse
did not identify ten significant performance issues to fix.

## Project Status

Optimization, testing, and evidence documentation completed.
  
