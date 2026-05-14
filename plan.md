
You are building a production SaaS app called SEO Autopilot for WordPress.

The app is an AI-powered WordPress SEO automation SaaS.

The tool must:
- Connect to a user’s WordPress website
- Read posts, pages, categories, tags, media, authors, and SEO metadata
- Audit SEO issues
- Suggest keyword opportunities
- Generate SEO-optimized blog posts
- Optimize existing WordPress content
- Save generated content as WordPress drafts
- Optionally publish content after approval
- Create SEO reports with KPIs, charts, and tables
- Support future automation, billing, teams, and client reports

IMPORTANT BUILD ORDER:
1. Build the full frontend first.
2. Use mock data only during the frontend phase.
3. Do not build backend until the frontend is complete.
4. Do not connect WordPress until the backend phase.
5. Do not create unsafe auto-publishing in MVP.
6. Every page must be responsive.
7. Every major action must have loading, empty, error, and success states.
8. Every destructive or publishing action must require confirmation.
9. Use clean, modular components.
10. Do not create one huge file.
11. Do not leave broken buttons.
12. Do not expose credentials in the frontend.
13. Use TypeScript everywhere.
14. Avoid bugs, hydration errors, security mistakes, and unfinished flows.

TECH STACK:
- Next.js App Router
- TypeScript
- Tailwind CSS
- shadcn/ui
- Recharts
- TanStack Table
- React Hook Form
- Zod
- Lucide React icons
- next-themes for light/dark mode
- Prisma later for backend
- PostgreSQL later for database
- Redis/BullMQ later for background jobs
- Claude API later for AI generation
- WordPress REST API later for site access
- Stripe later for SaaS billing

USE AN OPEN-SOURCE SAAS OR DASHBOARD TEMPLATE FIRST:
- Use a Next.js + shadcn/ui SaaS/dashboard template.
- Keep the sidebar layout, dashboard structure, responsive shell, dark mode, auth/billing structure if available.
- Remove demo content.
- Replace demo content with SEO SaaS mock data.
- The design must look like a professional SaaS dashboard, not a simple admin panel.

DESIGN STYLE:
- Clean SaaS dashboard
- Premium UI/UX
- Responsive desktop/tablet/mobile
- Sidebar navigation
- Top navigation
- Site switcher
- User menu
- Breadcrumbs
- KPI cards
- Charts
- Data tables
- Filters
- Tabs
- Drawers
- Modals
- Toasts
- Skeleton loaders
- Empty states
- Error states
- Dark/light mode
- Strong spacing system
- Clear visual hierarchy
- Accessible contrast
- No lorem ipsum in final UI

MAIN ROUTES TO CREATE:
- /login
- /signup
- /dashboard
- /sites
- /sites/new
- /sites/[siteId]
- /sites/[siteId]/overview
- /sites/[siteId]/audit
- /sites/[siteId]/content
- /sites/[siteId]/keywords
- /sites/[siteId]/generator
- /sites/[siteId]/optimizer
- /sites/[siteId]/reports
- /sites/[siteId]/automation
- /sites/[siteId]/settings
- /billing
- /account
- /team
- /admin

PHASE 1 — PROJECT FOUNDATION:
- [ ] Initialize Next.js project from a SaaS/dashboard template
- [ ] Set up TypeScript
- [ ] Set up Tailwind CSS
- [ ] Set up shadcn/ui
- [ ] Set up app directory structure
- [ ] Set up global layout
- [ ] Set up dark/light mode
- [ ] Set up sidebar navigation
- [ ] Set up mobile sidebar
- [ ] Set up top navigation
- [ ] Set up breadcrumbs
- [ ] Set up toast system
- [ ] Set up reusable loading skeletons
- [ ] Set up reusable empty states
- [ ] Set up reusable error states
- [ ] Set up shared UI components
- [ ] Set up mock data folder
- [ ] Set up TypeScript types folder
- [ ] Set up service layer using mock data

PHASE 2 — TYPES AND MOCK DATA:
Create TypeScript types for:
- [ ] User
- [ ] Organization
- [ ] OrganizationMember
- [ ] Subscription
- [ ] Site
- [ ] WordPressConnection
- [ ] WordPressPost
- [ ] WordPressPage
- [ ] WordPressCategory
- [ ] WordPressTag
- [ ] WordPressMedia
- [ ] SeoAudit
- [ ] SeoIssue
- [ ] SeoScore
- [ ] Keyword
- [ ] KeywordCluster
- [ ] GeneratedArticle
- [ ] ContentOptimization
- [ ] AutomationRule
- [ ] AutomationJob
- [ ] Report
- [ ] ActivityLog
- [ ] UsageEvent

Create mock files:
- [ ] mock-users.ts
- [ ] mock-sites.ts
- [ ] mock-posts.ts
- [ ] mock-pages.ts
- [ ] mock-keywords.ts
- [ ] mock-audits.ts
- [ ] mock-issues.ts
- [ ] mock-generated-articles.ts
- [ ] mock-optimizations.ts
- [ ] mock-reports.ts
- [ ] mock-automation.ts
- [ ] mock-dashboard.ts
- [ ] mock-activity.ts

Create frontend services that currently return mock data:
- [ ] sites.service.ts
- [ ] posts.service.ts
- [ ] pages.service.ts
- [ ] keywords.service.ts
- [ ] audit.service.ts
- [ ] generator.service.ts
- [ ] optimizer.service.ts
- [ ] reports.service.ts
- [ ] automation.service.ts
- [ ] dashboard.service.ts
- [ ] billing.service.ts

PHASE 3 — GLOBAL APP LAYOUT:
Build:
- [ ] App shell
- [ ] Sidebar
- [ ] Mobile drawer sidebar
- [ ] Top bar
- [ ] Site switcher
- [ ] Account menu
- [ ] Notifications menu
- [ ] Command/search menu
- [ ] Breadcrumbs
- [ ] Page header component
- [ ] Section header component
- [ ] KPI card component
- [ ] Chart card component
- [ ] Data table wrapper
- [ ] Filter bar component
- [ ] Confirm modal component
- [ ] Detail drawer component
- [ ] Status badge component
- [ ] Severity badge component
- [ ] Score badge component
- [ ] Empty state component
- [ ] Loading skeleton component
- [ ] Error state component

PHASE 4 — MAIN DASHBOARD PAGE:
Route:
- /dashboard

Build dashboard with KPI cards:
- [ ] Total connected sites
- [ ] Total indexed posts
- [ ] Average SEO score
- [ ] Keywords tracked
- [ ] Posts generated this month
- [ ] Posts published this month
- [ ] Organic traffic estimate
- [ ] SEO issues found
- [ ] Content opportunities
- [ ] Automation jobs running

Build charts:
- [ ] Organic traffic trend chart
- [ ] SEO score trend chart
- [ ] Keyword ranking distribution chart
- [ ] Publishing activity chart
- [ ] Issue severity chart
- [ ] Top pages by opportunity chart

Build sections:
- [ ] Recent activity feed
- [ ] Top content opportunities table
- [ ] Critical issues summary
- [ ] Latest generated articles
- [ ] Automation status panel

Dashboard must:
- [ ] Be responsive
- [ ] Have loading state
- [ ] Have empty state
- [ ] Have error state
- [ ] Use mock data
- [ ] Have no broken buttons

PHASE 5 — SITES PAGE:
Routes:
- /sites
- /sites/new
- /sites/[siteId]

Build:
- [ ] Sites list page
- [ ] Connected site cards
- [ ] Site health badges
- [ ] Add new site button
- [ ] Empty state when no sites exist
- [ ] Search/filter sites
- [ ] Site status indicator
- [ ] Last sync indicator
- [ ] Site actions menu

Connect site page fields:
- [ ] Site name
- [ ] WordPress site URL
- [ ] WordPress admin username
- [ ] WordPress application password
- [ ] Permission mode
- [ ] Read-only mode
- [ ] Read and draft mode
- [ ] Full automation mode
- [ ] Test connection button
- [ ] Security explanation
- [ ] Application password instructions
- [ ] Save connection button

Connection UI states:
- [ ] Not connected
- [ ] Testing connection
- [ ] Connection success
- [ ] Invalid credentials
- [ ] WordPress REST API disabled
- [ ] SSL warning
- [ ] Permission warning
- [ ] Site already connected

PHASE 6 — SITE OVERVIEW PAGE:
Route:
- /sites/[siteId]/overview

Build KPIs:
- [ ] Total posts
- [ ] Total pages
- [ ] Total categories
- [ ] Total tags
- [ ] Average word count
- [ ] Average SEO score
- [ ] Missing meta descriptions
- [ ] Missing focus keywords
- [ ] Broken internal links
- [ ] Outdated posts
- [ ] Duplicate titles
- [ ] Duplicate meta descriptions

Build sections:
- [ ] Site health summary
- [ ] Latest synced content
- [ ] Best SEO opportunities
- [ ] Critical SEO issues
- [ ] Automation status
- [ ] Last sync status
- [ ] Suggested next actions

PHASE 7 — SEO AUDIT PAGE:
Route:
- /sites/[siteId]/audit

Audit categories:
- [ ] Title tag issues
- [ ] Meta description issues
- [ ] H1 issues
- [ ] Heading structure issues
- [ ] Thin content
- [ ] Missing internal links
- [ ] Missing external links
- [ ] Image alt text issues
- [ ] Keyword cannibalization
- [ ] Duplicate content
- [ ] Duplicate titles
- [ ] Duplicate meta descriptions
- [ ] Slug issues
- [ ] Schema markup issues
- [ ] Readability issues
- [ ] Content freshness issues
- [ ] Broken links
- [ ] Missing FAQ sections
- [ ] Missing CTA sections

Build:
- [ ] Audit summary cards
- [ ] SEO score chart
- [ ] Issue severity chart
- [ ] Issue category chart
- [ ] Audit table
- [ ] Issue detail drawer
- [ ] Fix with AI button
- [ ] Export report button

Audit table columns:
- [ ] Page/post title
- [ ] Type
- [ ] URL
- [ ] SEO score
- [ ] Issues count
- [ ] Critical issues
- [ ] Suggested action
- [ ] Last updated
- [ ] Status
- [ ] Actions

Filters:
- [ ] Search
- [ ] Filter by severity
- [ ] Filter by post/page type
- [ ] Filter by issue type
- [ ] Filter by status
- [ ] Sort by score
- [ ] Sort by severity
- [ ] Sort by last updated

PHASE 8 — CONTENT LIBRARY PAGE:
Route:
- /sites/[siteId]/content

Build content table with columns:
- [ ] Title
- [ ] Type
- [ ] Status
- [ ] Author
- [ ] Category
- [ ] Word count
- [ ] SEO score
- [ ] Focus keyword
- [ ] Traffic estimate
- [ ] Last updated
- [ ] Actions

Content actions:
- [ ] View content
- [ ] Analyze SEO
- [ ] Optimize with AI
- [ ] Generate meta description
- [ ] Generate FAQ
- [ ] Generate schema
- [ ] Add internal links
- [ ] Rewrite introduction
- [ ] Rewrite conclusion
- [ ] Save draft
- [ ] Publish update with confirmation

Build:
- [ ] Content preview drawer
- [ ] SEO issue panel
- [ ] Content filters
- [ ] Bulk actions UI
- [ ] Before/after comparison UI
- [ ] Save draft button
- [ ] Publish confirmation modal

PHASE 9 — KEYWORD RESEARCH PAGE:
Route:
- /sites/[siteId]/keywords

Build pages/sections:
- [ ] Keyword overview
- [ ] Keyword discovery
- [ ] Keyword clusters
- [ ] Keyword opportunities
- [ ] Content gaps
- [ ] Ranking tracker placeholder

Keyword discovery form:
- [ ] Seed keyword
- [ ] Target country
- [ ] Target language
- [ ] Search intent
- [ ] Niche
- [ ] Generate ideas button

Keyword table columns:
- [ ] Keyword
- [ ] Search intent
- [ ] Search volume
- [ ] Difficulty
- [ ] CPC
- [ ] Competition
- [ ] Current ranking URL
- [ ] Suggested content type
- [ ] Priority score
- [ ] Status
- [ ] Actions

Keyword actions:
- [ ] Add to content plan
- [ ] Create content brief
- [ ] Send to blog generator
- [ ] Assign to existing post
- [ ] Export CSV

Build:
- [ ] Keyword opportunity table
- [ ] Keyword cluster cards
- [ ] Search intent badges
- [ ] Priority score UI
- [ ] CSV export UI
- [ ] Keyword detail drawer

PHASE 10 — BLOG GENERATOR PAGE:
Route:
- /sites/[siteId]/generator

Generator form fields:
- [ ] Target site
- [ ] Main topic
- [ ] Focus keyword
- [ ] Secondary keywords
- [ ] Search intent
- [ ] Target audience
- [ ] Tone of voice
- [ ] Language
- [ ] Country/region
- [ ] Word count
- [ ] Content type
- [ ] Include FAQ
- [ ] Include schema
- [ ] Include internal links
- [ ] Include external links
- [ ] Include CTA
- [ ] Auto-generate image prompt
- [ ] Publishing status: SaaS draft, WordPress draft, scheduled, published

Generated result sections:
- [ ] SEO title
- [ ] Meta description
- [ ] Slug
- [ ] Excerpt
- [ ] Outline
- [ ] Full article
- [ ] FAQ section
- [ ] Schema markup
- [ ] Image prompts
- [ ] Internal link suggestions
- [ ] External link suggestions
- [ ] SEO checklist
- [ ] Readability score
- [ ] Publish preview

Build:
- [ ] Blog generator form
- [ ] Generated article preview
- [ ] SEO metadata panel
- [ ] Outline viewer
- [ ] FAQ preview
- [ ] Schema preview
- [ ] Internal links panel
- [ ] Publish settings panel
- [ ] Generation loading screen
- [ ] Regeneration controls
- [ ] Save draft action
- [ ] Publish action disabled until backend exists
- [ ] Confirmation modal for publish actions

PHASE 11 — CONTENT OPTIMIZER PAGE:
Route:
- /sites/[siteId]/optimizer

Optimizer flow:
- [ ] Select existing post
- [ ] Show current content
- [ ] Show current SEO score
- [ ] Show detected SEO issues
- [ ] Generate recommendations
- [ ] Accept/reject recommendations
- [ ] Generate updated version
- [ ] Preview changes
- [ ] Save as draft
- [ ] Publish update with confirmation

Optimization features:
- [ ] Improve title
- [ ] Improve meta description
- [ ] Improve intro
- [ ] Improve headings
- [ ] Add missing keyword sections
- [ ] Add FAQ
- [ ] Add schema
- [ ] Add internal links
- [ ] Add image alt text
- [ ] Improve readability
- [ ] Update outdated facts
- [ ] Expand thin sections
- [ ] Improve CTA

Build:
- [ ] Post selector
- [ ] SEO score card
- [ ] Recommendations list
- [ ] Before/after comparison
- [ ] Accept/reject controls
- [ ] Updated article preview
- [ ] Publish confirmation modal

PHASE 12 — REPORTS PAGE:
Route:
- /sites/[siteId]/reports

Report types:
- [ ] Weekly SEO report
- [ ] Monthly SEO report
- [ ] Content performance report
- [ ] Keyword opportunity report
- [ ] Site audit report
- [ ] Automation activity report
- [ ] Client report PDF placeholder

Report KPIs:
- [ ] SEO score change
- [ ] New issues found
- [ ] Issues fixed
- [ ] Posts published
- [ ] Posts optimized
- [ ] Keywords added
- [ ] Traffic estimate change
- [ ] Top opportunities
- [ ] Content decay warnings

Build:
- [ ] Report dashboard
- [ ] Report filters
- [ ] Report preview
- [ ] Export PDF button
- [ ] Export CSV button
- [ ] Schedule email report UI
- [ ] Report history table

PHASE 13 — AUTOMATION PAGE:
Route:
- /sites/[siteId]/automation

Automation rules:
- [ ] Auto-generate blog posts weekly
- [ ] Auto-update old content
- [ ] Auto-generate meta descriptions
- [ ] Auto-add FAQ schema
- [ ] Auto-detect outdated content
- [ ] Auto-create drafts only
- [ ] Auto-publish after approval
- [ ] Full auto-publish mode later

Safety settings:
- [ ] Require manual approval
- [ ] Publish as draft only
- [ ] Limit posts per day
- [ ] Limit posts per week
- [ ] Exclude categories
- [ ] Exclude pages
- [ ] Never overwrite existing content without backup
- [ ] Keep revision history
- [ ] Notify before publishing

Build:
- [ ] Automation rule builder
- [ ] Frequency selector
- [ ] Safety settings panel
- [ ] Approval workflow UI
- [ ] Automation log table
- [ ] Pause/resume controls
- [ ] Delete rule confirmation modal

PHASE 14 — SITE SETTINGS PAGE:
Route:
- /sites/[siteId]/settings

Settings sections:
- [ ] WordPress connection
- [ ] Permission mode
- [ ] Default author
- [ ] Default category
- [ ] Default tags
- [ ] Default post status
- [ ] Default language
- [ ] Default tone
- [ ] SEO plugin compatibility
- [ ] Sitemap URL
- [ ] Robots.txt status
- [ ] Danger zone

SEO plugin compatibility:
- [ ] Yoast SEO
- [ ] Rank Math
- [ ] All in One SEO
- [ ] SEOPress
- [ ] Native WordPress fields

Build:
- [ ] Settings tabs
- [ ] Connection settings
- [ ] Publishing defaults
- [ ] SEO plugin selector
- [ ] Danger zone
- [ ] Disconnect site button with confirmation

PHASE 15 — BILLING PAGE:
Route:
- /billing

Plans:
Free:
- 1 site
- 20 posts scanned
- 3 AI generations/month
- Draft only
- No automation

Starter:
- 3 sites
- 500 posts scanned
- 50 AI generations/month
- WordPress draft publishing
- Basic reports

Pro:
- 10 sites
- 5,000 posts scanned
- 300 AI generations/month
- Auto-publishing after approval
- Advanced reports
- Keyword API integrations

Agency:
- Multiple client sites
- Team members
- White-label reports
- Client dashboards
- Priority queue

Build:
- [ ] Pricing cards
- [ ] Current plan badge
- [ ] Usage meters
- [ ] Billing history placeholder
- [ ] Upgrade buttons
- [ ] Cancel plan UI
- [ ] Stripe integration placeholder

PHASE 16 — ACCOUNT AND TEAM PAGES:
Routes:
- /account
- /team

Account:
- [ ] Profile settings
- [ ] Email settings
- [ ] Password/security placeholder
- [ ] Notification preferences
- [ ] API usage summary

Team:
- [ ] Team members table
- [ ] Invite member UI
- [ ] Role selector
- [ ] Remove member confirmation
- [ ] Roles: owner, admin, editor, viewer

PHASE 17 — FRONTEND QUALITY CHECK:
Before backend, verify:
- [ ] No TypeScript errors
- [ ] No ESLint errors
- [ ] No unused imports
- [ ] No console errors
- [ ] No hydration errors
- [ ] All routes load
- [ ] All navigation links work
- [ ] Mobile sidebar works
- [ ] Tables are responsive
- [ ] Forms validate correctly
- [ ] Empty states exist
- [ ] Loading states exist
- [ ] Error states exist
- [ ] Dark mode works
- [ ] Light mode works
- [ ] Buttons have disabled states
- [ ] Destructive actions require confirmation
- [ ] Publish actions require confirmation
- [ ] Mock data is separated from UI components
- [ ] No backend code is required for frontend phase
- [ ] No real credentials are used

ONLY AFTER FRONTEND IS COMPLETE, START BACKEND.

PHASE 18 — BACKEND FOUNDATION:
Use:
- Next.js API route handlers
- TypeScript
- Prisma
- PostgreSQL
- Zod
- Auth provider
- Encrypted credential storage
- WordPress REST API
- Claude API
- Redis/BullMQ later

Create database tables:
- [ ] users
- [ ] organizations
- [ ] organization_members
- [ ] sites
- [ ] wordpress_credentials
- [ ] wordpress_posts
- [ ] wordpress_pages
- [ ] wordpress_categories
- [ ] wordpress_tags
- [ ] seo_audits
- [ ] seo_issues
- [ ] keywords
- [ ] keyword_clusters
- [ ] generated_articles
- [ ] content_optimizations
- [ ] automation_rules
- [ ] automation_jobs
- [ ] reports
- [ ] subscriptions
- [ ] usage_events
- [ ] audit_logs

PHASE 19 — BACKEND API ROUTES:
Site routes:
- [ ] POST /api/sites/connect
- [ ] GET /api/sites
- [ ] GET /api/sites/:siteId
- [ ] PATCH /api/sites/:siteId
- [ ] DELETE /api/sites/:siteId
- [ ] POST /api/sites/:siteId/test-connection
- [ ] POST /api/sites/:siteId/sync

WordPress content routes:
- [ ] GET /api/sites/:siteId/posts
- [ ] GET /api/sites/:siteId/pages
- [ ] GET /api/sites/:siteId/categories
- [ ] GET /api/sites/:siteId/tags
- [ ] POST /api/sites/:siteId/posts
- [ ] PATCH /api/sites/:siteId/posts/:postId
- [ ] POST /api/sites/:siteId/posts/:postId/publish
- [ ] POST /api/sites/:siteId/posts/:postId/backup

SEO routes:
- [ ] POST /api/sites/:siteId/audit
- [ ] GET /api/sites/:siteId/audit
- [ ] GET /api/sites/:siteId/issues
- [ ] POST /api/sites/:siteId/issues/:issueId/fix

Keyword routes:
- [ ] POST /api/sites/:siteId/keywords/discover
- [ ] GET /api/sites/:siteId/keywords
- [ ] POST /api/sites/:siteId/keywords/cluster
- [ ] POST /api/sites/:siteId/keywords/:keywordId/brief

AI content routes:
- [ ] POST /api/sites/:siteId/generate/article
- [ ] POST /api/sites/:siteId/generate/meta
- [ ] POST /api/sites/:siteId/generate/faq
- [ ] POST /api/sites/:siteId/generate/schema
- [ ] POST /api/sites/:siteId/optimize/post/:postId

Automation routes:
- [ ] GET /api/sites/:siteId/automation/rules
- [ ] POST /api/sites/:siteId/automation/rules
- [ ] PATCH /api/sites/:siteId/automation/rules/:ruleId
- [ ] DELETE /api/sites/:siteId/automation/rules/:ruleId
- [ ] GET /api/sites/:siteId/automation/jobs
- [ ] POST /api/sites/:siteId/automation/jobs/:jobId/cancel

Reports routes:
- [ ] GET /api/sites/:siteId/reports
- [ ] POST /api/sites/:siteId/reports/generate
- [ ] GET /api/sites/:siteId/reports/:reportId
- [ ] POST /api/sites/:siteId/reports/:reportId/export

PHASE 20 — WORDPRESS INTEGRATION:
Authentication:
- [ ] Use WordPress Application Passwords
- [ ] Create WordPress client class
- [ ] Validate WordPress URL
- [ ] Normalize trailing slashes
- [ ] Test /wp-json
- [ ] Test /wp-json/wp/v2/users/me
- [ ] Store username
- [ ] Encrypt application password
- [ ] Never log credentials
- [ ] Add timeout handling
- [ ] Add retry handling
- [ ] Add rate limiting

Read operations:
- [ ] Fetch posts
- [ ] Fetch pages
- [ ] Fetch categories
- [ ] Fetch tags
- [ ] Fetch media
- [ ] Fetch authors
- [ ] Fetch revisions if available
- [ ] Handle pagination
- [ ] Handle draft/private posts based on permission
- [ ] Store synced content locally

Write operations:
- [ ] Create draft post
- [ ] Publish post
- [ ] Update post
- [ ] Update title
- [ ] Update slug
- [ ] Update excerpt
- [ ] Update content
- [ ] Update categories
- [ ] Update tags
- [ ] Upload featured image later
- [ ] Add backup before update
- [ ] Add rollback support

WordPress safety:
- [ ] Never overwrite live content without backup
- [ ] Keep original content snapshot
- [ ] Store generated changes separately
- [ ] Require explicit approval for destructive changes
- [ ] Add dry-run mode
- [ ] Add draft-only mode
- [ ] Add full automation mode only for paid/admin users

PHASE 21 — AI CONTENT ENGINE:
Create Claude prompt modules:
- [ ] Site niche detection
- [ ] SEO audit
- [ ] Keyword suggestions
- [ ] Keyword clustering
- [ ] Content brief generation
- [ ] Blog outline
- [ ] Full article generation
- [ ] Meta title generation
- [ ] Meta description generation
- [ ] FAQ generation
- [ ] Schema generation
- [ ] Internal link suggestions
- [ ] Content optimization
- [ ] Content freshness update
- [ ] Readability improvement

AI output rules:
- [ ] Force structured JSON
- [ ] Validate AI output with Zod
- [ ] Retry if JSON invalid
- [ ] Sanitize generated HTML
- [ ] Strip unsafe scripts
- [ ] Prevent prompt injection from WordPress content
- [ ] Add max token limits
- [ ] Add usage tracking
- [ ] Add cost tracking

Expected article JSON:
{
  "seoTitle": "",
  "metaDescription": "",
  "slug": "",
  "focusKeyword": "",
  "secondaryKeywords": [],
  "outline": [],
  "articleHtml": "",
  "faq": [],
  "schemaJsonLd": {},
  "internalLinks": [],
  "externalLinks": [],
  "seoChecklist": [],
  "readabilityScore": 0,
  "seoScore": 0
}

PHASE 22 — SEO AUDIT ENGINE:
Deterministic checks:
- [ ] Title length
- [ ] Missing title
- [ ] Meta description length
- [ ] Missing meta description
- [ ] Missing H1
- [ ] Multiple H1s
- [ ] Heading order
- [ ] Word count
- [ ] Slug length
- [ ] Missing image alt text
- [ ] Internal link count
- [ ] External link count
- [ ] Broken links later
- [ ] Duplicate titles
- [ ] Duplicate meta descriptions
- [ ] Old content detection
- [ ] Empty categories/tags
- [ ] Missing schema

AI checks:
- [ ] Search intent match
- [ ] Content depth
- [ ] Readability
- [ ] Topical coverage
- [ ] Missing subtopics
- [ ] Content quality
- [ ] CTA quality
- [ ] FAQ opportunities
- [ ] Semantic keyword suggestions

SEO score formula:
- Technical SEO: 25 points
- On-page SEO: 25 points
- Content quality: 25 points
- Internal linking: 15 points
- Freshness: 10 points

PHASE 23 — KEYWORD SYSTEM:
MVP keyword system:
- [ ] Let user enter seed keywords
- [ ] Let AI suggest keyword ideas
- [ ] Let AI classify search intent
- [ ] Let AI group into clusters
- [ ] Let user manually add search volume/difficulty
- [ ] Let generated content use selected keywords

Production keyword integrations later:
- [ ] Google Search Console
- [ ] DataForSEO
- [ ] Semrush
- [ ] Ahrefs
- [ ] SerpAPI
- [ ] Google Keyword Planner if available

Priority score formula:
Priority = Business Value + Search Intent Fit + Content Gap + Ranking Opportunity - Difficulty

PHASE 24 — PUBLISHING SYSTEM:
Publishing modes:
- [ ] Save as SaaS draft only
- [ ] Save as WordPress draft
- [ ] Schedule in WordPress
- [ ] Publish immediately
- [ ] Update existing post
- [ ] Create revision backup
- [ ] Rollback update

Before publishing, validate:
- [ ] Title
- [ ] Slug
- [ ] Meta description
- [ ] Content length
- [ ] Unsafe HTML
- [ ] Internal links
- [ ] Category
- [ ] Tags
- [ ] Duplicate topic
- [ ] User permission
- [ ] Usage limits
- [ ] Backup snapshot

PHASE 25 — SECURITY:
Authentication and authorization:
- [ ] Add protected routes
- [ ] Add organization membership
- [ ] Add RBAC
- [ ] Roles: owner, admin, editor, viewer
- [ ] Check permission on every API route
- [ ] Prevent cross-tenant data access
- [ ] Add middleware protection

Credentials:
- [ ] Encrypt WordPress application passwords
- [ ] Use server-only environment variables
- [ ] Never send stored credentials to frontend
- [ ] Never log credentials
- [ ] Rotate encryption key carefully
- [ ] Delete credentials on disconnect

API security:
- [ ] Validate all inputs with Zod
- [ ] Add rate limiting
- [ ] Add CSRF protection where needed
- [ ] Add request size limits
- [ ] Add HTML sanitization
- [ ] Add SSRF protection for WordPress URLs
- [ ] Block localhost/private IP WordPress URLs
- [ ] Block file URLs
- [ ] Block non-http protocols
- [ ] Add audit logs for publish/update actions

AI security:
- [ ] Treat WordPress content as untrusted input
- [ ] Add prompt injection guard
- [ ] Do not allow site content to override system instructions
- [ ] Validate AI JSON output
- [ ] Sanitize generated HTML
- [ ] Add human approval mode

PHASE 26 — BACKGROUND JOBS:
Use background jobs for:
- [ ] Sync WordPress content
- [ ] Run SEO audit
- [ ] Generate article
- [ ] Optimize article
- [ ] Generate report
- [ ] Publish scheduled post
- [ ] Update old content
- [ ] Check automation rules
- [ ] Fetch keyword data
- [ ] Send email report

Job safety:
- [ ] Job status
- [ ] Retries
- [ ] Failure logs
- [ ] Cancellation
- [ ] Progress percentage
- [ ] User notifications
- [ ] Queue rate limits

PHASE 27 — BILLING:
Add Stripe:
- [ ] Stripe checkout
- [ ] Stripe customer portal
- [ ] Subscription table
- [ ] Usage limits
- [ ] Plan enforcement middleware
- [ ] Failed payment handling
- [ ] Trial system
- [ ] Upgrade prompts

PHASE 28 — REPORTS AND EXPORTS:
Reports:
- [ ] Site health report
- [ ] SEO audit report
- [ ] Content opportunity report
- [ ] Keyword report
- [ ] Automation report
- [ ] Monthly client report

Exports:
- [ ] CSV
- [ ] PDF
- [ ] HTML report
- [ ] Email report

Report generation:
- [ ] Generate report data from database
- [ ] Generate charts
- [ ] Generate AI summary
- [ ] Include recommendations
- [ ] Include completed work
- [ ] Include next actions

PHASE 29 — TESTING:
Frontend testing:
- [ ] Test all pages load
- [ ] Test mobile layout
- [ ] Test forms
- [ ] Test validation
- [ ] Test dark mode
- [ ] Test tables
- [ ] Test charts
- [ ] Test empty states
- [ ] Test loading states
- [ ] Test error states

Backend testing:
- [ ] Test auth
- [ ] Test RBAC
- [ ] Test site connection
- [ ] Test WordPress read
- [ ] Test WordPress write
- [ ] Test credential encryption
- [ ] Test SEO audit
- [ ] Test AI generation
- [ ] Test publishing
- [ ] Test billing
- [ ] Test usage limits

Security testing:
- [ ] Test cross-tenant access
- [ ] Test invalid site URLs
- [ ] Test localhost/private IP blocking
- [ ] Test XSS in generated content
- [ ] Test malicious WordPress content
- [ ] Test rate limits
- [ ] Test credential leaks
- [ ] Test logs for sensitive data

PHASE 30 — DEPLOYMENT:
Environments:
- [ ] Local
- [ ] Development
- [ ] Staging
- [ ] Production

Environment variables:
- [ ] DATABASE_URL
- [ ] AUTH_SECRET
- [ ] ENCRYPTION_KEY
- [ ] ANTHROPIC_API_KEY
- [ ] STRIPE_SECRET_KEY
- [ ] STRIPE_WEBHOOK_SECRET
- [ ] REDIS_URL
- [ ] SENTRY_DSN
- [ ] NEXT_PUBLIC_APP_URL

Deployment tasks:
- [ ] Deploy frontend/API to Vercel
- [ ] Deploy PostgreSQL
- [ ] Deploy Redis
- [ ] Configure environment variables
- [ ] Configure Stripe webhook
- [ ] Configure cron jobs
- [ ] Configure error tracking
- [ ] Configure analytics
- [ ] Test production WordPress connection
- [ ] Test production publishing with draft mode first

MVP SCOPE:
Build first:
- [ ] User login
- [ ] Dashboard UI
- [ ] Connect WordPress site UI
- [ ] WordPress connection backend
- [ ] Read posts/pages
- [ ] SEO audit
- [ ] Blog generator
- [ ] Save generated article as WordPress draft
- [ ] Content optimizer
- [ ] Reports page
- [ ] Basic billing limit

Do not build in MVP:
- [ ] Full auto-publishing
- [ ] Competitor scraping
- [ ] Advanced rank tracking
- [ ] White-label reports
- [ ] Agency client portal
- [ ] Full AI image generation
- [ ] Advanced backlink tracking

BIGGEST MISTAKES TO AVOID:
- Do not build backend before frontend flow is complete.
- Do not give full WordPress write access without safety modes.
- Do not store WordPress passwords unencrypted.
- Do not auto-publish without approval in MVP.
- Do not rely only on AI for SEO audits.
- Do not put all UI in one component.
- Do not skip mobile responsiveness.
- Do not skip empty/loading/error states.
- Do not publish AI content without preview.
- Do not trust AI JSON without validation.
- Do not allow WordPress content to control AI prompts.
- Do not forget backups before updating posts.
- Do not expose secrets to the client.
- Do not create broken routes or buttons.

FINAL BUILD ORDER:
1. Clone a Next.js + shadcn dashboard/SaaS template.
2. Remove demo content.
3. Build all frontend screens using mock SEO data.
4. Polish responsive UI.
5. Add database/auth.
6. Add WordPress connection.
7. Add content sync.
8. Add SEO audit.
9. Add Claude generation.
10. Add WordPress draft publishing.
11. Add reports.
12. Add billing.
13. Add automation safely.
a# SEO Autopilot - Post Analysis & Improvement Plan

## Goal
Connect to WordPress posts, analyze SEO issues, improve posts for high SEO scores using AI, and integrate Nvidia NIM API.

## Error Fix
**Error**: `Unexpected content chunk type tool_reference. We only support 'text', 'image_url', and, 'video_url'.`

**Root Cause**: This error occurs when the AI API returns a `tool_reference` content type that the client doesn't handle. This typically happens with:
1. Anthropic Claude API when tool definitions are incorrectly formatted
2. Nvidia NIM API when using vision/image tools with incompatible response formats
3. Streaming responses with tool use that aren't properly handled

**Fix Strategy**:
- Filter out non-text content chunks in API responses
- Add proper content chunk type validation before processing
- Use text-only mode for initial implementation
- Update streaming parser to skip unsupported chunk types

---

## Phase 1: WordPress Post Integration

### 1.1 Enhanced WordPress API Routes
**Files to create/modify**:
- `src/app/api/wordpress/posts/route.ts` - Fetch posts with SEO data
- `src/app/api/wordpress/posts/[postId]/route.ts` - Get single post
- `src/lib/services/posts.service.ts` - Post management service

**Endpoints needed**:
```
GET /api/wordpress/posts?siteId=xxx&per_page=50&status=publish,draft
GET /api/wordpress/posts/:postId?siteId=xxx
POST /api/wordpress/posts/:postId/update?siteId=xxx
```

### 1.2 Post Fetching with SEO Metadata
**WordPress REST API endpoints**:
- `/wp-json/wp/v2/posts` - Get posts
- Include `_embed` for featured media and author
- Request Yoast/Rank Math SEO meta fields if available

**Add to wordpress.ts**:
```typescript
export async function fetchWordPressPostsWithSeo(
  siteUrl: string,
  username: string,
  applicationPassword: string,
  options?: {
    perPage?: number;
    page?: number;
    status?: string;
    search?: string;
    categories?: number;
    tags?: number;
  }
) {
  // Fetch posts with SEO data
}
```

---

## Phase 2: SEO Analysis Engine

### 2.1 SEO Analysis Service
**File**: `src/lib/services/seo-analyzer.service.ts`

**Analysis Categories**:

**Technical SEO** (25 points):
- Title tag: presence, length (30-60 chars), keyword placement
- Meta description: presence, length (120-160 chars), keyword placement
- H1: presence, count (exactly 1), keyword in H1
- Heading hierarchy: H2-H6 order
- URL slug: length, readability, keyword

**On-Page SEO** (25 points):
- Focus keyword: presence in title, first paragraph, headings, URL
- Keyword density: 1-3% range
- Content length: minimum 300 words, optimal 1000+
- Images: alt text presence, file names
- Internal links: count, anchor text
- External links: authority sources

**Content Quality** (25 points):
- Readability: Flesch-Kincaid score (60+)
- Content depth: subtopic coverage
- Freshness: last updated date
- Duplicate content: title/meta checks
- Paragraph structure: short paragraphs, lists

**Internal Linking** (15 points):
- Links to other posts
- Anchor text quality
- Orphan content detection

**Freshness** (10 points):
- Content age
- Update frequency

### 2.2 SEO Score Calculator
```typescript
interface SeoAnalysisResult {
  postId: number;
  title: string;
  url: string;
  seoScore: number;
  scores: {
    technical: number;
    onPage: number;
    content: number;
    internalLinking: number;
    freshness: number;
  };
  issues: SeoIssue[];
  recommendations: string[];
  wordCount: number;
  focusKeyword?: string;
}
```

### 2.3 Issues Detection
**Critical Issues**:
- Missing title tag
- Missing meta description
- Missing H1
- Multiple H1s
- No focus keyword
- Thin content (<300 words)

**Warnings**:
- Title too long/short
- Meta description too long/short
- Keyword not in first paragraph
- Missing internal links
- Missing image alt text

---

## Phase 3: AI Post Improvement Engine

### 3.1 AI Provider Setup

#### Option A: Anthropic Claude (if already working)
- Continue using existing implementation
- Fix tool_reference error by filtering content types

#### Option B: Nvidia NIM Integration
**API Endpoint**: `https://integrate.api.nvidia.com/v1/chat/completions`

**Setup**:
1. Get API key from https://build.nvidia.com/
2. Add to environment: `NIM_API_KEY`

**Implementation**:
```typescript
// src/lib/ai/nvidia-nim.ts
export async function generateWithNim(
  prompt: string,
  model: string = 'nvidia/llama-3.1-nemotron-70b-instruct',
  options?: {
    temperature?: number;
    maxTokens?: number;
  }
) {
  const response = await fetch('https://integrate.api.nvidia.com/v1/chat/completions', {
    method: 'POST',
    headers: {
      'Authorization': `Bearer ${process.env.NIM_API_KEY}`,
      'Content-Type': 'application/json',
    },
    body: JSON.stringify({
      model,
      messages: [{ role: 'user', content: prompt }],
      temperature: options?.temperature ?? 0.7,
      max_tokens: options?.maxTokens ?? 2048,
      stream: false, // Avoid tool_reference issue with streaming
    }),
  });

  if (!response.ok) {
    throw new Error(`NIM API error: ${response.status}`);
  }

  return response.json();
}
```

### 3.2 Fix tool_reference Error
```typescript
function filterContentChunks(content: any): string {
  if (Array.isArray(content)) {
    return content
      .filter((chunk) => {
        // Only allow text, image_url, video_url
        const type = chunk.type || chunk;
        return ['text', 'image_url', 'video_url'].includes(type);
      })
      .map((chunk) => {
        // Extract text from allowed types
        if (chunk.type === 'text' || typeof chunk === 'string') {
          return chunk.text || chunk;
        }
        return '';
      })
      .join('');
  }
  return content;
}
```

### 3.3 Post Improvement Prompts

**Title Optimization**:
```
Analyze this post title and SEO metadata:
Title: {title}
Current meta description: {metaDescription}
Focus keyword: {focusKeyword}

Improve the title to:
1. Include focus keyword near the beginning
2. Be 30-60 characters
3. Be compelling and click-worthy
4. Match search intent

Return JSON: { "improvedTitle": "...", "reason": "..." }
```

**Meta Description Optimization**:
```
Write an optimized meta description:
Title: {title}
Content excerpt: {excerpt}
Focus keyword: {focusKeyword}

Requirements:
1. 120-160 characters
2. Include focus keyword
3. Include CTA words (learn, discover, get, etc.)
4. Match title promise

Return JSON: { "metaDescription": "...", "reason": "..." }
```

**Content Improvement**:
```
Improve this content for SEO:

Focus keyword: {focusKeyword}
Secondary keywords: {secondaryKeywords}

Current title: {title}
Current content: {content}

SEO requirements:
1. Add keyword in first paragraph
2. Use H2-H3 headings with keywords
3. Add internal link placeholders [link:page-slug]
4. Add external authority links
5. Short paragraphs (2-3 sentences)
6. Use bullet lists where appropriate
7. Add FAQ section if valuable

Return JSON with improved content and specific recommendations.
```

**Add Missing SEO Elements**:
```
Analyze and fix SEO issues:

Post URL: {url}
Current issues: {issues}

For each critical issue, provide:
1. Specific fix
2. Example code/snippet
3. Priority (high/medium/low)

Return JSON: { "fixes": [...] }
```

---

## Phase 4: MCP Dev Chrome Integration

### 4.1 MCP Server Setup
**MCP Server**: `@modelcontextprotocol/server-playwright`

**Configuration** (`.mcp.json` or project config):
```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@modelcontextprotocol/server-playwright"]
    }
  }
}
```

### 4.2 Use Cases for SEO Tool
- **Live Site Analysis**: Visit WordPress site and analyze rendered content
- **Structured Data Validation**: Check schema.org markup in browser
- **JavaScript SEO Check**: Analyze JS-rendered content
- **Sitemap Analysis**: Parse XML sitemaps
- **Competitor Analysis**: Analyze competitor SERP appearances

### 4.2 Chrome DevTools Integration
```typescript
// MCP Chrome usage for SEO
async function analyzeLivePageSEO(url: string) {
  // Navigate to page
  // Get page content
  // Analyze meta tags
  // Check structured data
  // Capture screenshots
  // Analyze rendered HTML vs source
}
```

---

## Phase 5: Testing & Validation

### 5.1 Test Scenarios

**Test 1: Post Fetching**
- Connect to WordPress site
- Fetch posts with different statuses
- Verify SEO metadata is included
- Test pagination

**Test 2: SEO Analysis**
- Analyze posts with various SEO issues
- Verify score calculation accuracy
- Check issue detection
- Validate recommendations

**Test 3: AI Improvement**
- Generate title improvements
- Generate meta description improvements
- Generate content improvements
- Verify output quality
- Test without tool_reference errors

**Test 4: Nvidia NIM Integration**
- Connect with API key
- Test text generation
- Verify response format
- Handle errors gracefully

**Test 5: Publishing**
- Save as draft to WordPress
- Verify content updates
- Test backup creation

### 5.2 Quality Metrics
- SEO score improvement: Target +20 points
- Processing time: <5 seconds per post
- Error rate: <1%
- User satisfaction: Manual review of improvements

---

## Implementation Order

### Week 1: Foundation
1. ✅ Review existing code structure
2. Enhance WordPress API routes for post fetching
3. Create SEO analysis service (deterministic checks)
4. Add SEO types

### Week 2: AI Integration
1. Fix tool_reference error in current AI calls
2. Add Nvidia NIM API integration
3. Create improvement prompts
4. Test both Claude and NIM

### Week 3: MCP & Testing
1. Configure MCP Playwright server
2. Implement live analysis features
3. End-to-end testing
4. Bug fixes

### Week 4: Polish
1. UI improvements for SEO results display
2. Performance optimization
3. Documentation

---

## Files to Create/Modify

### New Files
- `src/lib/services/seo-analyzer.service.ts` - SEO analysis engine
- `src/lib/services/post-improver.service.ts` - AI-powered improvements
- `src/lib/ai/nvidia-nim.ts` - Nvidia NIM integration
- `src/lib/ai/claude.ts` - Fixed Claude integration
- `src/app/api/seo/analyze/route.ts` - Analyze endpoint
- `src/app/api/seo/improve/route.ts` - Improve endpoint

### Modify Existing
- `src/lib/services/index.ts` - Add new services
- `src/lib/types/index.ts` - Add SEO result types
- `src/app/(dashboard)/sites/[siteId]/content/page.tsx` - Add analyze button

---

## API Keys Needed

```
# Required
NIM_API_KEY=nvapi-xxxxxxx  # From https://build.nvidia.com/

# Optional (if using Claude)
ANTHROPIC_API_KEY=sk-ant-xxxxx
```

---

## Error Handling

### tool_reference Error Prevention
```typescript
// In API calls, add content filtering
async function safeAIRequest(prompt: string) {
  try {
    const response = await makeAIRequest(prompt);
    // Filter content before processing
    const safeContent = filterContentChunks(response.content);
    return parseJSON(safeContent);
  } catch (error) {
    if (error.message.includes('tool_reference')) {
      // Retry with text-only mode
      return makeTextOnlyRequest(prompt);
    }
    throw error;
  }
}
```

### NIM API Errors
- 401: Invalid API key
- 429: Rate limit - implement backoff
- 500: Server error - retry with exponential backoff

---

## Success Criteria

1. ✅ Can fetch and display WordPress posts with SEO data
2. ✅ Can analyze posts and generate SEO scores
3. ✅ Can detect and categorize SEO issues
4. ✅ Can generate AI-powered improvements
5. ✅ Can save improvements as WordPress drafts
6. ✅ Nvidia NIM integration works without tool_reference errors
7. ✅ MCP Chrome integration for live analysis
8. ✅ Average SEO score improvement of 20+ points
