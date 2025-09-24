# Shopee Clone - Dự án E-commerce với React TypeScript

## 📋 Tổng quan dự án

Shopee Clone là một ứng dụng thương mại điện tử hoàn chỉnh được xây dựng bằng React TypeScript, mô phỏng các tính năng chính của trang web Shopee. Dự án này được phát triển với mục tiêu học tập và thực hành các công nghệ web hiện đại.

## 🛠️ Công nghệ sử dụng

### Frontend Core

- **React 18** - Thư viện UI chính
- **TypeScript** - Ngôn ngữ lập trình có type safety
- **Vite** - Build tool và dev server nhanh
- **React Router DOM v7** - Routing cho SPA
- **Tailwind CSS** - Framework CSS utility-first
- **PostCSS** - CSS processor

### State Management & Data Fetching

- **TanStack React Query v5** - Server state management và data caching
- **React Context** - Client state management
- **Immer** - Immutable state updates
- **React Query Persist Client** - Persistent query cache

### Form & Validation

- **React Hook Form** - Form management
- **Yup** - Schema validation
- **@hookform/resolvers** - Validation resolvers

### HTTP Client & Authentication

- **Axios** - HTTP client
- **JWT** - JSON Web Tokens cho authentication

### UI/UX Libraries

- **@floating-ui/react** - Positioning library cho tooltips, dropdowns
- **Framer Motion** - Animation library
- **React Toastify** - Toast notifications
- **React Helmet Async** - Document head management
- **DOMPurify** - HTML sanitization
- **Classnames** - Conditional CSS classes

### Development & Testing

- **Vitest** - Testing framework
- **@testing-library/react** - React testing utilities
- **MSW (Mock Service Worker)** - API mocking cho testing
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **Storybook** - Component development environment

### Internationalization

- **i18next** - Internationalization framework
- **react-i18next** - React bindings cho i18next

## 🏗️ Cấu trúc dự án

```
src/
├── @types/                 # Type definitions
├── apis/                   # API service layer
├── assets/                 # Static assets (images, icons)
├── components/             # Reusable UI components
├── constants/              # Application constants
├── contexts/               # React contexts
├── hooks/                  # Custom hooks
├── i18n/                   # Internationalization setup
├── layouts/                # Layout components
├── locales/                # Translation files
├── msw/                    # Mock Service Worker handlers
├── pages/                  # Page components
├── stories/                # Storybook stories
├── types/                  # TypeScript type definitions
├── utils/                  # Utility functions
└── main.tsx               # Application entry point
```

## 🎯 Chức năng chính

### 🔐 Hệ thống Authentication

- **Đăng ký tài khoản**: Form validation với email và password
- **Đăng nhập**: JWT-based authentication
- **Đăng xuất**: Clear token và redirect
- **Quản lý session**: Auto refresh token, persistent login
- **Route protection**: Protected và public routes

### 🛍️ Quản lý sản phẩm

- **Danh sách sản phẩm**:
  - Hiển thị grid layout responsive
  - Lazy loading với Suspense
  - Pagination
  - Product rating và giá cả
- **Chi tiết sản phẩm**:
  - Image slider với zoom effect
  - Thông tin chi tiết (mô tả, giá, đánh giá)
  - Thêm vào giỏ hàng
  - Mua ngay
  - Sản phẩm liên quan

### 🔍 Tìm kiếm và lọc

- **Tìm kiếm**: Search by product name
- **Bộ lọc nâng cao**:
  - Lọc theo danh mục
  - Lọc theo khoảng giá
  - Lọc theo đánh giá
  - Sắp xếp (giá, độ phổ biến, mới nhất)

### 🛒 Giỏ hàng

- **Quản lý giỏ hàng**:
  - Thêm/xóa sản phẩm
  - Cập nhật số lượng
  - Chọn multiple sản phẩm
  - Tính tổng tiền tự động
- **Checkout**: Mua hàng với validation
- **Mini cart**: Preview giỏ hàng trong header

### 👤 Quản lý người dùng

- **Hồ sơ cá nhân**:
  - Cập nhật thông tin (tên, địa chỉ, SĐT)
  - Upload và cập nhật avatar
  - Date picker cho ngày sinh
- **Đổi mật khẩu**: Form validation an toàn
- **Lịch sử mua hàng**:
  - Theo dõi đơn hàng
  - Lọc theo trạng thái đơn hàng
  - Chi tiết từng đơn hàng

### 🌐 Đa ngôn ngữ (i18n)

- **Hỗ trợ**: Tiếng Việt và English
- **Switch language**: Dropdown trong header
- **Persistent**: Lưu ngôn ngữ đã chọn

### 📱 Responsive Design

- **Mobile-first**: Thiết kế tối ưu cho mobile
- **Breakpoints**: SM, MD, LG, XL với Tailwind
- **Touch-friendly**: UI phù hợp với touch devices

## 🔧 Tính năng kỹ thuật

### Performance Optimization

- **Code splitting**: Lazy loading cho routes
- **Image optimization**: Lazy loading images
- **Query caching**: TanStack Query với stale time
- **Bundle analysis**: Rollup visualizer
- **Million.js**: React compiler tối ưu performance

### Error Handling

- **Error Boundary**: Catch và handle React errors
- **API Error**: Axios interceptors
- **Form validation**: Real-time validation
- **Toast notifications**: User-friendly error messages

### Development Experience

- **TypeScript**: Full type safety
- **ESLint + Prettier**: Code quality
- **Storybook**: Component documentation
- **MSW**: API mocking cho development
- **Hot reload**: Fast development cycle

### Testing

- **Unit tests**: Vitest + Testing Library
- **Component tests**: Isolated component testing
- **API mocking**: MSW cho reliable tests
- **Coverage reports**: Test coverage tracking

## 🚀 Cách chạy dự án

### Yêu cầu hệ thống

- Node.js >= 18
- Yarn hoặc npm

### Cài đặt và chạy

```bash
# Clone repository
git clone <repository-url>
cd ShopeeClone

# Cài đặt dependencies
yarn install

# Chạy development server
yarn dev

# Chạy tests
yarn test

# Chạy Storybook
yarn storybook

# Build production
yarn build
```

### Scripts chính

- `yarn dev` - Development server (port 3000)
- `yarn build` - Build production
- `yarn preview` - Preview production build
- `yarn test` - Run tests với Vitest
- `yarn coverage` - Test coverage report
- `yarn storybook` - Chạy Storybook
- `yarn lint` - ESLint checking
- `yarn prettier` - Code formatting

## 🌟 Điểm nổi bật

### Architecture

- **Scalable**: Cấu trúc thư mục rõ ràng, dễ mở rộng
- **Type-safe**: Full TypeScript cho reliability
- **Maintainable**: Clean code với proper separation of concerns
- **Testable**: High test coverage với MSW

### User Experience

- **Fast**: Vite + lazy loading + query caching
- **Responsive**: Mobile-first design
- **Accessible**: Screen reader friendly
- **Intuitive**: Familiar e-commerce UX patterns

### Developer Experience

- **Modern tooling**: Vite, Vitest, Storybook
- **Code quality**: ESLint, Prettier, TypeScript
- **Documentation**: Storybook cho components
- **Debugging**: React Query Devtools

## 📝 API Integration

Dự án tích hợp với backend API REST với các endpoints:

### Authentication

- `POST /register` - Đăng ký tài khoản
- `POST /login` - Đăng nhập
- `POST /logout` - Đăng xuất
- `POST /refresh-access-token` - Refresh token

### Products

- `GET /products` - Danh sách sản phẩm (có pagination, filtering)
- `GET /products/:id` - Chi tiết sản phẩm
- `GET /categories` - Danh mục sản phẩm

### Cart & Purchases

- `POST /purchases/add-to-cart` - Thêm vào giỏ hàng
- `GET /purchases` - Lấy giỏ hàng
- `PUT /purchases/update-purchase` - Cập nhật giỏ hàng
- `DELETE /purchases` - Xóa khỏi giỏ hàng
- `POST /purchases/buy-products` - Mua hàng

### User Management

- `GET /me` - Thông tin user
- `PUT /user` - Cập nhật profile
- `POST /user/upload-avatar` - Upload avatar

## 🎨 Design System

Dự án sử dụng design system tutạcbij với:

- **Colors**: Orange theme chính, gray scale
- **Typography**: Responsive font sizes
- **Spacing**: Consistent padding/margin
- **Components**: Reusable UI components
- **Icons**: SVG icons tối ưu
- **Animations**: Subtle micro-interactions

## 🔒 Security

- **XSS Protection**: DOMPurify sanitization
- **CSRF**: Token-based authentication
- **Input Validation**: Client và server-side validation
- **Secure Headers**: Proper HTTP headers
- **Environment Variables**: Sensitive data protection

## 🚀 Deployment

Dự án được cấu hình cho deployment trên:

- **Vercel**: Static hosting với `vercel.json`
- **Build optimization**: Tree shaking, code splitting
- **Environment setup**: Production configs

---

_Dự án được phát triển cho mục đích học tập và thực hành các công nghệ React/TypeScript hiện đại. Đây là một ví dụ hoàn chỉnh về cách xây dựng một ứng dụng e-commerce scale production._
