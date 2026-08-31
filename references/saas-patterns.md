# SaaS & Digital Product IA Patterns

Common structural patterns observed in mature SaaS and complex digital products.

## Tenant / Scope Hierarchy
Most multi-user products follow a variation of:

Account / Organization  
→ Workspace / Team  
→ Project / Object (the atomic unit of work)

Make the current scope always visible and explicit. Actions that affect runtime behavior should clearly show which scope they operate in.

## Navigation Layers
- **Global navigation** — Persistent product areas (rarely changes)
- **Local / Section navigation** — Within a major area
- **Contextual navigation** — Inside a specific object or record
- **Utility navigation** — Account, settings, help, notifications

## Organization Approaches
- **Object-oriented** — Group by the things users manage (Projects, Documents, Campaigns…)
- **Task-oriented** — Group by what users are trying to accomplish
- **Feature-oriented** — Group by product capabilities (often weakest for users)

Prefer object or task orientation when the mental model supports it. Pure feature lists scale poorly.

## Role & Permission Awareness
Different roles often need different entry points and visible navigation.  
Design a shared core structure, then layer role-specific views or entry points on top rather than creating completely separate products.

## Settings Separation
Keep distinct:
- Account-level settings
- Workspace / Team settings
- Project / Object settings

Mixing these levels is a frequent source of confusion.

## Progressive Disclosure
As products grow, primary navigation reaches cognitive limits.  
Use command palettes, search, and contextual actions to keep the main structure clean while still providing power-user access.
