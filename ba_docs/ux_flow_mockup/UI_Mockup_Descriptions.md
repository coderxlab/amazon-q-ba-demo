# UI Mockup Descriptions - Calorie Counter Application

**Document Version**: 1.0  
**Date**: 2025-01-27  
**Project**: Calorie Counter Application  
**Document Type**: UI Mockup Specifications  
**Design System**: Material Design 3 Guidelines

---

## Screen 1: Landing/Search Screen

### Layout Structure
- **Header**: Fixed top bar (64px height)
- **Main Content**: Centered search interface
- **Footer**: Minimal attribution section

### UI Components

#### Header Section
- **App Title**: "Calorie Counter"
  - Typography: Headline Medium (24px, Roboto Medium)
  - Color: Primary (#1976D2)
  - Position: Left-aligned with 16px margin
- **USDA Attribution**: "Powered by USDA FoodData Central"
  - Typography: Body Small (12px, Roboto Regular)
  - Color: On-surface variant (#49454F)
  - Position: Right-aligned

#### Main Search Interface
- **Container**: Centered card with elevation-1 shadow
  - Width: 90% (mobile), 480px max (desktop)
  - Padding: 32px
  - Border radius: 12px
  - Background: Surface (#FFFBFE)

- **Search Input Field**:
  - Component: Material Outlined TextField
  - Width: 100%
  - Height: 56px
  - Label: "Search for food"
  - Placeholder: "e.g., chicken breast, apple"
  - Leading icon: Search icon (24px)
  - Trailing icon: Clear icon (appears on input)
  - Border: 1px solid Outline (#79747E)
  - Focus state: 2px solid Primary (#1976D2)
  - Error state: 2px solid Error (#BA1A1A)

- **Search Button**:
  - Component: Material Filled Button
  - Width: 100%
  - Height: 40px
  - Text: "Search"
  - Background: Primary (#1976D2)
  - Text color: On-primary (#FFFFFF)
  - Margin top: 16px
  - Disabled state: Surface variant (#E7E0EC)

#### Error Message Area
- **Container**: Below search button
- **Typography**: Body Small (12px, Roboto Regular)
- **Color**: Error (#BA1A1A)
- **Visibility**: Hidden by default, shown on validation errors

### Responsive Behavior
- **Mobile (≤768px)**: Full-width container with 16px side margins
- **Tablet/Desktop (>768px)**: Fixed 480px width, centered

---

## Screen 2: Search Results Screen

### Layout Structure
- **Header**: Persistent search bar (72px height)
- **Results Section**: Scrollable list container
- **Load More**: Bottom-aligned button

### UI Components

#### Persistent Search Header
- **Background**: Surface (#FFFBFE) with elevation-2 shadow
- **Search Bar**: 
  - Width: Calc(100% - 32px)
  - Height: 40px
  - Current search term pre-filled
  - Edit icon (16px) on right side

#### Results Header
- **Text**: "X results found for 'search term'"
- **Typography**: Title Small (14px, Roboto Medium)
- **Color**: On-surface (#1C1B1F)
- **Padding**: 16px horizontal, 12px vertical

#### Results List Container
- **Component**: Material List with dividers
- **Background**: Surface (#FFFBFE)

#### Individual Result Items
- **Container**: List item with 16px padding
- **Height**: 72px minimum
- **Layout**: Three-column grid

- **Food Name** (Column 1):
  - Typography: Body Large (16px, Roboto Regular)
  - Color: On-surface (#1C1B1F)
  - Max width: 50%
  - Text overflow: Ellipsis

- **Portion Size** (Column 2):
  - Typography: Body Medium (14px, Roboto Regular)
  - Color: On-surface variant (#49454F)
  - Text align: Center

- **Calorie Count** (Column 3):
  - Typography: Label Large (14px, Roboto Medium)
  - Color: Primary (#1976D2)
  - Text align: Right
  - Format: "XXX cal"

- **Hover State**: Background changes to Surface variant (#F3EDF7)
- **Focus State**: 2px outline in Primary color
- **Divider**: 1px line in Outline variant (#CAC4D0)

#### Load More Button
- **Component**: Material Outlined Button
- **Width**: Calc(100% - 32px)
- **Height**: 40px
- **Text**: "Load More Results"
- **Margin**: 16px all sides
- **Border**: 1px solid Outline (#79747E)
- **Background**: Transparent
- **Text color**: Primary (#1976D2)

### Responsive Behavior
- **Mobile**: Single column, full-width items
- **Tablet**: Two-column grid layout
- **Desktop**: Three-column grid with larger spacing

---

## Screen 3: No Results Screen

### Layout Structure
- **Header**: Same persistent search bar as Results screen
- **Main Content**: Centered empty state illustration and messaging
- **Suggestions**: Card-based recommendation section

### UI Components

#### Empty State Illustration
- **Container**: Centered, 240px width
- **Icon**: Material Search Off icon (64px)
- **Color**: On-surface variant (#49454F)
- **Background**: Circular surface variant (#F3EDF7), 120px diameter

#### No Results Message
- **Primary Text**: "No results found"
- **Typography**: Headline Small (24px, Roboto Regular)
- **Color**: On-surface (#1C1B1F)
- **Text align**: Center
- **Margin bottom**: 8px

- **Secondary Text**: "for 'search term'"
- **Typography**: Body Large (16px, Roboto Regular)
- **Color**: On-surface variant (#49454F)
- **Text align**: Center

#### Suggestions Card
- **Container**: Material Card with elevation-1
- **Width**: 90% (mobile), 480px max (desktop)
- **Padding**: 24px
- **Margin top**: 32px
- **Border radius**: 12px

- **Suggestions Title**: "Try these suggestions:"
- **Typography**: Title Medium (16px, Roboto Medium)
- **Color**: On-surface (#1C1B1F)
- **Margin bottom**: 16px

- **Suggestion List**:
  - Bullet points with 8px spacing
  - Typography: Body Medium (14px, Roboto Regular)
  - Color: On-surface variant (#49454F)
  - Line height: 20px

#### Popular Searches Section
- **Title**: "Popular searches:"
- **Typography**: Label Large (14px, Roboto Medium)
- **Color**: On-surface (#1C1B1F)
- **Margin**: 24px top, 12px bottom

- **Search Tags**: Material Chip components
- **Layout**: Flex wrap with 8px gaps
- **Individual Chip**:
  - Height: 32px
  - Padding: 0 12px
  - Background: Surface variant (#E7E0EC)
  - Text color: On-surface variant (#49454F)
  - Border radius: 16px
  - Hover: Elevation-1 shadow

#### Try Again Button
- **Component**: Material Filled Button
- **Width**: 100%
- **Height**: 40px
- **Text**: "Try Another Search"
- **Background**: Primary (#1976D2)
- **Text color**: On-primary (#FFFFFF)
- **Margin top**: 24px

---

## Screen 4: Loading States

### Layout Structure
- **Header**: Same persistent search bar (if applicable)
- **Main Content**: Centered loading indicator and messaging
- **Cancel Option**: Bottom-aligned button (appears after 3 seconds)

### UI Components

#### Loading Indicator
- **Component**: Material Circular Progress Indicator
- **Size**: 48px diameter
- **Color**: Primary (#1976D2)
- **Position**: Centered horizontally and vertically

#### Loading Message
- **Text**: "Searching for 'search term'..."
- **Typography**: Body Large (16px, Roboto Regular)
- **Color**: On-surface variant (#49454F)
- **Text align**: Center
- **Margin top**: 24px

#### Progress Context (Optional)
- **Text**: "This may take a few seconds"
- **Typography**: Body Small (12px, Roboto Regular)
- **Color**: On-surface variant (#49454F)
- **Text align**: Center
- **Margin top**: 8px

#### Cancel Search Button
- **Component**: Material Text Button
- **Text**: "Cancel Search"
- **Text color**: Primary (#1976D2)
- **Position**: Bottom center
- **Margin bottom**: 32px
- **Visibility**: Hidden initially, appears after 3 seconds

### Animation Specifications
- **Loading Spinner**: Continuous rotation, 1.4s duration
- **Fade In**: Cancel button fades in over 300ms
- **Pulse Effect**: Subtle pulse on loading message (optional)

---

## Global Design Specifications

### Color Palette (Material Design 3)
- **Primary**: #1976D2 (Blue 700)
- **On-Primary**: #FFFFFF
- **Surface**: #FFFBFE
- **On-Surface**: #1C1B1F
- **On-Surface Variant**: #49454F
- **Outline**: #79747E
- **Outline Variant**: #CAC4D0
- **Error**: #BA1A1A
- **Surface Variant**: #E7E0EC

### Typography Scale
- **Headline Medium**: 24px, Roboto Medium
- **Headline Small**: 24px, Roboto Regular
- **Title Medium**: 16px, Roboto Medium
- **Title Small**: 14px, Roboto Medium
- **Body Large**: 16px, Roboto Regular
- **Body Medium**: 14px, Roboto Regular
- **Body Small**: 12px, Roboto Regular
- **Label Large**: 14px, Roboto Medium

### Spacing System
- **Base unit**: 4px
- **Common spacings**: 8px, 12px, 16px, 24px, 32px
- **Component padding**: 16px standard
- **Section margins**: 24px vertical, 16px horizontal

### Elevation Levels
- **Level 0**: No shadow (default surface)
- **Level 1**: 0px 1px 3px rgba(0,0,0,0.12)
- **Level 2**: 0px 2px 6px rgba(0,0,0,0.16)

### Interactive States
- **Hover**: Slight elevation increase or background color change
- **Focus**: 2px outline in Primary color
- **Active**: Slight scale reduction (0.98) with elevation
- **Disabled**: 38% opacity, no interaction

### Responsive Breakpoints
- **Mobile**: 0px - 767px
- **Tablet**: 768px - 1023px
- **Desktop**: 1024px and above

### Accessibility Specifications
- **Minimum touch target**: 44px x 44px
- **Color contrast ratio**: 4.5:1 minimum
- **Focus indicators**: Always visible and high contrast
- **Screen reader labels**: All interactive elements have descriptive labels
- **Keyboard navigation**: Logical tab order throughout all screens