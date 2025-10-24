# Quarry Point Design Blueprint

## Part 1: The Design System (The "DNA")

Before we design a single page, we must define the rules. This ensures every page, button, and component feels like it belongs to the same family. This is the "look and feel" you asked for.

### 1. Color Palette

The name "Quarry Point" evokes a balance of earthy/solid ("Quarry") and modern/precise ("Point"). The palette must be professional, high-end, and trustworthy, with a creative spark.

- **Charcoal (Primary Text):** #2D2D2D  
  *Use:* All primary text, headlines, and icons. It's softer and more professional than pure black.

- **Stone (Main Background):** #F8F7F5  
  *Use:* The main background for all pages. Very light, warm, stony-grey. Architectural feel.

- **Sand (Card Background):** #EAE4D9  
  *Use:* Background for cards (project cards, user cards). Adds depth and subtle earthy texture.

- **Rust (Primary Action):** #D95B43  
  *Use:* The "Builder" color. Main buttons, key notifications, active states. Strong and earthy.

- **Blueprint Blue (Accent/Link):** #4A6CFA  
  *Use:* The "Creator" color. Text links, secondary buttons, metadata. Vibrant, precise, pops against earthy tones.

### 2. Typography

We need two fonts: one for headlines (Creator/Vision) and one for text (Builder/Functional).

- **Headings Font: Manrope**  
  Modern, geometric sans-serif. Clean and strong. Ideal for headlines and brand identity. (Google Fonts)

- **Body Font: Inter**  
  Highly-readable, functional sans-serif for body text, descriptions, UI elements. (Google Fonts)

### 3. Core Components (The "Lego Bricks")

- **Navbar:** Stone background, logo on left, center search bar, right-side links ("Discover," "Feed") and user profile icon.
- **Buttons:**  
  - Primary (Rust): Solid background, bold white text. Main actions.  
  - Secondary (Blueprint Blue): Text and outline in Blueprint Blue. Secondary actions.
- **Project Card:**  
  - Layout: Sand background, 8px rounded corners  
  - Top: Full-width image  
  - Bottom: Project title (Manrope, bold), creator's profile pic + name (Inter, Blueprint Blue link)
- **User Card:**  
  - Layout: Circular profile pic left, full name bold + @username grey right

---

## Part 2: Page-by-Page UI & Layout Blueprint

### 1. Home (The Feed)
- **Purpose:** Visual feed of inspiration from creators and suggested projects  
- **Color Scheme:** Stone background, grid of Sand-colored ProjectCard components  
- **Layout (3-Column):**  
  - Left (20%): User profile info, navigation links (Feed, Discover, Bookmarks)  
  - Middle (50%): Main endless-scrolling feed of ProjectCard components  
  - Right (30%): "Who to Follow" (architects) + "Find a Builder" (tradespeople)

### 2. Project Detail
- **Purpose:** Deep dive into a single project  
- **Color Scheme:** Stone background, Rust & Blueprint Blue buttons  
- **Layout (1-Column, Wide):**  
  - Project Header: Manrope bold title, architect's UserCard, Bookmark & Share buttons  
  - Hero Image: Full-bleed main project image  
  - Project Description: Rich text explaining brief & process  
  - Image Gallery: Masonry grid of other project photos  
  - "The Build Team": Horizontal list of tagged tradespeople UserCards  
  - Comment Section: Community comments

### 3. User Profile (Architect / "Creator")
- **Purpose:** Creator's main portfolio  
- **Layout:**  
  - Profile Header: Large circular profile picture left, full name (Manrope), @username, Bio right, Follow (Rust) + Contact (Blue) far right  
  - Tab Navigation: "Projects" (Default) | "Saved" | "About"  
  - Projects Tab: 3-column grid of ProjectCard components

### 4. User Profile (Tradesperson / "Builder")
- **Purpose:** Builder's resume showing verified projects  
- **Layout:**  
  - Profile Header: Same as Architect + "Verified" badge  
  - Tab Navigation: "Tagged In" (Default) | "Portfolio" | "Credentials"  
  - Tagged In Tab: 3-column grid of ProjectCard components  
  - Credentials: License, Insurance, Specialty

### 5. Login & Register
- **Purpose:** Simple, secure access  
- **Layout (50/50 Split Screen):**  
  - Left (50%): Full-height image (architectural detail)  
  - Right (50%): Stone background, Quarry Point Logo, Headline: "Sign in to the Collective"  
  - Form Fields: Email, Password with Sand backgrounds  
  - Main Button: Login (Rust)  
  - Link: "Don't have an account? Sign Up" (Blueprint Blue)

### 6. Upload Project
- **Purpose:** Workflow for creators to add new projects  
- **Layout (1-Column, Centered):**  
  - Headline: "Add a New Project" (Manrope)  
  - Image Uploader: Drag & Drop area  
  - Form Fields: Project Title, Description (rich text), Categories (tags)  
  - "Tag Your Builders": Search box, clickable UserCard results  
  - Publish Button: Large Rust button
