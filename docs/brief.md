# Page Vuilder — Project Brief

## Overview

Page Vuilder is an experimental headless visual page builder for Vue applications.

The project explores how a modern component-driven page builder and SSR rendering system can be built from scratch using Vue and a custom rendering pipeline.

Instead of generating raw HTML, Page Vuilder represents pages as structured trees of Vue components with typed props, configurable layouts, and reusable UI blocks.

The project focuses on understanding and controlling the rendering process while providing a visual editing experience similar to tools like Webflow, GrapesJS, Elementor, or Craft.js, but designed specifically for Vue ecosystems and component-based architectures.

---

# Purpose

The purpose of Page Vuilder is to experiment with and learn:

- Visual page builder architecture
- Component-driven rendering systems
- Server-side rendering (SSR)
- Hydration and client rendering
- Structured page schemas
- Dynamic component rendering
- Component registries
- Typed component configuration
- Headless CMS concepts
- Runtime rendering pipelines

The project is intended primarily as a learning and experimentation platform rather than a production-ready CMS.

---

# Problem

Modern visual page builders often have several limitations:

- They are tightly coupled to specific CMS platforms.
- They generate raw HTML instead of structured component trees.
- They provide limited control over rendering.
- They are difficult to integrate cleanly with modern Vue component systems.
- They are not designed around typed props and reusable application components.
- They often abstract away rendering internals completely.

For developers working with Vue and modern component-based architectures, there is value in a system that allows visual editing while preserving structured data, reusable components, and full control over rendering behavior.

---

# Proposed Solution

Page Vuilder proposes a visual page-building system where pages are composed from registered Vue components instead of raw HTML blocks.

Each page is represented as a structured JSON tree describing:

- Which Vue components are used
- Their props and configuration
- Their layout relationships
- Their nested children or slots

The rendering layer is responsible for converting this structured tree into server-rendered HTML using a custom Vue SSR pipeline.

This allows pages to remain:

- Structured
- Portable
- Typed
- Component-driven
- Headless CMS compatible

while still being editable through a visual interface.

---

# Core Idea

The core idea behind Page Vuilder is:

> Treat pages as structured trees of Vue components instead of HTML documents.

The visual builder becomes an interface for editing component trees, while the rendering runtime is responsible for producing the final SSR output.

This creates a cleaner separation between:

- Content
- Layout
- Rendering
- Components
- Editing tools

---

# Vision

Page Vuilder aims to become a developer-first experimental platform for exploring:

- Vue SSR internals
- Visual builder systems
- Structured rendering architectures
- Component-based page composition
- Runtime rendering pipelines

The long-term vision is not necessarily to compete with existing CMS platforms, but to better understand how modern rendering and visual editing systems work internally through hands-on experimentation and custom implementation.

---

# Key Principles

## Vue-First

The project is intentionally focused on Vue and Vue SSR rather than supporting multiple frontend frameworks.

---

## Component-Driven

Pages are built entirely from reusable Vue components.

---

## Structured Rendering

Pages are represented as structured data instead of raw HTML.

---

## Headless Architecture

The builder and rendering system should remain independent from any specific CMS platform.

---

## Learning Through Building

The project intentionally favors transparency and experimentation over abstraction and production-ready complexity.

---

# Target Outcome

A modern experimental Vue-based visual page builder capable of:

- Visually composing pages
- Managing structured component trees
- Rendering pages with custom SSR
- Editing typed component props
- Exploring runtime rendering architecture
- Serving as a learning platform for SSR and builder systems
