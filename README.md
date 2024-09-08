# Next.js Tutorials

This repository contains a series of tutorials on Next.js, organized into four separate repositories for easy navigation and focused learning.

## Repositories

<h3>1. Routing (Next.js)</h3> 

- **Repository:** `nextjs-routing`

<details>

<summary>  Topics Covered: </summary>

  - Page Routing
  - Nested Routing
  - Dynamic Routing
  - Nested Dynamic Routing
  - Catch All Segments
  - Optional Catch All Segments
  - Not Found Page
  - File Collocation
  - Private Folder
  - Route Groups
  - Nested Layouts
  - Route Group Layout
  - Routing Metadata
  - Title Metadata
  - Link Component
  - Active Links
  - Navigating Pragmatically
  - Template
  - Loading UI
  - Error Handling
  - Recovering from Error
  - Handling Error in Nested Routes
  - Handling Error in Layout
  - Parallel Route
  - Learned Unmatched Routes
  - Conditional Routes
  - Intercepting Route
  - Parallel Intercepting Routes

</details>

<h3> 2. Route Handlers </h3>

- **Repository:** `nextjs-route-handlers`
<details>
<summary>  Topics Covered: </summary>

  - Route Handlers
  - Handling GET Requests
  - Handling POST Requests
  - Dynamic Route Handlers
  - Handling PATCH Requests
  - Handling DELETE Requests
  - URL Query Parameters
  - Redirects in Route Handlers
  - Headers in Route Handlers
  - Cookies in Route Handlers
  - Caching in Route Handlers
  - Middleware

</details>

 

<h3> 3. Rendering </h3>

- **Repository:** `nextjs-rendering`
<details>

<summary>  Topics Covered: </summary>

  - Server and Client Components
  - Dynamic Rendering
  - Streaming
  - Server-only Code
  - Third Party Packages
  - Context Providers
  - Client-only Code
  - Client Component Placement
  - Interleaving Server and Client Components

  </details>

<h3> 4.  Data Fetching </h3>

- **Repository:** `nextjs-data-fetching`
<details>

<summary>  Topics Covered: </summary>

  - Fetching Data with Server Components
  - Loading and Error States
  - JSON Server Setup
  - Caching Data
  - Opting Out of Caching
  - React
  - Time-based Data Revalidation
  - Client-side Data Fetching

</details>

---

## Using Submodules

To use these repositories as submodules within a parent repository, follow these steps:

### 1. **Clone the Parent Repository**

First, clone the parent repository where you want to include the submodules:

```bash
git clone <parent-repository-url>
cd <parent-repository-directory>
```

### 2. **Add Submodules**

Add each tutorial repository as a submodule. Replace `<submodule-repo-url>` with the actual URL of the submodule repository.

```bash
git submodule add <submodule-repo-url> path/to/submodule
```

For example:

```bash
git submodule add https://github.com/shyamexe/next-js-routing.git routing
git submodule add https://github.com/shyamexe/next-js-route-handlers.git route-handlers
git submodule add https://github.com/shyamexe/next-js-rendering.git rendering
git submodule add https://github.com/shyamexe/next-js-data-fetching.git data-fetching
```

### 3. **Initialize and Update Submodules**

After adding the submodules, initialize and update them:

```bash
git submodule update --init --recursive
```

### 4. **Working with Submodules**

To make changes within a submodule:

1. Navigate to the submodule directory:

   ```bash
   cd path/to/submodule
   ```

2. Make changes, commit them, and push to the submodule repository.

3. Update the submodule reference in the parent repository:

   ```bash
   cd ../
   git add path/to/submodule
   git commit -m "Updated submodule to latest commit"
   git push
   ```

### 5. **Cloning a Repository with Submodules**

When cloning a repository with submodules, use the `--recurse-submodules` option to automatically clone the submodules:

```bash
git clone --recurse-submodules <parent-repository-url>
```

### 6. **Updating Submodules**

To update your submodules to the latest commit from their respective repositories:

```bash
git submodule update --remote
```

---