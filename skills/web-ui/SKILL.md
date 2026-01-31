---
name: web-ui
description: Build polished, production-ready web interfaces. Use when creating UI components, pages, layouts, forms, or any visual interface work.
---

# Web UI Development

Use this skill when building user interfaces for web applications. This guide directs you to the right component libraries and patterns.

## When to Use

- Creating UI components and pages
- Building forms, data tables, navigation
- Implementing modals, dialogs, toasts
- Styling with Tailwind CSS
- Building responsive, accessible interfaces

## Recommended Component Libraries

### shadcn/ui (Primary)
https://ui.shadcn.com/

Copy-paste components built with Radix UI and Tailwind CSS. Use as your foundation for all standard UI needs.

**Always check the shadcn/ui documentation for:**
- Available components and their variants
- Installation commands
- Usage patterns and props
- Accessibility features

### Cult UI (Animations & Effects)
https://www.cult-ui.com/

Animated components that complement shadcn/ui. Use for enhanced visual effects like animated backgrounds, text effects, and interactive elements.

**Check Cult UI documentation for:**
- Animation components
- Visual effects
- Interactive patterns

## Component Selection Approach

1. **Check shadcn/ui first** - It likely has what you need (buttons, inputs, dialogs, tables, navigation, forms, etc.)
2. **Use Cult UI for animations** - When you need motion, transitions, or visual flair
3. **Look up current documentation** - Components and APIs evolve; always reference the latest docs

## Icons

Use **Lucide Icons** (included with shadcn/ui): https://lucide.dev/icons/

Browse the icon library and import what you need.

## Color Palettes

Use HSL format for shadcn/ui compatibility. The shadcn/ui themes page provides ready-to-use palettes: https://ui.shadcn.com/themes

## Typography

Use **Google Fonts** for web fonts: https://fonts.google.com/

Common choices: Inter, Geist, Plus Jakarta Sans

## Responsive Design (Tailwind Breakpoints)

```
sm:  640px   - Landscape phones
md:  768px   - Tablets
lg:  1024px  - Laptops
xl:  1280px  - Desktops
2xl: 1536px  - Large screens
```

## Best Practices

- Use shadcn/ui as your component foundation
- Always reference current library documentation for usage
- Implement loading states with Skeleton components
- Use React Hook Form + Zod for form validation
- Test on multiple screen sizes
- Use CSS variables for theming
