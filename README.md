# Advanced-Link-Injector-Wordpress-Plugin-
Automatically injects and manages post links on static pages under specific headings based on categories. Features smart sync for Title/URL changes and automatic cleanup on Trash. Designed for sites using the Classic Editor.

          
---

## 📖 Complete Usage Manual & Features

This plugin automates the process of adding post links to static pages. Below is a full summary of all active features and how everything works. Designed for sites using the Classic Editor.

---

## 🚀 Quick Start: How to Use

1. **Map Categories**
   In the mapping table, select a **Post Category** and the **Target Page** where links should appear.

2. **Set the Heading**
   Enter the **exact HTML heading** from your target page, for example:

   ```html
   <h2>Latest Updates</h2>
   ```

   The plugin uses this heading to locate where links should be inserted.

3. **Prepare the List**
   Ensure the target page contains a bullet list (`<ul>`) **immediately after** the specified heading.

4. **Choose Position**
   Select where links should appear:

   * **Top** → Newest posts first
   * **Bottom** → Oldest posts first

5. **Go Live**
   Publish a new post in the mapped category — the plugin handles everything automatically.

---

## ✅ Automated Synchronization

* **Title & URL Updates**
  If you update a post title or permalink, the plugin automatically updates the corresponding link on the target page.

* **Category Swapping**
  If a post is moved from **Category A** to **Category B**:

  * The link is removed from the original mapped heading
  * The link is added under the new mapped heading (if configured)

---

## 🛠️ Technical Standards

* **SEO Friendly**
  Links are added with:

  ```html
  target="_blank" rel="noopener"
  ```

  for security and performance.

* **Safe Search & Replace**
  Special characters (such as `&`) are handled automatically, ensuring reliable updates.

* **ID Tracking (`data-ali-id`)**
  Each generated link includes a hidden attribute:

  ```html
  data-ali-id="XX"
  ```

  ⚠️ **Do not remove this attribute.**
  It allows the plugin to reliably locate and update links even after title or URL changes.

---

## 🔄 Status & Removal Logic

* **Publishing**
  Links are added **only** when a post is published.

* **Trashing**
  Moving a post to **Trash** is the **only** action that automatically removes its link from pages.

* **Drafts**
  Switching a post to **Draft** does **not** remove the link.
  This allows curated links to remain visible even if the post is hidden from the main blog.

