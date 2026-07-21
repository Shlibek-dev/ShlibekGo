# GEMINI CODE AGENT CONTEXT & INSTRUCTIONS: SHLIBEKGO

## 1. PROJECT IDENTITY & PURPOSE
- **Application Name**: ShlibekGo
- **Domain**: Building materials sales, delivery logistics, accounting, and bookkeeping system in Libya.
- **Operating Environment**: Mobile handsets and tablets used by stationary office workers (Reception, Sales, Cashier, Admin) and mobile field workers (Drivers).
- **Scale**: 5+ internal employees, 10+ company delivery trucks.

## 2. CORE ARCHITECTURAL & DESIGN GUARDRAILS
- **Target Platform**: Android 11 (API Level 30) and above.
- **Design System**: Native Material Design 3 (M3) components.
- **Localization & Layouts**: Full English and Arabic support with dynamic Right-to-Left (RTL) layout flipping capability.
- **Local-First Philosophy**: All primary operations (reading, writing, order processing) must operate seamlessly offline locally first, with background real-time cloud synchronization when online.
- **Footprint**: Ultra-lightweight codebase; avoid unnecessary external libraries or heavy frameworks. Maintain maximum performance on standard Android hardware.

## 3. BUSINESS ROLES & WORKFLOW PIPELINE
1. **Admin / Management**:
   - Company profile configuration.
   - User credential provisioning & role assignment.
   - Mass admin messaging broadcasted directly to employee system notification trays.
2. **Reception**:
   - Customer search and profile creation (Name, Phone, Site Address).
   - Sale Order creation for materials and site transportation.
   - Generation of digital/printable PDF Sale Orders.
3. **Sales**:
   - Order intake queue processing.
   - Conversion of Sale Orders into active Sales transactions.
   - Transaction edits and PDF order output.
4. **Cashier**:
   - In-person cash payment collection (Libyan Dinar).
   - Partial and full payment tracking.
   - Automated creation of formal Delivery Orders.
5. **Driver / Field Logistics**:
   - Logistics queue of assigned pending deliveries.
   - Real-time delivery status updates (Item-level or full delivery site confirmation).

## 4. SYSTEM CAPABILITIES & MODULES
- **PDF Generation**: Native support for creating printable/shareable invoices, sale orders, and delivery slips.
- **In-App APK Update System**: Mechanism to check for software updates against a remote configuration and trigger seamless in-app APK update downloads and installs.
- **System Tray Push Messaging**: Admin messaging feature that pushes alerts directly to active employee Android notification bars.

## 5. CODE AGENT CODE GENERATION RULES
- Write clean, modular, and compilable Kotlin/XML code tailored for Android Studio.
- Produce **complete, non-truncated code files** ready to copy/paste or automatically integrate.
- Ensure all UI components natively respect Material Design 3 and RTL constraints.
- Prioritize incremental build tasks: solve one specific UI component, database layer, or business logic rule at a time.