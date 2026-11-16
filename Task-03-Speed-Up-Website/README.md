# Task 3: Speed Up a Website

## Objective
Analyze the mobile performance of three websites using Google PageSpeed Insights, identify major performance issues, and recommend practical improvements in simple language.

## Tool Used
- Google PageSpeed Insights
- Lighthouse mobile performance audit
- GitHub for documentation

## Websites Tested
1. Cloud Security Portfolio (GitHub Pages)
2. Wikipedia
3. BBC

## Performance Comparison

| Website | Performance | Accessibility | Best Practices | SEO |
|---|---:|---:|---:|---:|
| Cloud Security Portfolio | 100 | 100 | 100 | 90 |
| Wikipedia | 98 | 94 | 100 | 100 |
| BBC | 37 | 93 | 54 | 100 |

Scores are from mobile Lighthouse tests performed on November 16, 2026. They represent individual test runs and can vary over time.

## Website 1: Cloud Security Portfolio

**Performance score:** 100/100

### Key Results
- First Contentful Paint: 0.8 s
- Largest Contentful Paint: 0.8 s
- Total Blocking Time: 0 ms
- Speed Index: 0.8 s
- Cumulative Layout Shift: 0

### Analysis
The website performed very well because it is a lightweight static HTML and CSS page with limited external resources. No major performance problems were visible in the provided audit.

### Recommended Improvements
- Continue keeping CSS and HTML lightweight.
- Optimize any images added in the future.
- Avoid unnecessary JavaScript and external dependencies.
- Recheck performance after website updates.

## Website 2: Wikipedia

**Performance score:** 98/100

### Key Results
- First Contentful Paint: 1.0 s
- Largest Contentful Paint: 1.2 s
- Total Blocking Time: 150 ms
- Speed Index: 2.4 s
- Cumulative Layout Shift: 0.012

### Problems Found
1. Inefficient cache lifetimes: estimated 27 KiB savings.
2. Image delivery could be improved: estimated 35 KiB savings.
3. One long main-thread task was identified.
4. Some elements were animated without compositor-friendly techniques.

### Recommended Fixes
- Use appropriate browser caching for static resources.
- Compress and resize images to reduce download size.
- Break long JavaScript tasks into smaller operations.
- Prefer efficient CSS animations using transform and opacity.

## Website 3: BBC

**Performance score:** 37/100

### Key Results
- First Contentful Paint: 1.3 s
- Largest Contentful Paint: 8.5 s
- Total Blocking Time: 2,360 ms
- Speed Index: 10.4 s
- Cumulative Layout Shift: 0.049

### Problems Found
1. High JavaScript execution time: 6.5 seconds.
2. Excessive main-thread work: 9.0 seconds.
3. Unused JavaScript: estimated 726 KiB savings.
4. Inefficient caching: estimated 1,249 KiB savings.
5. Unoptimized images: estimated 165 KiB savings.
6. Large network payload: 4,333 KiB.
7. Forced reflow and network dependencies may delay rendering.

### Recommended Fixes
- Remove unused JavaScript and defer noncritical scripts.
- Reduce long main-thread tasks to improve responsiveness.
- Optimize large images using modern formats and responsive sizes.
- Configure appropriate caching for static assets.
- Reduce unnecessary third-party scripts and resource downloads.
- Prioritize critical content, including the largest visible image.
- Minimize unnecessary layout recalculations.

### Important Observation
The BBC passed its real-user Core Web Vitals assessment, even though its simulated mobile Lighthouse performance score was 37. These assessments use different measurement methods and conditions.

## Conclusion
The Cloud Security Portfolio achieved the highest performance score (100), followed by Wikipedia (98), while BBC scored 37 in the tested mobile Lighthouse runs.

The results show that website complexity, JavaScript execution, image optimization, caching, and network payloads can influence page loading performance.

These are proposed improvements based on PageSpeed Insights findings. No changes were made to Wikipedia or BBC.

## Evidence

The complete Google PageSpeed Insights screenshots for all three websites are available in the PDF below.

[View Task 3 PageSpeed Analysis Evidence](Task-03-PageSpeed-Analysis-Evidence.pdf)

## Project Status

Completed ✅
