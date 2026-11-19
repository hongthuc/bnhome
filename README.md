<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <title>BN HOME - Công Ty TNHH Tư Vấn Thiết Kế Kiến Trúc - Xây Dựng Đà Nẵng</title>
    <meta name="description" content="CÔNG TY TNHH TƯ VẤN THIẾT KẾ KIẾN TRÚC - XÂY DỰNG BN HOME (bnhome.com) - Chuyên thiết kế kiến trúc, nội thất, thi công phần thô, hoàn thiện và xây nhà trọn gói tại Đà Nẵng. Hotline: 0934.954.832.">

    <!-- Favicon & Ảnh Thumbnail Logo khi chia sẻ đường link website -->
    <link rel="icon" type="image/png" href="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w256">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://bnhome.com/">
    <meta property="og:site_name" content="BN HOME - bnhome.com">
    <meta property="og:title" content="CÔNG TY TNHH TƯ VẤN THIẾT KẾ KIẾN TRÚC - XÂY DỰNG BN HOME">
    <meta property="og:description" content="Thiết kế kiến trúc – Nội thất – Thi công xây dựng trọn gói chuyên nghiệp tại Đà Nẵng. Hotline: 0934.954.832.">
    <meta property="og:image" content="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w1000">
    <meta property="og:image:width" content="1000">
    <meta property="og:image:height" content="1000">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="CÔNG TY TNHH TƯ VẤN THIẾT KẾ KIẾN TRÚC - XÂY DỰNG BN HOME">
    <meta name="twitter:description" content="Thiết kế kiến trúc – Thi công xây dựng trọn gói uy tín tại Đà Nẵng.">
    <meta name="twitter:image" content="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w1000">

    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Cấu hình màu chủ đạo đồng bộ nhận diện logo BN HOME & bố cục Flatsome -->
    <style>
        :root {
            /* Dễ dàng đồng bộ vào Flatsome -> Theme Options -> Style -> Colors */
            --bn-primary: #143250;       /* Xanh kiến trúc đậm theo tông nhận diện chuyên nghiệp */
            --bn-primary-dark: #0D2238;  /* Xanh đậm footer & hover */
            --bn-accent: #C8933B;        /* Vàng đồng sang trọng làm điểm nhấn */
            --bn-accent-hover: #B07E2C;  /* Vàng đồng hover */
            --bn-bg-light: #F6F8FA;      /* Nền xám sáng phân tách section UXBuilder */
            --bn-text: #222B35;          /* Màu chữ nội dung dễ đọc */
            --bn-muted: #5A6776;         /* Màu chữ phụ */
            --bn-border: #E5EAF0;        /* Màu viền tinh tế */
        }

        *, *::before, *::after {
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            overflow-x: hidden;
            width: 100%;
            max-width: 100%;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            color: var(--bn-text);
            background-color: #FFFFFF;
            margin: 0;
            padding: 0;
            width: 100%;
            max-width: 100%;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
        }

        /* Khung bao chuẩn UXBuilder Flatsome: Chiều ngang máy tính đúng 95% màn hình, không lệch phải */
        .bn-container {
            width: 100%;
            max-width: 100%;
            margin-left: auto;
            margin-right: auto;
            padding-left: 12px;
            padding-right: 12px;
        }

        @media (min-width: 640px) {
            .bn-container {
                padding-left: 18px;
                padding-right: 18px;
            }
        }

        @media (min-width: 1024px) {
            .bn-container {
                width: 95%;
                max-width: 95%;
                padding-left: 0;
                padding-right: 0;
            }
        }

        /* Màu tiện ích Flatsome */
        .bg-bn-primary { background-color: var(--bn-primary); }
        .bg-bn-primary-dark { background-color: var(--bn-primary-dark); }
        .bg-bn-accent { background-color: var(--bn-accent); }
        .bg-bn-light { background-color: var(--bn-bg-light); }
        .text-bn-primary { color: var(--bn-primary); }
        .text-bn-accent { color: var(--bn-accent); }
        .border-bn-primary { border-color: var(--bn-primary); }
        .border-bn-accent { border-color: var(--bn-accent); }

        /* Tiêu đề Section chuẩn Flatsome UXBuilder */
        .section-heading {
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }
        .section-heading::after {
            content: "";
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            bottom: 0;
            width: 56px;
            height: 3px;
            background-color: var(--bn-accent);
            border-radius: 999px;
        }
        .section-heading-left::after {
            left: 0;
            transform: none;
        }

        /* Menu đa cấp Dropdown trên máy tính */
        .nav-dropdown {
            opacity: 0;
            visibility: hidden;
            transform: translateY(6px);
            transition: all 0.2s ease;
            pointer-events: none;
        }
        .nav-item:hover .nav-dropdown,
        .nav-item:focus-within .nav-dropdown {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
            pointer-events: auto;
        }

        /* Hệ thống 2 Banner tự trượt kích thước bằng nhau tuyệt đối (CSS Grid chồng lớp) */
        .hero-slider-stage {
            display: grid;
            grid-template-columns: 1fr;
            width: 100%;
            overflow: hidden;
            position: relative;
        }
        .hero-slide {
            grid-row: 1 / 2;
            grid-column: 1 / 2;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.65s ease, visibility 0.65s ease;
            position: relative;
            width: 100%;
            min-height: 350px;
        }
        @media (min-width: 640px) {
            .hero-slide {
                min-height: 430px;
            }
        }
        @media (min-width: 1024px) {
            .hero-slide {
                min-height: 510px;
            }
        }
        .hero-slide.active {
            opacity: 1;
            visibility: visible;
            z-index: 2;
        }

        /* Thẻ sản phẩm / dự án chuẩn Flatsome Box */
        .project-card {
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .project-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 24px -8px rgba(20, 50, 80, 0.14);
        }
        .project-card img {
            transition: transform 0.45s ease;
        }
        .project-card:hover img {
            transform: scale(1.04);
        }

        /* Nút danh mục lọc gọn gàng, tuyệt đối không xuống dòng bên trong tên danh mục */
        .cat-pill {
            white-space: nowrap;
            transition: all 0.2s ease;
        }
        .cat-pill.active {
            background-color: var(--bn-primary);
            color: #FFFFFF;
            border-color: var(--bn-primary);
        }
        .cat-pill:not(.active):hover {
            border-color: var(--bn-accent);
            color: var(--bn-primary);
            background-color: #FFFBF4;
        }

        /* Hiệu ứng nhịp nhẹ cho nút Hotline nổi bật */
        @keyframes bnPulse {
            0% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.55); }
            70% { box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
            100% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
        }
        .hotline-pulse {
            animation: bnPulse 2s infinite;
        }

        /* Ẩn thanh cuộn phụ nhưng vẫn giữ cuộn mượt */
        .no-scrollbar::-webkit-scrollbar { display: none; }
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    </style>
</head>
<body id="trang-chu">

    <!-- =========================================================
         TOP BAR (Chuẩn Flatsome - Không có thanh công cụ chỉnh sửa)
         ========================================================= -->
    <div class="bg-bn-primary text-white text-[12px] py-2 border-b border-white/10">
        <div class="bn-container flex flex-wrap items-center justify-between gap-2">
            <div class="flex items-center gap-3 sm:gap-5 flex-wrap">
                <a href="tel:0934954832" class="inline-flex items-center gap-1.5 hover:text-[#F0C97A] transition-colors font-medium">
                    <svg class="w-3.5 h-3.5 shrink-0" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/></svg>
                    <span>0934.954.832</span>
                </a>
                <span class="hidden sm:inline text-white/30">|</span>
                <span class="hidden sm:inline-flex items-center gap-1.5 text-white/90">
                    <svg class="w-3.5 h-3.5 shrink-0" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                    <span>Phường Thanh Khê, TP Đà Nẵng</span>
                </span>
            </div>
            <div class="flex items-center gap-3 text-white/90">
                <a href="https://bnhome.com" class="hover:text-[#F0C97A] transition-colors font-medium">bnhome.com</a>
                <span class="text-white/30">|</span>
                <a href="https://www.facebook.com/nguyen.phanbao" target="_blank" rel="noopener noreferrer" class="hover:text-[#F0C97A] transition-colors">Facebook</a>
                <span class="text-white/30">|</span>
                <a href="https://zalo.me/0934954832" target="_blank" rel="noopener noreferrer" class="hover:text-[#F0C97A] transition-colors">Zalo</a>
            </div>
        </div>
    </div>

    <!-- =========================================================
         HEADER CHÍNH (Logo gọn nhỏ, Menu 1 hàng không xuống dòng, không để nút gọi ngay tránh tràn viền)
         ========================================================= -->
    <header class="sticky top-0 z-40 bg-white/98 backdrop-blur-md border-b border-gray-200 shadow-sm">
        <div class="bn-container flex items-center justify-between h-[64px] lg:h-[72px] gap-3">
            <!-- Logo BN HOME chỉnh gọn nhỏ -->
            <a href="#trang-chu" class="flex items-center gap-2 shrink-0 min-w-0">
                <img
                    src="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w400"
                    data-drive-id="18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE"
                    onerror="handleDriveError(this)"
                    alt="Logo BN HOME"
                    class="h-10 sm:h-11 lg:h-12 w-auto max-w-[115px] object-contain rounded"
                >
                <div class="leading-tight">
                    <div class="text-[15px] sm:text-[16px] font-extrabold text-bn-primary tracking-tight whitespace-nowrap">BN HOME</div>
                    <div class="text-[10px] font-medium text-gray-500 uppercase tracking-wider whitespace-nowrap">Kiến Trúc & Xây Dựng</div>
                </div>
            </a>

            <!-- Menu Desktop: viết liền trên 1 hàng, chữ nhỏ gọn, không xuống dòng tên danh mục -->
            <nav class="hidden lg:flex items-center justify-end flex-nowrap gap-3 xl:gap-5 min-w-0" aria-label="Menu chính">
                <a href="#trang-chu" class="text-[12px] xl:text-[13px] font-semibold uppercase text-bn-primary hover:text-bn-accent transition-colors whitespace-nowrap py-2">Trang chủ</a>
                <a href="#gioi-thieu" class="text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap py-2">Giới thiệu</a>

                <!-- Dropdown: Công trình thực tế -->
                <div class="nav-item relative py-2">
                    <a href="#cong-trinh-thuc-te" class="inline-flex items-center gap-1 text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap">
                        <span>Công trình thực tế</span>
                        <svg class="w-3 h-3 shrink-0" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
                    </a>
                    <div class="nav-dropdown absolute left-0 top-full w-60 bg-white border border-gray-200 rounded-lg shadow-lg py-2 z-50">
                        <a href="#cong-trinh-thuc-te" onclick="filterConstruction('khach-san-can-ho')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Khách sạn – Căn hộ – Phòng trọ</a>
                        <a href="#cong-trinh-thuc-te" onclick="filterConstruction('biet-thu')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Biệt thự</a>
                        <a href="#cong-trinh-thuc-te" onclick="filterConstruction('nha-pho')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Nhà phố</a>
                        <a href="#cong-trinh-thuc-te" onclick="filterConstruction('van-phong')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Văn phòng</a>
                    </div>
                </div>

                <!-- Dropdown: Lĩnh vực hoạt động -->
                <div class="nav-item relative py-2">
                    <a href="#linh-vuc-hoat-dong" class="inline-flex items-center gap-1 text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap">
                        <span>Lĩnh vực</span>
                        <svg class="w-3 h-3 shrink-0" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
                    </a>
                    <div class="nav-dropdown absolute left-0 top-full w-60 bg-white border border-gray-200 rounded-lg shadow-lg py-2 z-50">
                        <a href="#linh-vuc-hoat-dong" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Thiết kế Kiến trúc – Nội thất</a>
                        <a href="#linh-vuc-hoat-dong" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Thi công phần thô</a>
                        <a href="#linh-vuc-hoat-dong" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Thi công hoàn thiện</a>
                        <a href="#linh-vuc-hoat-dong" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Thi công nội thất</a>
                    </div>
                </div>

                <a href="#du-an-da-nang" class="text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap py-2">Dự án Đà Nẵng</a>

                <!-- Dropdown: Mẫu thiết kế -->
                <div class="nav-item relative py-2">
                    <a href="#du-an-da-nang" class="inline-flex items-center gap-1 text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap">
                        <span>Mẫu thiết kế</span>
                        <svg class="w-3 h-3 shrink-0" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
                    </a>
                    <div class="nav-dropdown absolute left-0 top-full w-56 bg-white border border-gray-200 rounded-lg shadow-lg py-2 z-50">
                        <a href="#du-an-da-nang" onclick="filterDaNang('nha-pho-dn')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Mẫu thiết kế nhà phố</a>
                        <a href="#du-an-da-nang" onclick="filterDaNang('biet-thu-dn')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Mẫu thiết kế biệt thự</a>
                        <a href="#du-an-da-nang" onclick="filterDaNang('noi-that-dn')" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Mẫu thiết kế nội thất</a>
                    </div>
                </div>

                <!-- Dropdown: Báo giá -->
                <div class="nav-item relative py-2">
                    <a href="#bao-gia" class="inline-flex items-center gap-1 text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap">
                        <span>Báo giá</span>
                        <svg class="w-3 h-3 shrink-0" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
                    </a>
                    <div class="nav-dropdown absolute right-0 top-full w-60 bg-white border border-gray-200 rounded-lg shadow-lg py-2 z-50">
                        <a href="#bao-gia" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Báo giá thiết kế kiến trúc</a>
                        <a href="#bao-gia" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Báo giá thi công phần thô</a>
                        <a href="#bao-gia" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Báo giá thi công hoàn thiện</a>
                        <a href="#bao-gia" class="block px-4 py-2 text-[13px] text-gray-700 hover:bg-bn-light hover:text-bn-primary font-medium">Báo giá thi công trọn gói</a>
                    </div>
                </div>

                <a href="#tin-tuc" class="text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap py-2">Tin tức</a>
                <a href="#lien-he" class="text-[12px] xl:text-[13px] font-semibold uppercase text-gray-700 hover:text-bn-accent transition-colors whitespace-nowrap py-2">Liên hệ</a>
            </nav>

            <!-- Nút mở Menu Mobile -->
            <button id="mobileMenuBtn" type="button" aria-label="Mở menu điều hướng" class="lg:hidden inline-flex items-center justify-center p-2.5 rounded-lg border border-gray-200 text-bn-primary hover:bg-gray-50 active:bg-gray-100">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16"/></svg>
            </button>
        </div>
    </header>

    <!-- =========================================================
         MENU MOBILE DRAWER (Tương thích mượt trên điện thoại)
         ========================================================= -->
    <div id="mobileDrawer" class="fixed inset-0 z-50 hidden">
        <div id="mobileBackdrop" class="absolute inset-0 bg-black/50 backdrop-blur-[1px]"></div>
        <div class="relative w-[84%] max-w-[320px] h-full bg-white shadow-2xl flex flex-col overflow-y-auto">
            <div class="flex items-center justify-between p-4 border-b border-gray-200 bg-bn-primary text-white">
                <div class="flex items-center gap-2.5">
                    <img
                        src="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w256"
                        data-drive-id="18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE"
                        onerror="handleDriveError(this)"
                        alt="BN HOME"
                        class="h-8 w-auto bg-white rounded p-0.5 object-contain"
                    >
                    <span class="font-bold text-sm tracking-wide">BN HOME</span>
                </div>
                <button id="closeMobileBtn" type="button" aria-label="Đóng menu" class="p-2 rounded-lg hover:bg-white/10">
                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
                </button>
            </div>
            <nav class="flex-1 p-3 space-y-1 text-[14px]">
                <a href="#trang-chu" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-bn-primary hover:bg-bn-light">Trang chủ</a>
                <a href="#gioi-thieu" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Giới thiệu</a>
                <a href="#linh-vuc-hoat-dong" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Lĩnh vực hoạt động</a>
                <a href="#cong-trinh-thuc-te" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Công trình thực tế</a>
                <a href="#du-an-da-nang" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Dự án tại Đà Nẵng</a>
                <a href="#bao-gia" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Báo giá & Tư vấn</a>
                <a href="#tin-tuc" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Tin tức & Kiến thức</a>
                <a href="#doi-tac" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Đối tác chiến lược</a>
                <a href="#lien-he" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-lg font-semibold text-gray-700 hover:bg-bn-light">Liên hệ & Bản đồ</a>
            </nav>
            <div class="p-4 border-t border-gray-200 bg-bn-light text-xs text-gray-600 space-y-1.5">
                <p class="font-bold text-bn-primary">Hotline: 0934.954.832</p>
                <p>Thửa đất số 455, TBĐ số 11, Tổ 31, Phường Thanh Khê, TP Đà Nẵng</p>
            </div>
        </div>
    </div>

    <main class="w-full overflow-x-hidden">

        <!-- =========================================================
             SECTION 1: 2 BANNER TỰ TRƯỢT CHUYÊN NGHIỆP KÍCH THƯỚC BẰNG NHAU
             Hình ảnh & chữ nằm hoàn toàn trong banner, cách xa viền, không mất chữ trên Mobile & PC
             ========================================================= -->
        <section class="w-full bg-white py-3 sm:py-4">
            <div class="bn-container">
                <div class="relative rounded-xl overflow-hidden shadow-md border border-gray-200 bg-bn-primary-dark">
                    <div id="heroSlider" class="hero-slider-stage">

                        <!-- SLIDE 1 -->
                        <div class="hero-slide active flex items-center">
                            <!-- Ảnh nền nằm trọn trong banner -->
                            <img
                                src="https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w1600"
                                data-drive-id="157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT"
                                onerror="handleDriveError(this)"
                                alt="Thiết kế kiến trúc và thi công xây dựng trọn gói BN HOME"
                                class="absolute inset-0 w-full h-full object-cover object-center"
                            >
                            <!-- Lớp phủ chuyển sắc đảm bảo chữ tương phản sắc nét -->
                            <div class="absolute inset-0 bg-gradient-to-r from-[#0D2238]/92 via-[#0D2238]/76 to-[#0D2238]/35"></div>
                            <!-- Vùng chữ cách xa viền ảnh banner (padding rộng rãi cho cả mobile và desktop) -->
                            <div class="relative z-10 w-full px-10 sm:px-16 md:px-20 lg:px-24 py-10 sm:py-14 md:py-16">
                                <div class="max-w-2xl text-white">
                                    <p class="text-[11px] sm:text-xs md:text-sm font-semibold uppercase tracking-[0.18em] text-[#F0C97A] mb-2.5 sm:mb-3">
                                        BN HOME • KIẾN TRÚC & XÂY DỰNG ĐÀ NẴNG
                                    </p>
                                    <h1 class="text-[20px] sm:text-[30px] md:text-[38px] lg:text-[42px] font-extrabold leading-[1.24] tracking-tight mb-3 sm:mb-4">
                                        Nâng Tầm Không Gian Sống Từ Giá Trị Thật
                                    </h1>
                                    <p class="text-[13px] sm:text-[15px] md:text-[16px] text-white/90 leading-relaxed mb-5 sm:mb-7 max-w-xl">
                                        Đồng bộ từ tư duy thiết kế kiến trúc, tối ưu công năng đến thi công xây dựng chuẩn mực, bền vững theo thời gian cho từng tổ ấm tại Đà Nẵng.
                                    </p>
                                    <div class="flex flex-wrap items-center gap-3">
                                        <a href="#bao-gia" class="inline-flex items-center justify-center px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg bg-bn-accent hover:bg-[#B07E2C] text-white text-[13px] sm:text-sm font-semibold transition-colors shadow-sm">
                                            Nhận báo giá miễn phí
                                        </a>
                                        <a href="#du-an-da-nang" class="inline-flex items-center justify-center px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/40 text-[13px] sm:text-sm font-semibold transition-colors">
                                            Xem dự án Đà Nẵng
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- SLIDE 2 -->
                        <div class="hero-slide flex items-center">
                            <img
                                src="https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w1600"
                                data-drive-id="13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz"
                                onerror="handleDriveError(this)"
                                alt="Thi công xây dựng thực tế nhà phố biệt thự căn hộ BN HOME"
                                class="absolute inset-0 w-full h-full object-cover object-center"
                            >
                            <div class="absolute inset-0 bg-gradient-to-r from-[#0D2238]/92 via-[#0D2238]/76 to-[#0D2238]/35"></div>
                            <div class="relative z-10 w-full px-10 sm:px-16 md:px-20 lg:px-24 py-10 sm:py-14 md:py-16">
                                <div class="max-w-2xl text-white">
                                    <p class="text-[11px] sm:text-xs md:text-sm font-semibold uppercase tracking-[0.18em] text-[#F0C97A] mb-2.5 sm:mb-3">
                                        AN TOÀN • CHẤT LƯỢNG • ĐÚNG TIẾN ĐỘ
                                    </p>
                                    <h2 class="text-[20px] sm:text-[30px] md:text-[38px] lg:text-[42px] font-extrabold leading-[1.24] tracking-tight mb-3 sm:mb-4">
                                        Thi Công Trọn Gói Chuyên Nghiệp – Chìa Khóa Trao Tay
                                    </h2>
                                    <p class="text-[13px] sm:text-[15px] md:text-[16px] text-white/90 leading-relaxed mb-5 sm:mb-7 max-w-xl">
                                        Kiểm soát chặt chẽ vật tư, kết cấu và tiến độ công trình. Nhà phố, biệt thự, khách sạn, căn hộ dịch vụ với giải pháp tối ưu chi phí cho chủ đầu tư.
                                    </p>
                                    <div class="flex flex-wrap items-center gap-3">
                                        <a href="#cong-trinh-thuc-te" class="inline-flex items-center justify-center px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg bg-bn-accent hover:bg-[#B07E2C] text-white text-[13px] sm:text-sm font-semibold transition-colors shadow-sm">
                                            Công trình thực tế
                                        </a>
                                        <a href="tel:0934954832" class="inline-flex items-center justify-center px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg bg-white/15 hover:bg-white/25 text-white border border-white/40 text-[13px] sm:text-sm font-semibold transition-colors">
                                            Tư vấn: 0934.954.832
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>

                    </div>

                    <!-- Nút điều hướng trái / phải nằm gọn trong banner -->
                    <button type="button" onclick="prevSlide()" aria-label="Banner trước" class="absolute left-2 sm:left-3 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-bn-accent text-white flex items-center justify-center transition-colors">
                        <svg class="w-4 h-4 sm:w-5 sm:h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 19l-7-7 7-7"/></svg>
                    </button>
                    <button type="button" onclick="nextSlide()" aria-label="Banner tiếp theo" class="absolute right-2 sm:right-3 top-1/2 -translate-y-1/2 z-20 w-8 h-8 sm:w-10 sm:h-10 rounded-full bg-black/35 hover:bg-bn-accent text-white flex items-center justify-center transition-colors">
                        <svg class="w-4 h-4 sm:w-5 sm:h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7"/></svg>
                    </button>

                    <!-- Chấm chỉ báo 2 Slide -->
                    <div class="absolute bottom-3.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
                        <button type="button" onclick="goToSlide(0)" id="dot-0" aria-label="Slide 1" class="w-7 h-2 rounded-full bg-bn-accent transition-all"></button>
                        <button type="button" onclick="goToSlide(1)" id="dot-1" aria-label="Slide 2" class="w-2.5 h-2 rounded-full bg-white/55 hover:bg-white transition-all"></button>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 2: DỊCH VỤ TIÊU BIỂU (3 CỘT CHUẨN TÍN TRƯỜNG THỊNH / FLATSOME)
             ========================================================= -->
        <section id="linh-vuc-hoat-dong" class="py-10 sm:py-14 bg-white">
            <div class="bn-container">
                <div class="text-center mb-8 sm:mb-10">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Dịch Vụ Tiêu Biểu
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        Giải pháp toàn diện từ tư vấn thiết kế kiến trúc, thi công xây dựng đến hoàn thiện nội thất đồng bộ.
                    </p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-5 lg:gap-6">
                    <!-- Dịch vụ 1: Thiết kế -->
                    <div class="project-card bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] w-full overflow-hidden bg-gray-100">
                            <img
                                src="https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w900"
                                data-drive-id="1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff"
                                onerror="handleDriveError(this)"
                                alt="Thiết kế kiến trúc và nội thất BN HOME"
                                class="w-full h-full object-cover"
                            >
                        </div>
                        <div class="p-5 flex-1 flex flex-col">
                            <h3 class="text-[16px] sm:text-[18px] font-bold text-bn-primary uppercase mb-2">Thiết Kế Kiến Trúc – Nội Thất</h3>
                            <p class="text-[13.5px] text-gray-600 leading-relaxed flex-1">
                                Tư vấn thiết kế nhà phố, biệt thự, khách sạn, căn hộ tối ưu công năng sử dụng, hài hòa ánh sáng tự nhiên và thẩm mỹ hiện đại bền vững.
                            </p>
                            <a href="#bao-gia" class="mt-4 inline-flex items-center gap-1.5 text-[13px] font-semibold text-bn-accent hover:text-bn-primary transition-colors">
                                <span>Xem chi tiết & báo giá</span>
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7"/></svg>
                            </a>
                        </div>
                    </div>

                    <!-- Dịch vụ 2: Thi công -->
                    <div class="project-card bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] w-full overflow-hidden bg-gray-100">
                            <img
                                src="https://drive.google.com/thumbnail?id=1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR&sz=w900"
                                data-drive-id="1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR"
                                onerror="handleDriveError(this)"
                                alt="Thi công phần thô và trọn gói BN HOME"
                                class="w-full h-full object-cover"
                            >
                        </div>
                        <div class="p-5 flex-1 flex flex-col">
                            <h3 class="text-[16px] sm:text-[18px] font-bold text-bn-primary uppercase mb-2">Thi Công Phần Thô & Trọn Gói</h3>
                            <p class="text-[13.5px] text-gray-600 leading-relaxed flex-1">
                                Quy trình thi công chuẩn kỹ thuật, giám sát kết cấu chặt chẽ từng công đoạn, cam kết đúng vật tư, an toàn lao động và đúng tiến độ bàn giao.
                            </p>
                            <a href="#bao-gia" class="mt-4 inline-flex items-center gap-1.5 text-[13px] font-semibold text-bn-accent hover:text-bn-primary transition-colors">
                                <span>Xem chi tiết & báo giá</span>
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7"/></svg>
                            </a>
                        </div>
                    </div>

                    <!-- Dịch vụ 3: Nội thất -->
                    <div class="project-card bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                        <div class="aspect-[16/10] w-full overflow-hidden bg-gray-100">
                            <img
                                src="https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w900"
                                data-drive-id="1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz"
                                onerror="handleDriveError(this)"
                                alt="Thi công hoàn thiện và nội thất BN HOME"
                                class="w-full h-full object-cover"
                            >
                        </div>
                        <div class="p-5 flex-1 flex flex-col">
                            <h3 class="text-[16px] sm:text-[18px] font-bold text-bn-primary uppercase mb-2">Thi Công Hoàn Thiện & Nội Thất</h3>
                            <p class="text-[13.5px] text-gray-600 leading-relaxed flex-1">
                                Sản xuất và lắp đặt nội thất tinh tế, độ hoàn thiện sắc nét, đồng bộ giữa bản vẽ 3D và thực tế thi công mang lại không gian sống tiện nghi.
                            </p>
                            <a href="#bao-gia" class="mt-4 inline-flex items-center gap-1.5 text-[13px] font-semibold text-bn-accent hover:text-bn-primary transition-colors">
                                <span>Xem chi tiết & báo giá</span>
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7"/></svg>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 3: GIỚI THIỆU CÔNG TY BN HOME & THẾ MẠNH CỦA CHÚNG TÔI
             ========================================================= -->
        <section id="gioi-thieu" class="py-12 sm:py-16 bg-bn-light border-y border-gray-200/80">
            <div class="bn-container">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 lg:gap-10 items-center">
                    <!-- Cột ảnh thực tế giới thiệu -->
                    <div class="lg:col-span-5">
                        <div class="grid grid-cols-2 gap-3">
                            <div class="rounded-xl overflow-hidden shadow-sm border border-gray-200 aspect-[4/5] bg-white">
                                <img
                                    src="https://drive.google.com/thumbnail?id=1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k&sz=w800"
                                    data-drive-id="1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k"
                                    onerror="handleDriveError(this)"
                                    alt="Không gian kiến trúc BN HOME"
                                    class="w-full h-full object-cover"
                                >
                            </div>
                            <div class="rounded-xl overflow-hidden shadow-sm border border-gray-200 aspect-[4/5] bg-white mt-5">
                                <img
                                    src="https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w800"
                                    data-drive-id="1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv"
                                    onerror="handleDriveError(this)"
                                    alt="Thực tế thi công BN HOME"
                                    class="w-full h-full object-cover"
                                >
                            </div>
                        </div>
                    </div>

                    <!-- Cột nội dung giới thiệu -->
                    <div class="lg:col-span-7">
                        <h2 class="section-heading section-heading-left text-[19px] sm:text-[24px] lg:text-[26px] font-extrabold text-bn-primary uppercase leading-snug mb-5">
                            Công Ty TNHH Tư Vấn Thiết Kế Kiến Trúc – Xây Dựng BN HOME
                        </h2>
                        <p class="text-[14px] sm:text-[15px] text-gray-700 leading-relaxed mb-4">
                            <strong>BN HOME</strong> chuyên tư vấn thiết kế kiến trúc – nội thất và thi công xây dựng các công trình <strong>Nhà phố, Biệt thự, Khách sạn, Căn hộ cho thuê, Văn phòng</strong> tại khu vực Đà Nẵng và miền Trung. Một không gian sống đẹp không chỉ dừng ở bản vẽ 3D, mà giá trị thật nằm ở tư duy tổ chức công năng, chất lượng vật liệu và sự chỉn chu trong từng chi tiết thi công ngoài đời thực.
                        </p>
                        <p class="text-[14px] sm:text-[15px] text-gray-700 leading-relaxed mb-6">
                            Với phương châm đặt chữ <strong>“TÂM”</strong> và tinh thần trách nhiệm lên hàng đầu, đội ngũ kiến trúc sư và kỹ sư BN HOME luôn đồng hành xuyên suốt cùng gia chủ để mỗi công trình đạt chuẩn <strong>“An toàn – Chất lượng – Tiến độ – Bền vững lâu dài”</strong>.
                        </p>

                        <!-- 6 Thế mạnh cốt lõi chuẩn bố cục Flatsome Icon Box -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Kiến trúc sư, kỹ sư giàu kinh nghiệm</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Đội ngũ thiết kế sáng tạo, thi công thực chiến và lành nghề.</p>
                                </div>
                            </div>
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Kiểm soát chặt vật liệu & kết cấu</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Đảm bảo độ chính xác từ phần thô đến hoàn thiện sắc nét.</p>
                                </div>
                            </div>
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Giám sát tiến độ chuẩn xác</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Báo cáo tiến độ thường xuyên, bàn giao công trình đúng cam kết.</p>
                                </div>
                            </div>
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Chi phí hợp lý, minh bạch</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Dự toán rõ ràng theo từng hạng mục, hạn chế tối đa phát sinh.</p>
                                </div>
                            </div>
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Bảo hành công trình dài hạn</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Hỗ trợ nhanh chóng sau bàn giao, đồng hành bền vững cùng gia chủ.</p>
                                </div>
                            </div>
                            <div class="bg-white p-4 rounded-xl border border-gray-200 flex items-start gap-3">
                                <div class="w-9 h-9 rounded-lg bg-bn-primary/10 text-bn-primary flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M18.364 5.636l-3.536 3.536m0 5.656l3.536 3.536M9.172 9.172L5.636 5.636m3.536 9.192l-3.536 3.536M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-5 0a4 4 0 11-8 0 4 4 0 018 0z"/></svg>
                                </div>
                                <div>
                                    <h3 class="text-[14px] font-bold text-bn-primary mb-0.5">Tư vấn miễn phí 24/7</h3>
                                    <p class="text-[12.5px] text-gray-600 leading-snug">Lắng nghe nhu cầu thực tế và đề xuất phương án tối ưu nhất.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 4: CÔNG TRÌNH THI CÔNG THỰC TẾ (9 ẢNH THỰC TẾ TỪ GOOGLE DRIVE)
             Chữ danh mục nhỏ gọn trên 1 hàng, không xuống dòng tên danh mục, 2 cột trên điện thoại, không nhãn dán
             ========================================================= -->
        <section id="cong-trinh-thuc-te" class="py-12 sm:py-16 bg-white">
            <div class="bn-container">
                <div class="text-center mb-6 sm:mb-8">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Công Trình Thi Công Thực Tế
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        Hình ảnh thực tế các hạng mục thi công phần thô, kết cấu, hoàn thiện và bàn giao công trình của BN HOME.
                    </p>
                </div>

                <!-- Thanh danh mục lọc: Chữ nhỏ gọn, viết liền không xuống dòng tên danh mục -->
                <div id="constructionTabs" class="flex flex-wrap items-center justify-center gap-1.5 sm:gap-2 mb-7 sm:mb-8">
                    <button type="button" data-cat="all" onclick="filterConstruction('all')" class="cat-pill active px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold">Tất cả</button>
                    <button type="button" data-cat="nha-pho" onclick="filterConstruction('nha-pho')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Nhà phố</button>
                    <button type="button" data-cat="biet-thu" onclick="filterConstruction('biet-thu')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Biệt thự</button>
                    <button type="button" data-cat="khach-san-can-ho" onclick="filterConstruction('khach-san-can-ho')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Khách sạn – Căn hộ</button>
                    <button type="button" data-cat="van-phong" onclick="filterConstruction('van-phong')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Văn phòng</button>
                </div>

                <!-- Lưới sản phẩm: 2 cột trên điện thoại, 3 cột tablet/desktop -->
                <div id="constructionGrid" class="grid grid-cols-2 md:grid-cols-3 gap-3 sm:gap-5 lg:gap-6">
                    <!-- Được render tự động từ dữ liệu 9 ảnh thi công thực tế -->
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 5: DỰ ÁN TẠI ĐÀ NẴNG (10 ẢNH DỰ ÁN ĐÀ NẴNG TỪ GOOGLE DRIVE)
             2 cột trên điện thoại, tên sản phẩm đầy đủ không bị tràn hay thiếu chữ, không nhãn dán
             ========================================================= -->
        <section id="du-an-da-nang" class="py-12 sm:py-16 bg-bn-light border-y border-gray-200/80">
            <div class="bn-container">
                <div class="text-center mb-6 sm:mb-8">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Các Dự Án Tiêu Biểu Tại Đà Nẵng
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        Tuyển chọn các dự án kiến trúc, nhà phố, biệt thự, căn hộ và nội thất được BN HOME triển khai tại TP Đà Nẵng.
                    </p>
                </div>

                <!-- Danh mục dự án Đà Nẵng nhỏ gọn -->
                <div id="danangTabs" class="flex flex-wrap items-center justify-center gap-1.5 sm:gap-2 mb-7 sm:mb-8">
                    <button type="button" data-cat="all" onclick="filterDaNang('all')" class="cat-pill active px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold">Tất cả dự án</button>
                    <button type="button" data-cat="nha-pho-dn" onclick="filterDaNang('nha-pho-dn')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Nhà phố Đà Nẵng</button>
                    <button type="button" data-cat="biet-thu-dn" onclick="filterDaNang('biet-thu-dn')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Biệt thự Đà Nẵng</button>
                    <button type="button" data-cat="can-ho-dn" onclick="filterDaNang('can-ho-dn')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Căn hộ – Khách sạn</button>
                    <button type="button" data-cat="noi-that-dn" onclick="filterDaNang('noi-that-dn')" class="cat-pill px-3 sm:px-4 py-1.5 rounded-lg border border-gray-200 text-[11.5px] sm:text-[12.5px] font-semibold text-gray-700 bg-white">Thiết kế nội thất</button>
                </div>

                <!-- Lưới dự án Đà Nẵng: 2 cột mobile, 3 cột tablet, 5 cột desktop lớn (10 dự án chia 2 hàng cân đối đẹp) -->
                <div id="danangGrid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-3 sm:gap-4 lg:gap-5">
                    <!-- Được render tự động từ dữ liệu 10 dự án Đà Nẵng -->
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 6: BẢNG THAM KHẢO BÁO GIÁ & FORM YÊU CẦU TƯ VẤN TRANG CHỦ
             ========================================================= -->
        <section id="bao-gia" class="py-12 sm:py-16 bg-white">
            <div class="bn-container">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-7 lg:gap-9 items-start">

                    <!-- Cột trái: Các gói dịch vụ & đơn giá tham khảo (Chuẩn mẫu Tín Trường Thịnh) -->
                    <div class="lg:col-span-5 space-y-4">
                        <div>
                            <h2 class="section-heading section-heading-left text-[20px] sm:text-[24px] font-extrabold text-bn-primary uppercase mb-3">
                                Bảng Giá Dịch Vụ Tham Khảo
                            </h2>
                            <p class="text-[13.5px] sm:text-[14.5px] text-gray-600 leading-relaxed">
                                BN HOME cung cấp báo giá chi tiết, bóc tách rõ từng hạng mục vật tư theo nhu cầu thực tế và ngân sách đầu tư của gia chủ.
                            </p>
                        </div>

                        <div class="space-y-3">
                            <div class="p-4 rounded-xl border border-gray-200 bg-bn-light flex items-center justify-between gap-3">
                                <div>
                                    <h3 class="text-[14px] sm:text-[15px] font-bold text-bn-primary">Thiết kế Kiến trúc – Nội thất</h3>
                                    <p class="text-[12px] text-gray-500 mt-0.5">Hồ sơ 3D ngoại thất, kết cấu, điện nước & nội thất</p>
                                </div>
                                <div class="text-right shrink-0">
                                    <div class="text-[14px] sm:text-[15px] font-extrabold text-bn-accent">Từ 150.000đ</div>
                                    <div class="text-[11px] text-gray-500">/ m²</div>
                                </div>
                            </div>

                            <div class="p-4 rounded-xl border border-gray-200 bg-bn-light flex items-center justify-between gap-3">
                                <div>
                                    <h3 class="text-[14px] sm:text-[15px] font-bold text-bn-primary">Thi công Phần thô & Nhân công</h3>
                                    <p class="text-[12px] text-gray-500 mt-0.5">Vật tư thô chuẩn chất lượng + nhân công hoàn thiện</p>
                                </div>
                                <div class="text-right shrink-0">
                                    <div class="text-[14px] sm:text-[15px] font-extrabold text-bn-accent">Từ 3.600.000đ</div>
                                    <div class="text-[11px] text-gray-500">/ m²</div>
                                </div>
                            </div>

                            <div class="p-4 rounded-xl border border-gray-200 bg-bn-light flex items-center justify-between gap-3">
                                <div>
                                    <h3 class="text-[14px] sm:text-[15px] font-bold text-bn-primary">Thi công Hoàn thiện & Trọn gói</h3>
                                    <p class="text-[12px] text-gray-500 mt-0.5">Chìa khóa trao tay, tặng hồ sơ thiết kế & xin phép</p>
                                </div>
                                <div class="text-right shrink-0">
                                    <div class="text-[14px] sm:text-[15px] font-extrabold text-bn-accent">Từ 5.800.000đ</div>
                                    <div class="text-[11px] text-gray-500">/ m²</div>
                                </div>
                            </div>

                            <div class="p-4 rounded-xl border border-gray-200 bg-bn-light flex items-center justify-between gap-3">
                                <div>
                                    <h3 class="text-[14px] sm:text-[15px] font-bold text-bn-primary">Thi công Nội thất & Cải tạo</h3>
                                    <p class="text-[12px] text-gray-500 mt-0.5">Sản xuất trực tiếp, bảo hành dài hạn theo hạng mục</p>
                                </div>
                                <div class="text-right shrink-0">
                                    <div class="text-[14px] sm:text-[15px] font-extrabold text-bn-accent">Theo dự toán</div>
                                    <div class="text-[11px] text-gray-500">Khảo sát miễn phí</div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Cột phải: Form Yêu Cầu & Báo Giá Miễn Phí -->
                    <div class="lg:col-span-7 bg-bn-primary rounded-2xl p-5 sm:p-8 text-white shadow-lg">
                        <div class="mb-5">
                            <p class="text-[11.5px] font-semibold uppercase tracking-widest text-[#F0C97A] mb-1">Miễn phí tư vấn & khảo sát</p>
                            <h3 class="text-[20px] sm:text-[24px] font-extrabold">Gửi Yêu Cầu Thiết Kế & Báo Giá</h3>
                            <p class="text-[13px] sm:text-[14px] text-white/80 mt-1">
                                Để lại thông tin bên dưới, kỹ sư BN HOME sẽ liên hệ tư vấn phương án và gửi dự toán chi tiết trong thời gian sớm nhất.
                            </p>
                        </div>

                        <form id="quoteForm" class="space-y-3.5" novalidate>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                <div>
                                    <label for="qName" class="block text-[12.5px] font-medium text-white/90 mb-1">Họ và tên *</label>
                                    <input id="qName" type="text" required placeholder="Nhập họ tên của bạn" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                </div>
                                <div>
                                    <label for="qPhone" class="block text-[12.5px] font-medium text-white/90 mb-1">Số điện thoại / Zalo *</label>
                                    <input id="qPhone" type="tel" required placeholder="Ví dụ: 0934.954.832" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                <div>
                                    <label for="qType" class="block text-[12.5px] font-medium text-white/90 mb-1">Loại công trình</label>
                                    <select id="qType" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                        <option value="Nhà phố">Nhà phố</option>
                                        <option value="Biệt thự">Biệt thự</option>
                                        <option value="Khách sạn – Căn hộ cho thuê – Phòng trọ">Khách sạn – Căn hộ – Phòng trọ</option>
                                        <option value="Văn phòng">Văn phòng</option>
                                        <option value="Thi công nội thất">Thi công nội thất</option>
                                        <option value="Cải tạo sửa chữa">Cải tạo sửa chữa</option>
                                    </select>
                                </div>
                                <div>
                                    <label for="qBudget" class="block text-[12.5px] font-medium text-white/90 mb-1">Mức đầu tư dự kiến</label>
                                    <select id="qBudget" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                        <option value="Chưa xác định">Chưa xác định</option>
                                        <option value="Dưới 500 triệu">Dưới 500 triệu</option>
                                        <option value="500 triệu - 1 tỷ">500 triệu – 1 tỷ</option>
                                        <option value="1 tỷ - 2 tỷ">1 tỷ – 2 tỷ</option>
                                        <option value="2 tỷ - 3 tỷ">2 tỷ – 3 tỷ</option>
                                        <option value="Trên 3 tỷ">Trên 3 tỷ</option>
                                    </select>
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                <div>
                                    <label for="qEmail" class="block text-[12.5px] font-medium text-white/90 mb-1">Email (nếu có)</label>
                                    <input id="qEmail" type="email" placeholder="email@domain.com" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                </div>
                                <div>
                                    <label for="qArea" class="block text-[12.5px] font-medium text-white/90 mb-1">Diện tích đất & số tầng</label>
                                    <input id="qArea" type="text" placeholder="Ví dụ: 5x20m, 3 tầng tại Thanh Khê" class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]">
                                </div>
                            </div>

                            <div>
                                <label for="qNote" class="block text-[12.5px] font-medium text-white/90 mb-1">Nhu cầu chi tiết</label>
                                <textarea id="qNote" rows="3" placeholder="Mô tả yêu cầu thiết kế, thi công hoặc thời gian dự kiến khởi công..." class="w-full px-3.5 py-2.5 rounded-lg bg-white text-gray-800 text-[13.5px] focus:outline-none focus:ring-2 focus:ring-[#C8933B]"></textarea>
                            </div>

                            <!-- Thông báo phản hồi trực tiếp (Không dùng alert) -->
                            <div id="quoteFeedback" class="hidden rounded-lg p-3.5 text-[13px] font-medium"></div>

                            <div class="flex flex-col sm:flex-row items-stretch sm:items-center gap-3 pt-1">
                                <button type="submit" class="px-6 py-3 rounded-lg bg-bn-accent hover:bg-[#B07E2C] text-white font-bold text-[14px] transition-colors shadow-sm">
                                    Gửi Yêu Cầu Báo Giá Ngay
                                </button>
                                <span class="text-[12.5px] text-white/80">
                                    Hoặc gọi trực tiếp: <a href="tel:0934954832" class="font-bold text-[#F0C97A] hover:underline">0934.954.832</a>
                                </span>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 7: TIN TỨC & CÁC BÀI VIẾT TRANG CHỦ
             ========================================================= -->
        <section id="tin-tuc" class="py-12 sm:py-16 bg-bn-light border-y border-gray-200/80">
            <div class="bn-container">
                <div class="text-center mb-8">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Tin Tức & Kinh Nghiệm Xây Dựng
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        Cập nhật kiến thức thiết kế, kỹ thuật thi công thực tế và cẩm nang xây nhà tiết kiệm từ đội ngũ kỹ sư BN HOME.
                    </p>
                </div>

                <!-- 2 cột trên điện thoại, 4 cột trên máy tính -->
                <div id="articlesGrid" class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
                    <!-- Render động từ danh sách bài viết -->
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 8: ĐỐI TÁC CHIẾN LƯỢC & NHÀ CUNG CẤP VẬT TƯ
             ========================================================= -->
        <section id="doi-tac" class="py-12 sm:py-14 bg-white">
            <div class="bn-container">
                <div class="text-center mb-8">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Đối Tác Cung Ứng Vật Tư
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        BN HOME hợp tác cùng các thương hiệu vật liệu xây dựng và nội thất hàng đầu nhằm đảm bảo chất lượng công trình bền vững.
                    </p>
                </div>

                <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-6 gap-3 sm:gap-4">
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">HÒA PHÁT</div>
                        <div class="text-[11px] text-gray-500 mt-1">Thép xây dựng</div>
                    </div>
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">SÔNG GIANH</div>
                        <div class="text-[11px] text-gray-500 mt-1">Xi măng cao cấp</div>
                    </div>
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">DULUX / JOTUN</div>
                        <div class="text-[11px] text-gray-500 mt-1">Sơn nội ngoại thất</div>
                    </div>
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">AN CƯỜNG</div>
                        <div class="text-[11px] text-gray-500 mt-1">Gỗ nội thất</div>
                    </div>
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">XINGFA</div>
                        <div class="text-[11px] text-gray-500 mt-1">Nhôm kính cao cấp</div>
                    </div>
                    <div class="p-4 rounded-xl border border-gray-200 bg-bn-light/60 hover:border-bn-accent transition-colors flex flex-col items-center justify-center text-center min-h-[88px]">
                        <div class="text-[15px] font-extrabold text-bn-primary tracking-wide">TOTO / CADIVI</div>
                        <div class="text-[11px] text-gray-500 mt-1">Thiết bị điện nước</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             SECTION 9: BẢN ĐỒ GOOGLE MAP & KẾT NỐI FACEBOOK TRANG CHỦ
             ========================================================= -->
        <section id="lien-he" class="py-12 sm:py-16 bg-bn-light border-t border-gray-200">
            <div class="bn-container">
                <div class="text-center mb-8">
                    <h2 class="section-heading text-[20px] sm:text-[26px] font-extrabold text-bn-primary uppercase tracking-tight">
                        Vị Trí Văn Phòng & Kết Nối Facebook
                    </h2>
                    <p class="text-gray-500 text-[13px] sm:text-[15px] mt-3 max-w-2xl mx-auto">
                        Mời Quý khách hàng ghé văn phòng BN HOME tại Đà Nẵng hoặc kết nối trực tiếp qua Facebook để trao đổi nhanh phương án thiết kế.
                    </p>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-stretch">
                    <!-- Google Map nhúng trực tiếp ra trang chủ -->
                    <div class="lg:col-span-7 bg-white rounded-2xl border border-gray-200 overflow-hidden shadow-sm flex flex-col">
                        <div class="p-4 border-b border-gray-100 flex flex-wrap items-center justify-between gap-2">
                            <div>
                                <h3 class="text-[15px] font-bold text-bn-primary">Bản đồ chỉ đường BN HOME</h3>
                                <p class="text-[12.5px] text-gray-600 mt-0.5">Thửa đất số 455, TBĐ số 11, Tổ 31, Phường Thanh Khê, TP Đà Nẵng</p>
                            </div>
                            <a href="https://www.google.com/maps/search/?api=1&query=Ph%C6%B0%E1%BB%9Dng+Thanh+Kh%C3%AA,+TP+%C4%90%C3%A0+N%E1%BA%B5ng" target="_blank" rel="noopener noreferrer" class="text-[12.5px] font-semibold text-bn-accent hover:underline whitespace-nowrap">
                                Mở Google Maps
                            </a>
                        </div>
                        <div class="w-full h-[300px] sm:h-[340px] flex-1 bg-gray-100">
                            <iframe
                                title="Bản đồ Công ty TNHH Tư vấn Thiết kế Kiến trúc - Xây dựng BN HOME"
                                src="https://maps.google.com/maps?q=Ph%C6%B0%E1%BB%9Dng%20Thanh%20Kh%C3%AA,%20TP%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=15&ie=UTF8&iwloc=&output=embed"
                                class="w-full h-full border-0"
                                loading="lazy"
                                referrerpolicy="no-referrer-when-downgrade">
                            </iframe>
                        </div>
                    </div>

                    <!-- Khối kết nối Facebook chính thức ra ngoài trang chủ -->
                    <div class="lg:col-span-5 bg-white rounded-2xl border border-gray-200 overflow-hidden shadow-sm flex flex-col justify-between">
                        <div>
                            <!-- Ảnh bìa khu vực Facebook -->
                            <div class="relative h-36 sm:h-40 w-full overflow-hidden bg-bn-primary">
                                <img
                                    src="https://drive.google.com/thumbnail?id=1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N&sz=w900"
                                    data-drive-id="1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N"
                                    onerror="handleDriveError(this)"
                                    alt="Kết nối Facebook BN HOME"
                                    class="w-full h-full object-cover opacity-85"
                                >
                                <div class="absolute inset-0 bg-gradient-to-t from-[#0D2238]/85 via-[#0D2238]/30 to-transparent"></div>
                            </div>

                            <!-- Thông tin trang Facebook -->
                            <div class="px-5 pb-5 -mt-10 relative z-10">
                                <div class="flex items-end gap-3.5 mb-3">
                                    <div class="w-20 h-20 rounded-xl bg-white p-1.5 shadow-md border border-gray-200 shrink-0 flex items-center justify-center">
                                        <img
                                            src="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w300"
                                            data-drive-id="18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE"
                                            onerror="handleDriveError(this)"
                                            alt="BN HOME Facebook"
                                            class="w-full h-full object-contain rounded-lg"
                                        >
                                    </div>
                                    <div class="pb-1 min-w-0">
                                        <h3 class="text-[16px] sm:text-[17px] font-extrabold text-bn-primary leading-tight">Phan Bảo Nguyên – BN HOME</h3>
                                        <p class="text-[12px] text-gray-500 mt-0.5 break-all">facebook.com/nguyen.phanbao</p>
                                    </div>
                                </div>

                                <p class="text-[13.5px] text-gray-600 leading-relaxed mb-4">
                                    Theo dõi Facebook chính thức của đại diện <strong>BN HOME</strong> để cập nhật hình ảnh thực tế từng công trình đang thi công tại Đà Nẵng, mẫu thiết kế mới nhất và trao đổi tư vấn trực tiếp.
                                </p>

                                <div class="space-y-2 text-[13px] text-gray-700 bg-bn-light p-3.5 rounded-xl border border-gray-200/80 mb-5">
                                    <div class="flex items-start gap-2">
                                        <span class="font-semibold text-bn-primary shrink-0">Hotline:</span>
                                        <a href="tel:0934954832" class="font-bold text-bn-accent hover:underline">0934.954.832</a>
                                    </div>
                                    <div class="flex items-start gap-2">
                                        <span class="font-semibold text-bn-primary shrink-0">Website:</span>
                                        <span>bnhome.com</span>
                                    </div>
                                    <div class="flex items-start gap-2">
                                        <span class="font-semibold text-bn-primary shrink-0">Mã số thuế:</span>
                                        <span>0402272941</span>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div class="px-5 pb-5 grid grid-cols-2 gap-3">
                            <a href="https://www.facebook.com/nguyen.phanbao" target="_blank" rel="noopener noreferrer" class="inline-flex items-center justify-center gap-2 py-2.5 px-3 rounded-lg bg-[#1877F2] hover:bg-[#1465D1] text-white text-[13px] font-semibold transition-colors">
                                <svg class="w-4 h-4 fill-current shrink-0" viewBox="0 0 24 24"><path d="M22.675 0h-21.35C.597 0 0 .597 0 1.326v21.348C0 23.403.597 24 1.326 24h11.495v-9.294H9.692v-3.622h3.129V8.413c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.463.099 2.795.143v3.24l-1.918.001c-1.504 0-1.795.715-1.795 1.763v2.313h3.587l-.467 3.622h-3.12V24h6.116C23.403 24 24 23.403 24 22.674V1.326C24 .597 23.403 0 22.675 0z"/></svg>
                                <span>Xem Facebook</span>
                            </a>
                            <a href="https://zalo.me/0934954832" target="_blank" rel="noopener noreferrer" class="inline-flex items-center justify-center gap-2 py-2.5 px-3 rounded-lg bg-[#0068FF] hover:bg-[#0055D4] text-white text-[13px] font-semibold transition-colors">
                                <span class="font-extrabold text-[13px]">Zalo</span>
                                <span>Nhắn tư vấn</span>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- =========================================================
         FOOTER CHUẨN FLATSOME (Cấu trúc 3 cột rõ ràng, dễ dựng UXBuilder)
         ========================================================= -->
    <footer class="bg-bn-primary-dark text-white/90 pt-12 pb-6">
        <div class="bn-container">
            <div class="grid grid-cols-1 md:grid-cols-12 gap-8 pb-9 border-b border-white/10">
                <!-- Cột 1: Thông tin doanh nghiệp -->
                <div class="md:col-span-5 space-y-3">
                    <div class="flex items-center gap-3">
                        <img
                            src="https://drive.google.com/thumbnail?id=18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE&sz=w300"
                            data-drive-id="18aFTZJwGEykhm6LIWlj6fNAdUdolx3GE"
                            onerror="handleDriveError(this)"
                            alt="Logo BN HOME"
                            class="h-11 w-auto bg-white rounded-lg p-1 object-contain"
                        >
                        <div>
                            <div class="text-[16px] font-extrabold text-white tracking-wide">BN HOME</div>
                            <div class="text-[11px] text-[#F0C97A] uppercase tracking-wider">bnhome.com</div>
                        </div>
                    </div>
                    <h4 class="text-[14px] font-bold text-white uppercase leading-snug pt-1">
                        CÔNG TY TNHH TƯ VẤN THIẾT KẾ KIẾN TRÚC – XÂY DỰNG BN HOME
                    </h4>
                    <ul class="space-y-2 text-[13px] text-white/80">
                        <li><strong>Địa chỉ:</strong> Thửa đất số 455, TBĐ số 11, Tổ 31, Phường Thanh Khê, TP Đà Nẵng</li>
                        <li><strong>Hotline / Zalo:</strong> <a href="tel:0934954832" class="text-[#F0C97A] font-semibold hover:underline">0934.954.832</a></li>
                        <li><strong>Mã số thuế:</strong> 0402272941</li>
                        <li><strong>Website:</strong> <a href="https://bnhome.com" class="hover:text-[#F0C97A]">bnhome.com</a></li>
                        <li><strong>Facebook:</strong> <a href="https://www.facebook.com/nguyen.phanbao" target="_blank" rel="noopener noreferrer" class="hover:text-[#F0C97A] break-all">facebook.com/nguyen.phanbao</a></li>
                    </ul>
                </div>

                <!-- Cột 2: Lĩnh vực hoạt động -->
                <div class="md:col-span-4 space-y-3">
                    <h4 class="text-[14px] font-bold text-white uppercase tracking-wide border-b border-white/15 pb-2">Lĩnh Vực Hoạt Động</h4>
                    <ul class="space-y-2 text-[13px] text-white/80">
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-[#F0C97A] transition-colors">Thiết kế Kiến trúc – Nội thất</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-[#F0C97A] transition-colors">Thi công phần thô nhà phố, biệt thự</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-[#F0C97A] transition-colors">Thi công hoàn thiện & xây nhà trọn gói</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-[#F0C97A] transition-colors">Thiết kế & thi công nội thất trọn gói</a></li>
                        <li><a href="#du-an-da-nang" class="hover:text-[#F0C97A] transition-colors">Xây dựng khách sạn, căn hộ cho thuê Đà Nẵng</a></li>
                    </ul>
                </div>

                <!-- Cột 3: Truy cập nhanh -->
                <div class="md:col-span-3 space-y-3">
                    <h4 class="text-[14px] font-bold text-white uppercase tracking-wide border-b border-white/15 pb-2">Danh Mục Chính</h4>
                    <ul class="space-y-2 text-[13px] text-white/80">
                        <li><a href="#gioi-thieu" class="hover:text-[#F0C97A] transition-colors">Giới thiệu BN HOME</a></li>
                        <li><a href="#cong-trinh-thuc-te" class="hover:text-[#F0C97A] transition-colors">Công trình thực tế</a></li>
                        <li><a href="#du-an-da-nang" class="hover:text-[#F0C97A] transition-colors">Dự án tại Đà Nẵng</a></li>
                        <li><a href="#bao-gia" class="hover:text-[#F0C97A] transition-colors">Yêu cầu báo giá</a></li>
                        <li><a href="#tin-tuc" class="hover:text-[#F0C97A] transition-colors">Tin tức & Kiến thức</a></li>
                    </ul>
                </div>
            </div>

            <div class="pt-5 text-center text-[12.5px] text-white/65">
                Copyright 2026 © CÔNG TY TNHH TƯ VẤN THIẾT KẾ KIẾN TRÚC – XÂY DỰNG BN HOME (bnhome.com). All rights reserved.
            </div>
        </div>
    </footer>

    <!-- =========================================================
         CÁC NÚT LIÊN HỆ NỔI BẬT: ZALO, FACEBOOK, HOTLINE
         Tương thích tối ưu trên cả máy tính và điện thoại, không gây tràn viền
         ========================================================= -->
    <div class="fixed right-3 bottom-4 sm:right-5 sm:bottom-6 z-40 flex flex-col items-end gap-2.5">
        <!-- Nút Facebook -->
        <a href="https://www.facebook.com/nguyen.phanbao" target="_blank" rel="noopener noreferrer" aria-label="Kết nối Facebook BN HOME" class="group flex items-center gap-2 bg-[#1877F2] hover:bg-[#1465D1] text-white rounded-full shadow-lg p-2.5 sm:px-3.5 sm:py-2.5 transition-all">
            <svg class="w-5 h-5 fill-current shrink-0" viewBox="0 0 24 24"><path d="M22.675 0h-21.35C.597 0 0 .597 0 1.326v21.348C0 23.403.597 24 1.326 24h11.495v-9.294H9.692v-3.622h3.129V8.413c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.463.099 2.795.143v3.24l-1.918.001c-1.504 0-1.795.715-1.795 1.763v2.313h3.587l-.467 3.622h-3.12V24h6.116C23.403 24 24 23.403 24 22.674V1.326C24 .597 23.403 0 22.675 0z"/></svg>
            <span class="hidden sm:inline text-[12.5px] font-bold pr-0.5">Facebook</span>
        </a>

        <!-- Nút Zalo -->
        <a href="https://zalo.me/0934954832" target="_blank" rel="noopener noreferrer" aria-label="Chat Zalo BN HOME" class="group flex items-center gap-2 bg-[#0068FF] hover:bg-[#0055D4] text-white rounded-full shadow-lg p-2.5 sm:px-3.5 sm:py-2.5 transition-all">
            <span class="w-5 h-5 rounded-full bg-white text-[#0068FF] text-[10px] font-black flex items-center justify-center shrink-0">Zalo</span>
            <span class="hidden sm:inline text-[12.5px] font-bold pr-0.5">Chat Zalo</span>
        </a>

        <!-- Nút Hotline -->
        <a href="tel:0934954832" aria-label="Gọi Hotline 0934.954.832" class="hotline-pulse flex items-center gap-2 bg-[#DC2626] hover:bg-[#B91C1C] text-white rounded-full shadow-lg p-2.5 sm:px-4 sm:py-2.5 transition-all">
            <svg class="w-5 h-5 shrink-0" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/></svg>
            <span class="hidden sm:inline text-[13px] font-extrabold tracking-wide">0934.954.832</span>
        </a>
    </div>

    <!-- =========================================================
         MODAL XEM CHI TIẾT CÔNG TRÌNH / BÀI VIẾT
         ========================================================= -->
    <div id="detailModal" class="fixed inset-0 z-50 hidden items-center justify-center p-3 sm:p-5">
        <div onclick="closeModal()" class="absolute inset-0 bg-black/65 backdrop-blur-[2px]"></div>
        <div class="relative z-10 bg-white rounded-2xl shadow-2xl w-full max-w-2xl max-h-[90vh] overflow-y-auto">
            <button type="button" onclick="closeModal()" aria-label="Đóng cửa sổ" class="absolute top-3 right-3 z-20 w-9 h-9 rounded-full bg-black/55 hover:bg-black/80 text-white flex items-center justify-center transition-colors">
                <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
            </button>
            <div id="modalImageWrap" class="w-full aspect-[16/10] bg-gray-100 overflow-hidden">
                <img id="modalImg" src="" alt="" class="w-full h-full object-cover">
            </div>
            <div class="p-5 sm:p-6">
                <p id="modalSub" class="text-[12px] font-semibold uppercase tracking-wider text-bn-accent mb-1"></p>
                <h3 id="modalTitle" class="text-[18px] sm:text-[22px] font-extrabold text-bn-primary leading-snug mb-3"></h3>
                <div id="modalMeta" class="grid grid-cols-2 gap-2.5 bg-bn-light p-3.5 rounded-xl border border-gray-200 text-[12.5px] text-gray-700 mb-4"></div>
                <p id="modalDesc" class="text-[14px] text-gray-600 leading-relaxed mb-5"></p>
                <div class="flex flex-wrap items-center gap-3">
                    <a href="#bao-gia" onclick="closeModal()" class="px-5 py-2.5 rounded-lg bg-bn-primary hover:bg-bn-primary-dark text-white text-[13px] font-semibold transition-colors">
                        Nhận báo giá tương tự
                    </a>
                    <a href="https://zalo.me/0934954832" target="_blank" rel="noopener noreferrer" class="px-5 py-2.5 rounded-lg bg-[#0068FF] hover:bg-[#0055D4] text-white text-[13px] font-semibold transition-colors">
                        Tư vấn qua Zalo
                    </a>
                </div>
            </div>
        </div>
    </div>

    <!-- =========================================================
         JAVASCRIPT: XỬ LÝ ẢNH DRIVE, SLIDER, LỌC DANH MỤC, FORM & MODAL
         ========================================================= -->
    <script>
        // 1. Hàm tạo URL ảnh Google Drive chuẩn & xử lý fallback an toàn khi tải ảnh
        function driveThumb(id, size = 'w900') {
            return `https://drive.google.com/thumbnail?id=${id}&sz=${size}`;
        }

        function handleDriveError(img) {
            const id = img.getAttribute('data-drive-id');
            const step = Number(img.getAttribute('data-err-step') || '0');
            if (step === 0 && id) {
                img.setAttribute('data-err-step', '1');
                img.src = `https://lh3.googleusercontent.com/d/${id}`;
            } else if (step === 1) {
                img.setAttribute('data-err-step', '2');
                img.src = 'https://placehold.co/800x600/143250/FFFFFF?text=BN+HOME';
            }
        }

        // 2. Dữ liệu 9 Công Trình Thi Công Thực Tế (Sử dụng đủ 9 link Google Drive người dùng cung cấp)
        const constructionProjects = [
            {
                id: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
                title: 'Thi Công Trọn Gói Nhà Phố Hiện Đại 3 Tầng – Thanh Khê',
                category: 'nha-pho',
                categoryName: 'Nhà phố',
                location: 'Quận Thanh Khê, TP Đà Nẵng',
                scale: '3 tầng • 210 m²',
                scope: 'Thiết kế & Thi công trọn gói',
                desc: 'Công trình nhà phố 3 tầng được BN HOME triển khai từ phần móng, kết cấu khung bê tông cốt thép đến hoàn thiện mặt tiền và nội thất, tối ưu ánh sáng và thông gió tự nhiên.'
            },
            {
                id: '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR',
                title: 'Thi Công Phần Thô & Kết Cấu Nhà Phố – Hòa Xuân',
                category: 'nha-pho',
                categoryName: 'Nhà phố',
                location: 'KĐT Hòa Xuân, Cẩm Lệ, Đà Nẵng',
                scale: '3 tầng • 240 m²',
                scope: 'Thi công phần thô & nhân công hoàn thiện',
                desc: 'Quá trình thi công kết cấu thép sàn, cốp pha và bảo dưỡng bê tông chuẩn quy trình kỹ thuật, được kỹ sư BN HOME giám sát chặt chẽ từng hạng mục.'
            },
            {
                id: '1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv',
                title: 'Thi Công Hoàn Thiện Biệt Thự Sân Vườn 2 Mặt Tiền',
                category: 'biet-thu',
                categoryName: 'Biệt thự',
                location: 'Quận Ngũ Hành Sơn, TP Đà Nẵng',
                scale: '2 tầng + tum • 320 m²',
                scope: 'Thi công trọn gói chìa khóa trao tay',
                desc: 'Biệt thự phong cách hiện đại với đường nét vuông vức, khoảng xanh ban công kết hợp sân vườn thoáng mát và vật liệu hoàn thiện cao cấp bền vững.'
            },
            {
                id: '1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_',
                title: 'Thi Công Căn Hộ Dịch Vụ & Phòng Trọ Cao Cấp – Sơn Trà',
                category: 'khach-san-can-ho',
                categoryName: 'Khách sạn – Căn hộ',
                location: 'Quận Sơn Trà, TP Đà Nẵng',
                scale: '5 tầng • 480 m²',
                scope: 'Thiết kế & Thi công xây dựng',
                desc: 'Dự án căn hộ cho thuê tối ưu công năng khai thác, hệ thống điện nước và phòng cháy tiêu chuẩn, đảm bảo tiến độ nhanh để chủ đầu tư sớm vận hành.'
            },
            {
                id: '1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO',
                title: 'Thi Công Xây Dựng Nhà Phố BoB House – Hòa Khánh',
                category: 'nha-pho',
                categoryName: 'Nhà phố',
                location: 'Hòa Khánh, Liên Chiểu, Đà Nẵng',
                scale: '2 tầng • 5x20m (160 m²)',
                scope: 'Thiết kế & Thi công trọn gói',
                desc: 'Công trình thực tế bàn giao đúng tiến độ 120 ngày, tối ưu chi phí xây dựng nhưng vẫn giữ trọn thẩm mỹ hiện đại và tiện nghi sinh hoạt gia đình.'
            },
            {
                id: '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t',
                title: 'Thi Công Hoàn Thiện Khách Sạn Boutique Ven Biển',
                category: 'khach-san-can-ho',
                categoryName: 'Khách sạn – Căn hộ',
                location: 'Khu vực Mỹ Khê, Đà Nẵng',
                scale: '6 tầng • 650 m²',
                scope: 'Thi công hoàn thiện & nội thất',
                desc: 'Công trình khách sạn boutique với mặt tiền thanh lịch, sảnh lễ tân sang trọng và hệ thống phòng nghỉ đạt tiêu chuẩn thẩm mỹ cao.'
            },
            {
                id: '1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_',
                title: 'Thi Công Biệt Thự Mái Nhật Hiện Đại – Khu Nam Việt Á',
                category: 'biet-thu',
                categoryName: 'Biệt thự',
                location: 'Khu Nam Việt Á, Đà Nẵng',
                scale: '2 tầng • 300 m²',
                scope: 'Thiết kế kiến trúc & Thi công trọn gói',
                desc: 'Kiến trúc mái Nhật độ dốc cân đối, hình khối khỏe khoắn kết hợp vật liệu đá, gỗ và kính lớn tạo nên tổng thể sang trọng và gần gũi.'
            },
            {
                id: '1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT',
                title: 'Thi Công Cải Tạo & Hoàn Thiện Văn Phòng Công Ty',
                category: 'van-phong',
                categoryName: 'Văn phòng',
                location: 'Quận Hải Châu, TP Đà Nẵng',
                scale: '3 tầng • 280 m²',
                scope: 'Thi công hoàn thiện & nội thất văn phòng',
                desc: 'Không gian làm việc hiện đại, phân khu khoa học giữa phòng họp, khu điều hành và khu tiếp khách, nâng cao hình ảnh thương hiệu doanh nghiệp.'
            },
            {
                id: '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn',
                title: 'Thi Công Nhà Phố Kết Hợp Kinh Doanh – Khu Phước Lý',
                category: 'nha-pho',
                categoryName: 'Nhà phố',
                location: 'Khu Phước Lý, Cẩm Lệ, Đà Nẵng',
                scale: '3 tầng • 260 m²',
                scope: 'Thi công phần thô & hoàn thiện trọn gói',
                desc: 'Giải pháp thiết kế linh hoạt tách biệt không gian kinh doanh tầng trệt và khu sinh hoạt riêng tư các tầng trên, thi công chắc chắn, thẩm mỹ cao.'
            }
        ];

        // 3. Dữ liệu 10 Dự Án Tại Đà Nẵng (Sử dụng đủ 10 link Google Drive người dùng cung cấp)
        const danangProjects = [
            {
                id: '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT',
                title: 'Nội Thất Căn Hộ Sun Symphony 1PN+1 – Đà Nẵng',
                category: 'noi-that-dn',
                categoryName: 'Thiết kế nội thất',
                location: 'Sơn Trà, TP Đà Nẵng',
                scale: 'Căn hộ 1PN+1 • 62 m²',
                scope: 'Thiết kế & Thi công nội thất',
                desc: 'Không gian sống gam màu trung tính ấm áp, kết hợp chất liệu gỗ sáng, đá terrazzo và đường cong nội thất mềm mại giàu cảm xúc.'
            },
            {
                id: '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff',
                title: 'Nhà Phố Hiện Đại 3 Tầng – Thanh Khê Đà Nẵng',
                category: 'nha-pho-dn',
                categoryName: 'Nhà phố Đà Nẵng',
                location: 'Phường Thanh Khê, TP Đà Nẵng',
                scale: '3 tầng • 5x18m',
                scope: 'Thiết kế kiến trúc & Xây dựng trọn gói',
                desc: 'Mặt tiền thanh thoát với hệ lam che nắng và mảng xanh ban công, giúp ngôi nhà luôn mát mẻ giữa khí hậu miền Trung.'
            },
            {
                id: '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz',
                title: 'Biệt Thự Sân Vườn Khu Đô Thị Hòa Xuân',
                category: 'biet-thu-dn',
                categoryName: 'Biệt thự Đà Nẵng',
                location: 'Hòa Xuân, Cẩm Lệ, Đà Nẵng',
                scale: '2 tầng • 280 m²',
                scope: 'Thiết kế & Thi công trọn gói',
                desc: 'Biệt thự vườn sở hữu bố cục thông thoáng, liên thông phòng khách – bếp – sân vườn, tạo trải nghiệm nghỉ dưỡng ngay tại gia.'
            },
            {
                id: '1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k',
                title: 'Căn Hộ Cao Cấp View Sông Hàn – Hải Châu',
                category: 'can-ho-dn',
                categoryName: 'Căn hộ – Khách sạn',
                location: 'Quận Hải Châu, TP Đà Nẵng',
                scale: '5 tầng • 420 m²',
                scope: 'Thiết kế kiến trúc & Nội thất',
                desc: 'Mô hình căn hộ lưu trú cao cấp tối ưu tầm nhìn thoáng rộng, bố trí nội thất thông minh đáp ứng nhu cầu khách du lịch và chuyên gia.'
            },
            {
                id: '1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N',
                title: 'Biệt Thự Nghỉ Dưỡng Ngũ Hành Sơn – Đà Nẵng',
                category: 'biet-thu-dn',
                categoryName: 'Biệt thự Đà Nẵng',
                location: 'Quận Ngũ Hành Sơn, TP Đà Nẵng',
                scale: '3 tầng • 350 m²',
                scope: 'Thiết kế kiến trúc & Thi công',
                desc: 'Thiết kế tối giản sang trọng sử dụng mảng kính lớn đón gió biển, kết hợp vật liệu tự nhiên bền bỉ với môi trường ven biển.'
            },
            {
                id: '1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML',
                title: 'Nhà Phố 2 Tầng Phong Cách Tối Giản – Liên Chiểu',
                category: 'nha-pho-dn',
                categoryName: 'Nhà phố Đà Nẵng',
                location: 'Quận Liên Chiểu, TP Đà Nẵng',
                scale: '2 tầng • 175 m²',
                scope: 'Thi công trọn gói BN HOME',
                desc: 'Giải pháp nhà ở gia đình trẻ tối ưu chi phí đầu tư, đảm bảo đầy đủ 3 phòng ngủ, giếng trời đón nắng và không gian sinh hoạt chung ấm cúng.'
            },
            {
                id: '1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF',
                title: 'Thiết Kế Nội Thất Nhà Phố Wabi Sabi – Đà Nẵng',
                category: 'noi-that-dn',
                categoryName: 'Thiết kế nội thất',
                location: 'Quận Cẩm Lệ, TP Đà Nẵng',
                scale: '3 tầng • 220 m²',
                scope: 'Thiết kế & Sản xuất thi công nội thất',
                desc: 'Bảng màu trung tính dịu mắt, tập trung vào kết cấu bề mặt tự nhiên và ánh sáng gián tiếp mang lại sự thư thái sau mỗi ngày làm việc.'
            },
            {
                id: '1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A',
                title: 'Khách Sạn Boutique Biển Mỹ Khê – Sơn Trà',
                category: 'can-ho-dn',
                categoryName: 'Căn hộ – Khách sạn',
                location: 'Quận Sơn Trà, TP Đà Nẵng',
                scale: '7 tầng • 720 m²',
                scope: 'Tư vấn thiết kế & Thi công hoàn thiện',
                desc: 'Kiến trúc mặt tiền ấn tượng thu hút du khách, mặt bằng phòng nghỉ chuẩn công năng giúp nâng cao hiệu quả kinh doanh lưu trú.'
            },
            {
                id: '1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80',
                title: 'Nhà Phố Hiện Đại Khu Nam Việt Á – Đà Nẵng',
                category: 'nha-pho-dn',
                categoryName: 'Nhà phố Đà Nẵng',
                location: 'Khu Nam Việt Á, Ngũ Hành Sơn, Đà Nẵng',
                scale: '3 tầng • 245 m²',
                scope: 'Thiết kế & Thi công trọn gói',
                desc: 'Công trình nổi bật với hình khối kiến trúc hiện đại, không gian bếp ăn liên thông sân sau thoáng đãng và hệ nội thất gỗ đồng bộ.'
            },
            {
                id: '1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4',
                title: 'Không Gian Nội Thất Phòng Khách – Bếp Thanh Khê',
                category: 'noi-that-dn',
                categoryName: 'Thiết kế nội thất',
                location: 'Quận Thanh Khê, TP Đà Nẵng',
                scale: 'Nội thất trọn gói • 190 m²',
                scope: 'Thiết kế 3D & Thi công hoàn thiện',
                desc: 'Bố trí nội thất liền mạch, tối ưu hệ tủ lưu trữ âm tường giúp ngôi nhà luôn gọn gàng, sang trọng và tiện nghi cho cả gia đình.'
            }
        ];

        // 4. Dữ liệu Bài Viết Trang Chủ (Phong cách tin tức xây dựng Tín Trường Thịnh)
        const articlesData = [
            {
                imgId: '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR',
                date: 'Kiến thức thi công',
                title: 'Hướng dẫn bảo dưỡng bê tông móng đúng cách giúp nhà bền vững',
                excerpt: 'Trong xây dựng dân dụng, bê tông móng quyết định tuổi thọ toàn bộ công trình. Tìm hiểu quy trình giữ ẩm và kiểm tra cường độ chuẩn kỹ thuật.',
                content: 'Bảo dưỡng bê tông móng đúng quy trình giúp hạn chế nứt bề mặt do mất nước đột ngột và giúp bê tông đạt đúng mác thiết kế. Trong 7 ngày đầu sau khi đổ bê tông, đội ngũ kỹ sư BN HOME luôn che phủ giữ ẩm bề mặt, tưới nước đều đặn theo chu kỳ thời tiết Đà Nẵng và kiểm tra chặt chẽ trước khi tháo cốp pha triển khai bước tiếp theo.'
            },
            {
                imgId: '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT',
                date: 'Thiết kế nội thất',
                title: 'Tâm lý học không gian: Nội thất tác động đến chất lượng sống ra sao?',
                excerpt: 'Ánh sáng tự nhiên, tỷ lệ hình khối và bảng màu vật liệu ảnh hưởng trực tiếp đến cảm xúc thư thái của các thành viên trong gia đình.',
                content: 'Một không gian sống được tổ chức khoa học sẽ giảm căng thẳng và tăng sự kết nối giữa các thành viên. BN HOME ưu tiên thiết kế mở, tận dụng tối đa thông gió chéo, ánh sáng tự nhiên cùng các gam màu trung tính ấm áp để ngôi nhà không chỉ đẹp khi bàn giao mà còn dễ chịu trong suốt quá trình sử dụng lâu dài.'
            },
            {
                imgId: '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz',
                date: 'Cẩm nang xây nhà',
                title: '03 nỗi lo lớn nhất khi xây nhà trọn gói và giải pháp từ BN HOME',
                excerpt: 'Phát sinh chi phí, chậm tiến độ và thi công sai bản vẽ là 3 vấn đề phổ biến nhất. Cách lập hồ sơ dự toán minh bạch để an tâm tuyệt đối.',
                content: 'Để loại bỏ 3 nỗi lo lớn nhất của chủ đầu tư, BN HOME thực hiện chuẩn hóa ngay từ đầu: (1) Khảo sát và thiết kế hồ sơ kỹ thuật thi công chi tiết trước khi khởi công; (2) Bảng dự toán chủng loại vật tư rõ ràng từng hạng mục, cam kết không phát sinh vô lý; (3) Báo cáo tiến độ định kỳ bằng hình ảnh thực tế tại công trường để gia chủ dễ dàng theo dõi.'
            },
            {
                imgId: '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff',
                date: 'Tư vấn dự toán',
                title: 'Kinh nghiệm tính chi phí xây nhà phố tại Đà Nẵng chuẩn xác nhất',
                excerpt: 'Cách tính diện tích xây dựng theo hệ số móng, sàn, mái và lựa chọn gói vật tư phù hợp ngân sách gia đình tại khu vực Đà Nẵng.',
                content: 'Chi phí xây dựng nhà phố tại Đà Nẵng phụ thuộc vào quy mô số tầng, điều kiện địa chất nền móng, phong cách kiến trúc và cấp độ vật tư hoàn thiện. Gia chủ nên chuẩn bị hồ sơ thiết kế hoàn chỉnh để bóc tách khối lượng chính xác, từ đó chủ động kế hoạch tài chính và tránh thay đổi giữa chừng khi đang thi công.'
            }
        ];

        // 5. Render Công trình thực tế (Không nhãn dán, tên sản phẩm đầy đủ, 2 cột trên điện thoại)
        function renderConstruction(filter = 'all') {
            const container = document.getElementById('constructionGrid');
            const list = filter === 'all'
                ? constructionProjects
                : constructionProjects.filter(item => item.category === filter);

            container.innerHTML = list.map((item) => {
                const realIdx = constructionProjects.indexOf(item);
                return `
                    <article onclick="openProjectModal('construction', ${realIdx})" class="project-card cursor-pointer bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                        <div class="aspect-[4/3] w-full overflow-hidden bg-gray-100">
                            <img
                                src="${driveThumb(item.id, 'w800')}"
                                data-drive-id="${item.id}"
                                onerror="handleDriveError(this)"
                                alt="${item.title}"
                                loading="lazy"
                                class="w-full h-full object-cover"
                            >
                        </div>
                        <div class="p-3 sm:p-4 flex-1 flex flex-col justify-between">
                            <h3 class="text-[12.5px] sm:text-[14.5px] font-bold text-bn-primary leading-snug break-words">
                                ${item.title}
                            </h3>
                            <p class="text-[11.5px] sm:text-[12.5px] text-gray-500 mt-1.5 break-words">
                                ${item.location}
                            </p>
                        </div>
                    </article>
                `;
            }).join('');
        }

        function filterConstruction(cat) {
            document.querySelectorAll('#constructionTabs .cat-pill').forEach(btn => {
                btn.classList.toggle('active', btn.getAttribute('data-cat') === cat);
            });
            renderConstruction(cat);
        }

        // 6. Render Dự án Đà Nẵng (Không nhãn dán, 2 cột trên điện thoại, tên không tràn/thiếu chữ)
        function renderDaNang(filter = 'all') {
            const container = document.getElementById('danangGrid');
            const list = filter === 'all'
                ? danangProjects
                : danangProjects.filter(item => item.category === filter);

            container.innerHTML = list.map((item) => {
                const realIdx = danangProjects.indexOf(item);
                return `
                    <article onclick="openProjectModal('danang', ${realIdx})" class="project-card cursor-pointer bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                        <div class="aspect-[4/3] w-full overflow-hidden bg-gray-100">
                            <img
                                src="${driveThumb(item.id, 'w800')}"
                                data-drive-id="${item.id}"
                                onerror="handleDriveError(this)"
                                alt="${item.title}"
                                loading="lazy"
                                class="w-full h-full object-cover"
                            >
                        </div>
                        <div class="p-3 sm:p-3.5 flex-1 flex flex-col justify-between">
                            <h3 class="text-[12.5px] sm:text-[13.5px] font-bold text-bn-primary leading-snug break-words">
                                ${item.title}
                            </h3>
                            <p class="text-[11px] sm:text-[12px] text-gray-500 mt-1.5 break-words">
                                ${item.location}
                            </p>
                        </div>
                    </article>
                `;
            }).join('');
        }

        function filterDaNang(cat) {
            document.querySelectorAll('#danangTabs .cat-pill').forEach(btn => {
                btn.classList.toggle('active', btn.getAttribute('data-cat') === cat);
            });
            renderDaNang(cat);
        }

        // 7. Render Bài viết trang chủ
        function renderArticles() {
            const container = document.getElementById('articlesGrid');
            container.innerHTML = articlesData.map((art, idx) => `
                <article onclick="openArticleModal(${idx})" class="project-card cursor-pointer bg-white rounded-xl border border-gray-200 overflow-hidden flex flex-col">
                    <div class="aspect-[16/10] w-full overflow-hidden bg-gray-100">
                        <img
                            src="${driveThumb(art.imgId, 'w700')}"
                            data-drive-id="${art.imgId}"
                            onerror="handleDriveError(this)"
                            alt="${art.title}"
                            loading="lazy"
                            class="w-full h-full object-cover"
                        >
                    </div>
                    <div class="p-3 sm:p-4 flex-1 flex flex-col">
                        <p class="text-[11px] font-semibold text-bn-accent uppercase mb-1">${art.date}</p>
                        <h3 class="text-[12.5px] sm:text-[14.5px] font-bold text-bn-primary leading-snug break-words mb-2">
                            ${art.title}
                        </h3>
                        <p class="text-[11.5px] sm:text-[13px] text-gray-600 leading-relaxed flex-1 break-words">
                            ${art.excerpt}
                        </p>
                    </div>
                </article>
            `).join('');
        }

        // 8. Hệ thống Slider 2 Banner tự trượt mượt mà
        let currentSlide = 0;
        const slides = document.querySelectorAll('#heroSlider .hero-slide');
        let sliderInterval = null;

        function updateSlider() {
            slides.forEach((slide, i) => {
                slide.classList.toggle('active', i === currentSlide);
                const dot = document.getElementById(`dot-${i}`);
                if (dot) {
                    if (i === currentSlide) {
                        dot.className = 'w-7 h-2 rounded-full bg-bn-accent transition-all';
                    } else {
                        dot.className = 'w-2.5 h-2 rounded-full bg-white/55 hover:bg-white transition-all';
                    }
                }
            });
        }

        function nextSlide() {
            currentSlide = (currentSlide + 1) % slides.length;
            updateSlider();
            restartAutoSlide();
        }

        function prevSlide() {
            currentSlide = (currentSlide - 1 + slides.length) % slides.length;
            updateSlider();
            restartAutoSlide();
        }

        function goToSlide(index) {
            currentSlide = index;
            updateSlider();
            restartAutoSlide();
        }

        function restartAutoSlide() {
            if (sliderInterval) clearInterval(sliderInterval);
            sliderInterval = setInterval(() => {
                currentSlide = (currentSlide + 1) % slides.length;
                updateSlider();
            }, 5500);
        }

        // Hỗ trợ vuốt cảm ứng trên điện thoại cho 2 Banner
        let touchStartX = 0;
        const sliderEl = document.getElementById('heroSlider');
        sliderEl.addEventListener('touchstart', (e) => {
            touchStartX = e.changedTouches[0].screenX;
        }, { passive: true });
        sliderEl.addEventListener('touchend', (e) => {
            const diff = e.changedTouches[0].screenX - touchStartX;
            if (Math.abs(diff) > 45) {
                if (diff < 0) nextSlide();
                else prevSlide();
            }
        }, { passive: true });

        // 9. Modal Xem Chi Tiết Dự Án & Bài Viết
        const detailModal = document.getElementById('detailModal');

        function openProjectModal(source, idx) {
            const item = source === 'construction' ? constructionProjects[idx] : danangProjects[idx];
            if (!item) return;

            const img = document.getElementById('modalImg');
            img.setAttribute('data-drive-id', item.id);
            img.setAttribute('data-err-step', '0');
            img.onerror = function() { handleDriveError(this); };
            img.src = driveThumb(item.id, 'w1200');
            img.alt = item.title;

            document.getElementById('modalSub').textContent = item.categoryName;
            document.getElementById('modalTitle').textContent = item.title;
            document.getElementById('modalMeta').classList.remove('hidden');
            document.getElementById('modalMeta').innerHTML = `
                <div><span class="text-gray-500 block text-[11px]">Địa điểm</span><strong>${item.location}</strong></div>
                <div><span class="text-gray-500 block text-[11px]">Quy mô</span><strong>${item.scale}</strong></div>
                <div><span class="text-gray-500 block text-[11px]">Hạng mục</span><strong>${item.scope}</strong></div>
                <div><span class="text-gray-500 block text-[11px]">Đơn vị thực hiện</span><strong>BN HOME</strong></div>
            `;
            document.getElementById('modalDesc').textContent = item.desc;

            detailModal.classList.remove('hidden');
            detailModal.classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        function openArticleModal(idx) {
            const art = articlesData[idx];
            if (!art) return;

            const img = document.getElementById('modalImg');
            img.setAttribute('data-drive-id', art.imgId);
            img.setAttribute('data-err-step', '0');
            img.onerror = function() { handleDriveError(this); };
            img.src = driveThumb(art.imgId, 'w1200');
            img.alt = art.title;

            document.getElementById('modalSub').textContent = art.date;
            document.getElementById('modalTitle').textContent = art.title;
            document.getElementById('modalMeta').classList.add('hidden');
            document.getElementById('modalDesc').textContent = art.content;

            detailModal.classList.remove('hidden');
            detailModal.classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            detailModal.classList.add('hidden');
            detailModal.classList.remove('flex');
            document.body.style.overflow = '';
        }

        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                closeModal();
                closeMobileMenu();
            }
        });

        // 10. Điều khiển Menu Mobile Drawer
        const mobileDrawer = document.getElementById('mobileDrawer');
        document.getElementById('mobileMenuBtn').addEventListener('click', () => {
            mobileDrawer.classList.remove('hidden');
            document.body.style.overflow = 'hidden';
        });
        document.getElementById('closeMobileBtn').addEventListener('click', closeMobileMenu);
        document.getElementById('mobileBackdrop').addEventListener('click', closeMobileMenu);

        function closeMobileMenu() {
            mobileDrawer.classList.add('hidden');
            document.body.style.overflow = '';
        }

        // 11. Xử lý Form Yêu Cầu & Báo Giá (Hiển thị thông báo trực tiếp, không dùng alert)
        document.getElementById('quoteForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const name = document.getElementById('qName').value.trim();
            const phone = document.getElementById('qPhone').value.trim();
            const type = document.getElementById('qType').value;
            const budget = document.getElementById('qBudget').value;
            const feedback = document.getElementById('quoteFeedback');

            if (!name || !phone) {
                feedback.className = 'rounded-lg p-3.5 text-[13px] font-medium bg-red-500/20 border border-red-300/50 text-red-100';
                feedback.textContent = 'Vui lòng nhập đầy đủ Họ và tên cùng Số điện thoại để BN HOME liên hệ báo giá.';
                feedback.classList.remove('hidden');
                return;
            }

            feedback.className = 'rounded-lg p-3.5 text-[13px] font-medium bg-emerald-500/20 border border-emerald-300/50 text-emerald-100';
            feedback.textContent = `Cảm ơn ${name}! BN HOME đã tiếp nhận yêu cầu báo giá (${type} – ${budget}) cho SĐT ${phone}. Kỹ sư tư vấn sẽ liên hệ lại sớm nhất.`;
            feedback.classList.remove('hidden');
            this.reset();
        });

        // Khởi chạy dữ liệu ban đầu khi trang tải xong
        renderConstruction('all');
        renderDaNang('all');
        renderArticles();
        restartAutoSlide();
    </script>
</body>
</html>
