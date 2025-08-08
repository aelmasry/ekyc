# eKYC System - Technical Documentation

## Project Overview

The eKYC (Electronic Know Your Customer) system is a comprehensive Laravel-based backend API for managing customer onboarding, SIM card distribution, and staff hierarchy in a telecommunications context. The system implements a multi-tier organizational structure for managing different types of users and their permissions while facilitating customer verification through OCR technology and document management.

### Business Domain
- **Primary Purpose**: SIM card distribution and customer verification system
- **Industry**: Telecommunications/Mobile Network Operations
- **Target Markets**: Tanzania and UAE (based on OCR support)

## Business Logic & Core Features

### 1. Customer Management (KYC Process)
- **Customer Onboarding**: Digital customer registration with document verification
- **Document Processing**: OCR-powered automatic data extraction from national IDs
- **KYC File Generation**: Automated PDF generation for compliance documentation
- **Customer Types**: Support for both individual and company customers
- **Citizenship Handling**: Different rules for local vs foreign customers
- **Age Verification**: Minimum age requirements for SIM card purchases
- **Customer Blocking**: Ability to block/unblock customers with reasons

### 2. SIM Card Management
- **SIM Card Lifecycle**: Creation, assignment, approval/rejection workflow
- **Bulk Operations**: Support for bulk SIM card creation
- **Status Tracking**: Multiple states (pending, approved, rejected)
- **Supervisor Assignment**: Automatic assignment of SIMs to supervisors
- **Serial Number Management**: Unique identification and tracking
- **PUK Code Management**: Secure PUK code storage and retrieval

### 3. Staff Hierarchy Management
```
eKYC Staff Hierarchy
├── Sales General Manager
│   └── Sales Area Manager
│       └── Sales Supervisor
│           └── Sales Agent
│
└── iBolling General Manager
    └── iBolling Supervisor
        └── iBolling Agent
```

### 4. User Type & Permission System
- **Hierarchical User Types**: Structured user type system with superior-subordinate relationships
- **Role-Based Access Control**: Integration with Spatie Permissions package
- **Dynamic Permissions**: User type-based permission assignment
- **Organization Structure**: Visual organization chart generation

### 5. Geographical Data Management
- **Multi-level Geography**: Countries → Cities → States
- **User Location Tracking**: Geographic assignment for users
- **Team Area Management**: Territory-based team assignments

### 6. OCR Integration
- **Document Recognition**: Automatic data extraction from identity documents
- **Multi-Country Support**: Tanzanian and UAE ID card parsing
- **Image Processing**: Automatic image optimization and compression
- **Fallback Handling**: Graceful handling of OCR failures

## Technology Stack

### Backend Framework & Core
- **PHP 8.2+**: Modern PHP with latest features
- **Laravel 11.31**: Latest Laravel framework
- **Laravel Sanctum 4.0**: API authentication
- **MySQL**: Primary database

### Key Dependencies
- **spatie/laravel-permission**: Role and permission management
- **barryvdh/laravel-dompdf**: PDF generation for KYC documents
- **intervention/image**: Image processing and optimization
- **hofmannsven/laravel-brevo**: Email service integration
- **OCR.space API**: External OCR service integration

### Development & Testing
- **PHPUnit**: Unit and feature testing
- **Laravel Pint**: Code style formatting
- **Laravel Sail**: Docker development environment
- **Faker**: Test data generation

## Architecture Style

### MVC + Service Layer Architecture

The system follows a **Layered MVC architecture** with additional service layer for business logic:

```
┌─────────────────┐
│   Controllers   │  ← HTTP Request Handling
├─────────────────┤
│    Services     │  ← Business Logic Layer
├─────────────────┤
│     Models      │  ← Data Access Layer (Eloquent ORM)
├─────────────────┤
│    Database     │  ← MySQL Storage
└─────────────────┘
```

### Key Architectural Patterns
1. **Repository Pattern**: Implemented through Eloquent models
2. **Service Pattern**: Business logic encapsulated in service classes
3. **Resource Pattern**: API response transformation via Eloquent resources
4. **Request Validation**: Form request classes for input validation
5. **Observer Pattern**: Model events and listeners
6. **Strategy Pattern**: OCR parsing for different document types

## API Architecture

### Authentication
- **Laravel Sanctum**: Token-based API authentication
- **Multiple Guards**: Separate authentication for admin and agent users
- **Role-Based Access**: Permission-based route protection

### Response Format
All API responses follow a consistent format:

**Success Response:**
```json
{
  "data": {...},
  "message": "Success message",
  "pagination": {
    "total": 100,
    "count": 10,
    "per_page": 10,
    "current_page": 1,
    "total_pages": 10
  }
}
```

**Error Response:**
```json
{
  "message": "Error message"
}
```

### API Endpoints Structure

#### Authentication Endpoints
- `POST /api/admin/login` - Admin authentication
- `POST /api/agent/login` - Agent authentication
- `POST /api/admin/logout` - Admin logout
- `POST /api/agent/logout` - Agent logout
- `POST /api/set-password` - Set password for new users
- `POST /api/forgot-password` - Password reset request

#### User Management
- `GET /api/user/organization-structure` - Get hierarchical organization chart
- `GET /api/user/all` - List all users
- `GET /api/user/{id}` - Get user details
- `PUT /api/user/{id}` - Update user
- `POST /api/user` - Create new user
- `POST /api/user/change_password` - Change password
- `GET /api/user` - List users with pagination

#### Customer Management
- `GET /api/customer` - List customers with filtering
- `GET /api/customer/{id}` - Get customer details
- `POST /api/customer` - Create new customer
- `PUT /api/customer/{id}` - Update customer
- `DELETE /api/customer/{id}` - Delete customer
- `GET /api/customer/check` - Check customer eligibility

#### SIM Card Management
- `GET /api/sim` - List SIM cards
- `GET /api/sim/{id}` - Get SIM details
- `POST /api/sim` - Create SIM card
- `POST /api/sim/bulk` - Bulk create SIM cards
- `PUT /api/sim/{id}` - Update SIM status

#### Role & Permission Management
- `GET /api/role` - List roles
- `GET /api/role/{id}` - Get role details
- `POST /api/role` - Create role
- `PUT /api/role/{id}` - Update role
- `DELETE /api/role/{id}` - Delete role
- `GET /api/permission` - List permissions

#### Settings Management
- `POST /api/settings/set` - Update settings
- `GET /api/settings/get` - Get settings
- `POST /api/settings/add-sim-contract-image` - Upload contract image
- `POST /api/settings/refresh-sims-supervisors` - Refresh supervisor assignments

#### Team Management
- `GET /api/teams` - List teams
- `GET /api/teams/{id}` - Get team details
- `POST /api/teams` - Create team
- `PUT /api/teams/{id}` - Update team
- `DELETE /api/teams/{id}` - Delete team

#### User Type Management
- `GET /api/user-types` - List user types
- `GET /api/user-types/{id}` - Get user type details
- `POST /api/user-types` - Create user type
- `PUT /api/user-types/{id}` - Update user type
- `DELETE /api/user-types/{id}` - Delete user type

#### Geographical Data
- `GET /api/geo/countries` - List countries
- `GET /api/geo/country/{countryId}` - Get country details
- `GET /api/geo/country/{countryId}/cities` - Get cities by country
- `GET /api/geo/city/{cityId}/states` - Get states by city
- `POST /api/geo/add-country-data` - Add country
- `POST /api/geo/add-city-data` - Add city
- `DELETE /api/geo/country/{countryId}` - Delete country
- `DELETE /api/geo/city/{cityId}` - Delete city
- `DELETE /api/geo/state/{stateId}` - Delete state

#### OCR Service
- `POST /api/getData` - Extract data from document images (No authentication required)

## Database Schema & Relations

### Core Tables

#### Users Table
```sql
- id (Primary Key)
- name (string)
- email (string, unique)
- password (string, nullable)
- type (string, nullable)
- bio (text, nullable)
- status (boolean, default: false)
- phone (string, nullable)
- address (string, nullable)
- image (string, nullable)
- country_id (foreign key to setting_countries)
- city_id (foreign key to setting_cities)
- state_id (foreign key to setting_states)
- title (string, nullable)
- parent_id (foreign key to users, self-referencing)
- user_type_id (foreign key to user_types)
- created_at, updated_at
- deleted_at (soft deletes)
```

#### Customers Table
```sql
- id (Primary Key)
- name (string)
- email (string, nullable)
- phone_number (string, nullable)
- nationality (string, nullable)
- birth_date (date, nullable)
- document_number (string, unique)
- document_expiry_date (date)
- submission_status (string)
- address (string, nullable)
- occupation (string, nullable)
- sims_number (integer, nullable)
- type (string: individual/company)
- image (string, nullable)
- signature_image (string, nullable)
- document_image_front (string, nullable)
- document_image_back (string, nullable)
- support_document_image (string, nullable)
- document_type (string, nullable)
- permission_litter_image (string, nullable)
- kyc_file (string, nullable)
- created_by (foreign key to users)
- is_blocked (boolean, default: false)
- is_citizen (boolean, default: false)
- block_reason (text, nullable)
- created_at, updated_at
- deleted_at (soft deletes)
```

#### SIM Cards Table
```sql
- id (Primary Key)
- barcode_image (string, nullable)
- sim_number (string)
- serial_number (string, nullable)
- puk (string)
- status (string, default: 'pending')
- reject_reason (text, nullable)
- contract_file (string, nullable)
- customer_id (foreign key to customers)
- supervisor_id (foreign key to users)
- created_by (foreign key to users)
- created_at, updated_at
```

#### User Types Table
```sql
- id (Primary Key)
- name (string)
- role_id (foreign key to roles)
- superior_id (foreign key to user_types, self-referencing)
- created_at, updated_at
```

#### Teams Table
```sql
- id (Primary Key)
- name (string)
- manager_id (foreign key to users)
- created_at, updated_at
```

### Supporting Tables

#### Settings Table
```sql
- id (Primary Key)
- key (string)
- value (string)
- created_at, updated_at
```

#### Geographical Tables
```sql
-- setting_countries
- id (Primary Key)
- name (string)
- created_at, updated_at

-- setting_cities
- id (Primary Key)
- name (string)
- country_id (foreign key to setting_countries)
- created_at, updated_at

-- setting_states
- id (Primary Key)
- name (string)
- city_id (foreign key to setting_cities)
- created_at, updated_at
```

#### Junction Tables
```sql
-- team_user (Many-to-Many: Teams ↔ Users)
- team_id (foreign key to teams)
- user_id (foreign key to users)

-- team_manager (Many-to-Many: Teams ↔ Managers)
- team_id (foreign key to teams)
- user_id (foreign key to users)

-- team_area (Many-to-Many: Teams ↔ Areas)
- team_id (foreign key to teams)
- area_id (foreign key to setting_states)
```

### Key Relationships

1. **Users** have hierarchical relationships (parent_id → users.id)
2. **Users** belong to **UserTypes** which define roles and permissions
3. **Customers** are created by **Users** (created_by → users.id)
4. **SIM Cards** belong to **Customers** and are supervised by **Users**
5. **Teams** have **Users** as members and managers
6. **Teams** can be assigned to geographical **Areas** (States)
7. **Users** have geographical location (**Country** → **City** → **State**)

## Module Breakdown

### 1. Authentication Module
**Files:**
- `app/Http/Controllers/AdminAuthController.php`
- `app/Http/Controllers/AgentAuthController.php`
- `app/Http/Services/AuthService.php`

**Responsibilities:**
- Multi-guard authentication (Admin/Agent)
- Token management with Laravel Sanctum
- Login/logout functionality
- Password reset mechanisms

### 2. User Management Module
**Files:**
- `app/Http/Controllers/UserController.php`
- `app/Http/Services/UserService.php`
- `app/Models/User.php`
- `app/Models/UserType.php`

**Responsibilities:**
- User CRUD operations
- Hierarchical user organization
- Password management
- Organization structure visualization

### 3. Customer Management Module
**Files:**
- `app/Http/Controllers/CustomerController.php`
- `app/Http/Services/CustomerService.php`
- `app/Models/Customer.php`

**Responsibilities:**
- Customer onboarding and KYC
- Document management and file uploads
- PDF generation for compliance
- Customer eligibility verification
- Customer blocking/unblocking

### 4. SIM Card Management Module
**Files:**
- `app/Http/Controllers/SimCardsController.php`
- `app/Http/Services/SimCardService.php`
- `app/Models/SimCard.php`

**Responsibilities:**
- SIM card lifecycle management
- Bulk operations
- Status workflow management
- Supervisor assignment automation

### 5. OCR Processing Module
**Files:**
- `app/Http/Controllers/OcrController.php`
- `app/Http/Services/OcrService.php`
- `app/Http/Services/OcrAttributesObject.php`

**Responsibilities:**
- Document image processing
- OCR data extraction
- Multi-country ID card parsing
- Image optimization

### 6. Role & Permission Module
**Files:**
- `app/Http/Controllers/RoleController.php`
- `app/Http/Controllers/PermissionController.php`
- `app/Http/Services/RoleService.php`

**Responsibilities:**
- Role and permission management
- User type permission mapping
- Access control enforcement

### 7. Settings Module
**Files:**
- `app/Http/Controllers/SettingsController.php`
- `app/Http/Services/SettingsService.php`
- `app/Models/Setting.php`

**Responsibilities:**
- System configuration management
- SIM card limits configuration
- File upload management

### 8. Geographical Module
**Files:**
- `app/Http/Controllers/GeoController.php`
- `app/Http/Services/GeoService.php`
- `app/Models/SettingCountries.php`
- `app/Models/SettingCities.php`
- `app/Models/SettingStates.php`

**Responsibilities:**
- Multi-level geographical data management
- Location-based user assignment
- Territory management for teams

### 9. Team Management Module
**Files:**
- `app/Http/Controllers/TeamsController.php`
- `app/Http/Services/TeamsService.php`
- `app/Models/Team.php`

**Responsibilities:**
- Team creation and management
- Member and manager assignment
- Territory-based team organization

## Environment Variables & Configuration

### Required Environment Variables

```env
# Application
APP_NAME=eKYC
APP_ENV=production
APP_KEY=base64:...
APP_DEBUG=false
APP_URL=http://localhost

# Database
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ekyc
DB_USERNAME=root
DB_PASSWORD=

# Authentication
AUTH_GUARD=web
AUTH_PASSWORD_BROKER=users

# Email Configuration (Brevo)
BREVO_API_KEY=your_brevo_api_key

# OCR Service
OCR_API_KEY=your_ocr_space_api_key

# File Generation
GENERATE_KYC_FILE=true

# Sanctum
SANCTUM_STATEFUL_DOMAINS=localhost,localhost:3000,127.0.0.1,127.0.0.1:8000

# Cache & Session
CACHE_DRIVER=file
SESSION_DRIVER=file

# Queue
QUEUE_CONNECTION=sync

# File Storage
FILESYSTEM_DISK=local
```

### Key Configuration Files

1. **config/app.php** - Application settings
2. **config/auth.php** - Authentication guards and providers
3. **config/sanctum.php** - API authentication configuration
4. **config/permission.php** - Role and permission settings
5. **config/mail.php** - Email service configuration
6. **config/filesystems.php** - File storage configuration

## Setup & Running Instructions

### Prerequisites
- PHP 8.2 or higher
- Composer
- MySQL 5.7+ or 8.0+
- Node.js (for frontend assets)

### Installation Steps

1. **Clone & Dependencies**
   ```bash
   git clone <repository_url>
   cd ekyc
   composer install
   npm install
   ```

2. **Environment Setup**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

3. **Database Setup**
   ```bash
   # Configure database credentials in .env
   php artisan migrate
   php artisan db:seed
   ```

4. **Storage & Assets**
   ```bash
   php artisan storage:link
   npm run build
   ```

5. **Geographical Data**
   ```bash
   php artisan insert:geo
   ```

6. **Development Server**
   ```bash
   php artisan serve
   # Server starts at http://localhost:8000
   ```

### Production Deployment

1. **Optimize for Production**
   ```bash
   composer install --optimize-autoloader --no-dev
   php artisan config:cache
   php artisan route:cache
   php artisan view:cache
   ```

2. **Queue Workers** (if using queues)
   ```bash
   php artisan queue:work --daemon
   ```

3. **Scheduled Tasks** (add to crontab)
   ```bash
   * * * * * cd /path-to-your-project && php artisan schedule:run >> /dev/null 2>&1
   ```

### Development Workflow

The project includes a convenient development script:
```bash
composer run dev
```

This runs:
- Laravel development server
- Queue worker
- Log monitoring (Laravel Pail)
- Vite development server

## System Architecture Diagram

```mermaid
graph TB
    subgraph "Client Layer"
        WEB[Web Frontend<br/>React]
        MOBILE[Mobile App<br/>React Native]
    end
    
    subgraph "API Gateway"
        API[Laravel API<br/>Routes & Middleware]
    end
    
    subgraph "Authentication Layer"
        SANCTUM[Laravel Sanctum<br/>Token Authentication]
        GUARDS[Auth Guards<br/>Admin/Agent]
    end
    
    subgraph "Application Layer"
        CONTROLLERS[Controllers<br/>HTTP Request Handling]
        REQUESTS[Form Requests<br/>Validation]
        RESOURCES[API Resources<br/>Response Formatting]
    end
    
    subgraph "Business Logic Layer"
        SERVICES[Services<br/>Business Logic]
        AUTH_SVC[AuthService]
        CUSTOMER_SVC[CustomerService]
        SIM_SVC[SimCardService]
        OCR_SVC[OcrService]
        USER_SVC[UserService]
    end
    
    subgraph "Data Access Layer"
        MODELS[Eloquent Models]
        USER_MODEL[User]
        CUSTOMER_MODEL[Customer]
        SIM_MODEL[SimCard]
        TEAM_MODEL[Team]
    end
    
    subgraph "External Services"
        OCR_API[OCR.space API]
        EMAIL_SVC[Brevo Email Service]
        PDF_GEN[DomPDF Generator]
    end
    
    subgraph "Storage Layer"
        DATABASE[(MySQL Database)]
        FILES[File Storage<br/>Images & PDFs]
    end
    
    WEB --> API
    MOBILE --> API
    API --> SANCTUM
    SANCTUM --> GUARDS
    GUARDS --> CONTROLLERS
    CONTROLLERS --> REQUESTS
    CONTROLLERS --> RESOURCES
    CONTROLLERS --> SERVICES
    SERVICES --> MODELS
    MODELS --> DATABASE
    
    AUTH_SVC --> SANCTUM
    CUSTOMER_SVC --> PDF_GEN
    CUSTOMER_SVC --> FILES
    OCR_SVC --> OCR_API
    USER_SVC --> EMAIL_SVC
    
    SERVICES --> AUTH_SVC
    SERVICES --> CUSTOMER_SVC
    SERVICES --> SIM_SVC
    SERVICES --> OCR_SVC
    SERVICES --> USER_SVC
    
    MODELS --> USER_MODEL
    MODELS --> CUSTOMER_MODEL
    MODELS --> SIM_MODEL
    MODELS --> TEAM_MODEL
```

## Database Relationship Diagram

```mermaid
erDiagram
    USERS {
        bigint id PK
        string name
        string email UK
        string password
        string type
        boolean status
        string phone
        string address
        bigint country_id FK
        bigint city_id FK
        bigint state_id FK
        bigint parent_id FK
        bigint user_type_id FK
        timestamp created_at
        timestamp updated_at
    }
    
    USER_TYPES {
        bigint id PK
        string name
        bigint role_id FK
        bigint superior_id FK
        timestamp created_at
        timestamp updated_at
    }
    
    CUSTOMERS {
        bigint id PK
        string name
        string email
        string phone_number
        string nationality
        date birth_date
        string document_number UK
        date document_expiry_date
        string submission_status
        string type
        boolean is_blocked
        boolean is_citizen
        bigint created_by FK
        timestamp created_at
        timestamp updated_at
    }
    
    SIM_CARDS {
        bigint id PK
        string sim_number
        string serial_number
        string puk
        string status
        bigint customer_id FK
        bigint supervisor_id FK
        bigint created_by FK
        timestamp created_at
        timestamp updated_at
    }
    
    TEAMS {
        bigint id PK
        string name
        bigint manager_id FK
        timestamp created_at
        timestamp updated_at
    }
    
    SETTING_COUNTRIES {
        bigint id PK
        string name
        timestamp created_at
        timestamp updated_at
    }
    
    SETTING_CITIES {
        bigint id PK
        string name
        bigint country_id FK
        timestamp created_at
        timestamp updated_at
    }
    
    SETTING_STATES {
        bigint id PK
        string name
        bigint city_id FK
        timestamp created_at
        timestamp updated_at
    }
    
    ROLES {
        bigint id PK
        string name
        string guard_name
        timestamp created_at
        timestamp updated_at
    }
    
    PERMISSIONS {
        bigint id PK
        string name
        string guard_name
        timestamp created_at
        timestamp updated_at
    }
    
    TEAM_USER {
        bigint team_id FK
        bigint user_id FK
    }
    
    TEAM_MANAGER {
        bigint team_id FK
        bigint user_id FK
    }
    
    TEAM_AREA {
        bigint team_id FK
        bigint area_id FK
    }
    
    %% Relationships
    USERS ||--o{ USERS : "parent_id"
    USERS }o--|| USER_TYPES : "user_type_id"
    USER_TYPES }o--|| ROLES : "role_id"
    USER_TYPES ||--o{ USER_TYPES : "superior_id"
    
    USERS ||--o{ CUSTOMERS : "created_by"
    CUSTOMERS ||--o{ SIM_CARDS : "customer_id"
    USERS ||--o{ SIM_CARDS : "supervisor_id"
    USERS ||--o{ SIM_CARDS : "created_by"
    
    USERS }o--|| SETTING_COUNTRIES : "country_id"
    USERS }o--|| SETTING_CITIES : "city_id"
    USERS }o--|| SETTING_STATES : "state_id"
    
    SETTING_COUNTRIES ||--o{ SETTING_CITIES : "country_id"
    SETTING_CITIES ||--o{ SETTING_STATES : "city_id"
    
    TEAMS ||--o{ TEAM_USER : "team_id"
    USERS ||--o{ TEAM_USER : "user_id"
    TEAMS ||--o{ TEAM_MANAGER : "team_id"
    USERS ||--o{ TEAM_MANAGER : "user_id"
    TEAMS ||--o{ TEAM_AREA : "team_id"
    SETTING_STATES ||--o{ TEAM_AREA : "area_id"
```

This documentation provides a comprehensive overview of the eKYC system's architecture, business logic, and technical implementation. The system demonstrates enterprise-level Laravel development with proper separation of concerns, comprehensive authentication, and robust business logic handling.
