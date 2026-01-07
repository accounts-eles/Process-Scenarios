🔄 Process Scenarios - Interactive Guide

An advanced interactive walkthrough component designed for complex workflows and educational modules. This tool allows users to navigate through multiple high-level scenarios, each containing a dedicated 4-step process flow.

🚀 Live Demo

Explore the Process Scenarios Component Here

✨ Project Overview

The Process Scenarios Guide is built to handle hierarchical information. It features a dual-navigation system: a global "Scenario" switcher for high-level context changes and a local "Step" sidebar for granular process details.

Key Features

Dynamic Data Injection: Scenarios and steps are managed via a centralized JSON array, allowing for easy updates without modifying the core HTML structure.

Two-Tiered Navigation: * Primary: Footer buttons to switch between overarching scenarios.

Secondary: Interactive sidebar buttons to toggle between specific process steps.

Animated Transitions: Content panels utilize slideUp keyframe animations and opacity fades for a smooth, high-end feel.

Visual Step Tracking: Sidebar buttons feature active state tracking with horizontal translation (translateX) to provide clear visual feedback of the user's location in the flow.

Responsive Layout: Uses Tailwind's grid and flex utilities to transform from a vertical stacked layout on mobile to a sophisticated sidebar-and-main-panel layout on desktop.

🛠️ Technical Implementation

Logic Engine: Vanilla JavaScript handles the DOM generation for navigation buttons and content panels, ensuring the interface stays synchronized with the data.

Styling Architecture: * CSS Variables: Centralized brand colors (Midnight Blue, Teal, Light Aqua) for consistent UI scaling.

Tailwind CSS: Used for layout positioning, spacing, and responsive breakpoints.

State Management: An activateStep function manages class toggles, while renderScenario re-paints the UI when the user navigates between global scenarios.

📂 Design Tokens

Midnight Blue (#1f2a52): Used for headers and active states to convey authority and depth.

Teal (#00bec7): The primary action color, used for borders, icons, and navigation buttons.

Light Aqua (#d2f0f0): Used for hover backgrounds and secondary boxes to soften the interface.

Slate Grey (#abb5bf): Provides a neutral palette for secondary information and disabled states.

📖 Usage Instructions

The component automatically initializes on DOMContentLoaded. To add more scenarios, simply append new objects to the scenarios array in the <script> section.

{
    title: "Scenario Name",
    desc: "A brief overview of this specific scenario.",
    steps: [
        { h: "Step Title", p: "Detailed instruction text for this step." },
        // ... requires exactly 4 steps for this layout
    ]
}


📄 License

MIT License - Developed as part of the accounts-eles UI component library.
