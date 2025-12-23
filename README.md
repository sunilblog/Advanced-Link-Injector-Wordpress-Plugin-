# Advanced-Link-Injector-Wordpress-Plugin-
Automatically injects and manages post links on static pages under specific headings based on categories. Features smart sync for Title/URL changes and automatic cleanup on Trash. Designed for high-traffic sites using the Classic Editor.

           <h2>📖 Complete Usage Manual & Features</h2>
            <p>This plugin automates the process of adding post links to static pages. Here is a summary of all active features to help you remember how it works:</p>

            <div style="background: #f0f6fb; border: 1px solid #007cba; padding: 15px; border-radius: 4px; margin: 15px 0;">
                <h4 style="margin-top:0;">🚀 Quick Start: How to Use</h4>
                <ol style="margin-bottom:0;">
                    <li><strong>Map Categories:</strong> In the table below, select a <strong>Post Category</strong> and the <strong>Target Page</strong> where links should appear.</li>
                    <li><strong>Set the Heading:</strong> Enter the exact HTML heading from your page (e.g., <code>&lt;h2&gt;Latest Updates&lt;/h2&gt;</code>). The plugin uses this to find the list.</li>
                    <li><strong>Prepare the List:</strong> Make sure your target page has a Bullet List (<code>&lt;ul&gt;</code>) started immediately after that heading.</li>
                    <li><strong>Choose Position:</strong> Select <strong>Top</strong> (newest first) or <strong>Bottom</strong> (oldest first) for the link placement.</li>
                    <li><strong>Go Live:</strong> Simply publish a new post in that category. The plugin does the rest!</li>
                </ol>
            </div>

            <p><strong>✅ Automated Synchronization:</strong><br>
            • <strong>Title & URL Updates:</strong> If you change the post title or the permalink (URL) later, the plugin detects the change and automatically updates the link on the target page.<br>
            • <strong>Category Swapping:</strong> If you move a post from Category A to Category B, the link will automatically disappear from the first heading and reappear under the new one (if both are mapped).</p>

           <p><strong>🛠️ Technical Standards:</strong><br>
            • <strong>SEO Friendly:</strong> Links are added with <code>target="_blank"</code> and <code>rel="noopener"</code> for security and performance.<br>
            • <strong>Safe Search:</strong> Handles special characters (like <code>&amp;</code>) automatically so search-and-replace never fails.<br>
            • <strong>ID Tracking (The <code>data-ali-id</code>):</strong> Each link contains a hidden <code>data-ali-id="XX"</code> attribute. <strong>Do not remove this!</strong> This ID is what allows the plugin to find and update the link even if you change the Title or URL of the post.</p>

            <p><strong>🔄 Status & Removal Logic:</strong><br>
            • <strong>Publishing:</strong> Links are added only when a post is Published.<br>
            • <strong>Trashing:</strong> Moving a post to Trash is the <strong>only</strong> way to automatically remove the link from pages.<br>
            • <strong>Drafts:</strong> Switching to "Draft" <u>will not</u> remove the link. This allows you to keep curated links active even if the post is hidden from the main blog.</p>
