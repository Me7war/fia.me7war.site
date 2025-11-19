# Fia – AI Nutrition Companion

## Branding Overview

**Name**: Fia – short, cute, memorable; evokes a personal, pet-like companion.

**Tagline**: "Solving calorie tracking with AI for effortless healthy eating."

**Three-word Descriptor**: Healthy Eating Simplified

### Mascot & Logo Concept
- **Animal**: Fox - friendly, clever, and approachable
- **Design**: Orange body (#FF751B2) with soft cream accents (#FEEBD0)
- **Style**: Rounded, minimalist shapes for modern appeal
- **AI Element**: Optional spark in the eye to hint at AI intelligence
- **Integration**: Fox integrated with letter "F" or positioned next to name for iconic logo

### Color Palette
- **Primary**: #FF751B2 (fox accent color)
- **Background/Secondary**: #FEEBD0 (soft cream)
- **Highlights**: White accents for eyes and details

### Personality & Tone
Friendly, clever, supportive, and approachable — like a personal AI companion guiding nutrition journeys. Playful, warm, and humanized to feel like a helpful friend rather than a tool.

### Design Philosophy
Minimalist, rounded shapes for modern appeal. Warm, inviting colors that evoke friendliness and trust. Brand identity is soft, approachable, shareable, and consistent across app icon, promotional materials, and user interface.

---

## Project Overview
Fia is a serverless AI-powered calorie counter app that competes directly with premium fitness apps at a fraction of the cost. The app provides AI-powered meal analysis from plain text descriptions, personalized meal tracking, and goal management through both web and mobile platforms.

## Core Concept
Fia is an AI-powered calorie tracking app that combines simple note-taking with intelligent meal analysis. Users log what they eat in plain English, and the AI fetches calorie information from multiple reference sources, calculates averages, and displays results with an intuitive, motivating interface.

**Unique Value Proposition:**
- **Notebook-style logging**: Write meals naturally instead of barcode scanning or complex inputs
- **Transparent AI process**: Users see real-time "searching" and "calculating" with animations
- **Progressive engagement**: Experience AI power before requiring payment
- **Trusted calculation**: Multiple source averaging for accuracy

## Core Vision
Create an affordable alternative to premium health apps by offering:
- AI-powered meal analysis from plain text descriptions
- Serverless architecture for scalability
- Lower subscription costs than market leaders
- Intuitive notebook-style interface for sustainable health habits

## Business Model
- **Free tier**: Plain text meal logging, AI calorie calculation (limited tries), basic tracking, manual goals
- **Premium tier ($4.99/month)**: Unlimited AI calculations, personalized plans, advanced analytics, streak rewards
- **Revenue target**: 10,000+ users in first year through competitive pricing strategy

## Technical Architecture
### Frontend
- **Mobile**: React Native with Expo
- **Web**: Next.js with responsive design

### Backend-as-a-Service
- **Database**: Supabase (PostgreSQL with real-time features)
- **Auth**: Supabase Authentication
- **AI Services**: OpenAI Vision API / Google Cloud Vision
- **File Storage**: Supabase Storage

### Hosting & Infrastructure
- **Frontend**: Vercel (web) + Expo Application Services (mobile)
- **Serverless Functions**: Vercel Edge Functions / Supabase Edge Functions
- **Payment Processing**: Stripe integration

## Target Market
- Health-conscious individuals seeking affordable fitness tracking
- Users frustrated with high-priced subscription models
- Fitness enthusiasts who want AI-powered insights
- People following specific diet plans who need accurate nutritional data

## Competitive Advantages
1. **Price**: ~60% cheaper than premium competitors
2. **AI Accuracy**: Focus on improving food recognition over time
3. **User Experience**: Intuitive onboarding and clean design
4. **Scalability**: Serverless architecture supports rapid user growth
5. **Feature Parity**: Core features match or exceed premium competitors

## Revenue Streams
- Monthly subscriptions ($4.99)
- Annual subscriptions ($49.99 - 17% discount)
- In-app meal plan purchases
- Premium add-ons (advanced analytics)

## Success Metrics
- 10K+ active users within 6 months
- 4.8+ star app store rating
- 70% user retention rate
- Average revenue per user (ARPU) of $3.50/month

## Core Features

### Main Logging Interface
**UI Design Philosophy:**
- **Notebook Experience**: Page resembles a traditional notebook/journal for familiar, comfortable logging
- **Daily Fresh Start**: Clean page every day encourages consistent habit formation
- **Trust-Through-Transparency**: Show AI process visibly to build confidence

**Interface Layout:**
- **Top Bar**: Logo (top left), Settings and notification icons (top right)
- **Page Title**: "Today's Journey" + current date
- **Floating Info Widget**: Daily calorie target, consumed calories, streak counter
- **Daily Notebook Area**: Plain text input for natural meal descriptions like "A Big Mac from McDonald's with Pepsi and large fries"

### AI Meal Calculation Flow
**User Input Process:**
1. User writes meal in plain English
2. 5-second wait allows multi-line entries
3. Animated sequence builds anticipation and trust:

**Animation Steps:**
1. **"Searching..."** → AI queries multiple online reference sources with dynamic source icons
2. **"Calculating..."** → AI processes and averages calorie data
3. **"+[X] kcal"** → Final result displays with smooth transition

**Technical Implementation:**
- Multiple API sources for accuracy
- Intelligent averaging algorithm
- Error handling for unclear food descriptions
- Offline fallback for common foods

### Additional Features
- **Optional Body Photos**: Before/after photos for progress visualization (fully clothed, secure storage)
- **Goal Completion Flow**: "Finished Goal" button triggers celebration, AI analysis, and maintenance plan generation
- **Notifications System**: Customizable reminders, streak encouragement, health tips
- **Settings Panel**: Notification frequency, privacy controls, UI preferences

### Free vs. Premium Experience
**Free Tier:**
- Plain text meal logging
- Limited AI calculations (3 per day)
- Basic tracking and manual goals
- Core features work without payment

**Premium Tier ($4.99/month):**
- Unlimited AI calculations
- Personalized AI-generated plans
- Advanced analytics and insights
- Enhanced streak rewards
- Priority support

## Design Philosophy & User Experience Principles

**AI as Assistant, Not Dictator:**
- Users can always override AI suggestions
- Educational rather than restrictive approach
- Builds trust through transparency and control

**Frictionless Logging:**
- Natural language input eliminates barriers
- Interactive animations make waiting engaging
- One-tap meal recording for power users

**Progressive Engagement:**
- Experience full AI value before gating features
- Clear upgrade paths with compelling value props
- Free tier remains functionally useful

**Positive Reinforcement:**
- Streak counters celebrating consistency
- Achievement celebrations for milestones
- Encouraging copy throughout the experience

**Privacy & Trust:**
- Optional features never feel required
- Transparent data usage explanations
- Secure handling of photos and personal data

## User Experience & Onboarding Flow

### 1. Installation
User installs the app from App Store / Play Store.

### 2. Intro Slideshow
**Purpose**: Quick slides showing app features and building initial excitement.

**Slide Content**:
- Note-based logging (show interface)
- AI calorie calculation process
- Personalized plans and streaks
- Clean, intuitive design screenshots

### 3. Get Started / CTA Button
**Button Text**: "Count Me In"

**Supporting Elements**:
- Optional animation or microcopy: "Let's start your journey to a healthier you!"
- Builds excitement and commitment

### 4. Initial Data Collection
**Progressive Collection**:
After pressing CTA, collect basic personal info sequentially:

1. **Age** (least sensitive)
2. **Height**
3. **Weight** (most sensitive)
4. **Optional Body Photo**: Before/after photo for progress (fully clothed, secure storage)

*Each question appears one per screen for low-friction flow.*

### 5. Goals Selection
**Goal Options**:
- Lose weight
- Maintain weight
- Gain weight
- Custom calories per day

**Smart Defaults**: Based on user data, suggesting reasonable ranges.

### 6. Feature Choice: Premium vs. Normal
**Critical Branch Point**: Users choose their experience level.

#### Premium Path
**Pitch**: "Want our AI to build your healthy life? Let it design your complete body plan."

**Process**:
1. AI analyzes user data and selected goal
2. Generates personalized daily calorie goal
3. Creates weekly health strategy
4. Provides tailored tips

**Retry Mechanism**: Up to 3 attempts to get desired plan, then prompts Pro upgrade.

#### Normal Path
**Alternative Experience**:
- Manual daily calorie goal entry
- Standard tracking features
- No AI personalization
- Full functionality without premium limitations

### 7. Notification Preferences (Optional)
**Frequency Options**:
- Light reminders
- Standard reminders
- High-intensity tracking
- No notifications

*Avoids overwhelming users while providing customization.*

### 8. Account Creation & Final Setup
**Strategic Timing**: After investment in data entry, account creation feels purposeful.

**Copy**: "Your personalized plan is ready. Sign in to save it and enable AI tracking."

**Benefits**:
- Data syncs and persists
- Enables cross-device usage
- Unlocks premium features for subscribed users

**Upon Sign-in**: Main dashboard loads with personalized setup.

## Long-Term User Journey

### Daily Usage
- **Notebook Interface**: Daily fresh page encourages consistency
- **AI Meal Processing**: Text input → Searching → Calculating → Result
- **Progress Tracking**: Calories consumed vs. target, streaks, achievements

### Goal Completion Flow
**"Finished Goal" Button** in settings:

1. **Celebration**: Achievement recognition and congratulations
2. **Optional After Photo**: Progress comparison
3. **AI Analysis**: Reviews past consumption patterns
4. **New Plan Generation**: Creates maintenance calories based on actual habits
5. **Continued Engagement**: Shifts focus from weight change to sustainability

### Engagement Narrative
**Story Arc**: Start → Progress → Achievement → Sustain.
**Psychology**: Positive reinforcement, building habits, celebrating wins.
