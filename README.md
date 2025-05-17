# Concert-Booking-System-Project
concert-management/
├── config/
│   ├── db.js
│   └── jwt.js
├── controllers/
│   ├── admin/
│   │   ├── authController.js
│   │   ├── categoryController.js
│   │   ├── subCategoryController.js
│   │   ├── bookingController.js
│   │   └── reviewController.js
│   └── user/
│       ├── authController.js
│       ├── concertController.js
│       ├── bookingController.js
│       └── reviewController.js
├── middleware/
│   ├── auth.js
│   ├── adminAuth.js
│   └── errorHandler.js
├── models/
│   ├── User.js
│   ├── Admin.js
│   ├── Category.js
│   ├── SubCategory.js
│   ├── Concert.js (existing)
│   ├── Booking.js
│   └── Review.js
├── repositories/
│   ├── admin/
│   │   ├── authRepository.js
│   │   ├── categoryRepository.js
│   │   └── ...
│   └── user/
│       ├── authRepository.js
│       ├── concertRepository.js
│       └── ...
├── routes/
│   ├── admin/
│   │   ├── authRoutes.js
│   │   ├── categoryRoutes.js
│   │   └── ...
│   └── user/
│       ├── authRoutes.js
│       ├── concertRoutes.js
│       └── ...
├── services/
│   ├── admin/
│   │   ├── authService.js
│   │   ├── categoryService.js
│   │   └── ...
│   └── user/
│       ├── authService.js
│       ├── concertService.js
│       └── ...
├── utils/
│   ├── apiResponse.js
│   ├── logger.js
│   └── ...
├── views/
│   ├── admin/
│   │   ├── auth/
│   │   ├── categories/
│   │   └── ...
│   └── user/
│       ├── auth/
│       ├── concerts/
│       └── ...
└── app.js