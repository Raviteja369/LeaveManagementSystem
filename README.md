# LeaveManagementSystem
LeaveManagementSystem
Solution 'LeaveManagementSystem'
├─── LeaveManagementSystem.sln
├─── src
│   ├─── LeaveManagementSystem.Web (ASP.NET MVC Project)
│   │   ├─── App_Start
│   │   │   ├─── BundleConfig.cs
│   │   │   ├─── FilterConfig.cs
│   │   │   ├─── RouteConfig.cs
│   │   │   ├─── UnityConfig.cs (or other DI container setup)
│   │   ├─── Content (for Bootstrap CSS, etc.)
│   │   ├─── Controllers
│   │   │   ├─── LeaveController.cs
│   │   │   ├─── ManagerController.cs
│   │   │   └─── AccountController.cs (for authentication, if implemented)
│   │   ├─── Models (for ViewModels specific to UI)
│   │   │   ├─── LeaveRequestViewModel.cs
│   │   │   └─── PublicHolidayViewModel.cs
│   │   ├─── Scripts (for Bootstrap JS, jQuery, custom JS)
│   │   ├─── Views
│   │   │   ├─── Shared
│   │   │   ├─── Leave (e.g., Index.cshtml, Create.cshtml, Edit.cshtml)
│   │   │   └─── Manager (e.g., Index.cshtml, ApproveReject.cshtml)
│   │   ├─── Web.config
│   │   └─── Global.asax
│   │
│   ├─── LeaveManagementSystem.Application (Class Library)
│   │   ├─── DTOs
│   │   │   ├─── LeaveRequestDto.cs
│   │   │   └─── EmployeeDto.cs
│   │   ├─── Interfaces
│   │   │   ├─── ILeaveService.cs
│   │   │   └─── IEmployeeService.cs
│   │   ├─── Services
│   │   │   ├─── LeaveService.cs
│   │   │   └─── EmployeeService.cs
│   │   └─── Mappers (e.g., AutoMapper configurations)
│   │
│   ├─── LeaveManagementSystem.Domain (Class Library)
│   │   ├─── Entities
│   │   │   ├─── Employee.cs
│   │   │   ├─── LeaveRequest.cs
│   │   │   ├─── LeaveType.cs
│   │   │   ├─── LeaveStatus.cs
│   │   │   └─── PublicHoliday.cs
│   │   ├─── Interfaces (Repository interfaces)
│   │   │   ├─── IRepository.cs
│   │   │   ├─── IEmployeeRepository.cs
│   │   │   ├─── ILeaveRequestRepository.cs
│   │   │   └─── IPublicHolidayRepository.cs
│   │   ├─── Services (Domain services, e.g., LeaveCalculation)
│   │   │   ├─── LeaveCalculationService.cs
│   │   └─── Exceptions (Custom domain exceptions)
│   │
│   └─── LeaveManagementSystem.Infrastructure (Class Library)
│       ├─── Data (Entity Framework DbContext and Migrations)
│       │   ├─── ApplicationDbContext.cs
│       │   └─── Migrations
│       ├─── Repositories (Implementations of Domain interfaces)
│       │   ├─── Repository.cs (Generic)
│       │   ├─── EmployeeRepository.cs
│       │   ├─── LeaveRequestRepository.cs
│       │   └─── PublicHolidayRepository.cs
│       ├─── Mapping (for Entity Framework configurations)
│       └─── Identity (if using ASP.NET Identity for auth)
│
└─── tests
    ├─── LeaveManagementSystem.Tests (Unit Tests for Application, Domain, Infrastructure)
