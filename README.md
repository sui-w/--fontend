//工具
vscode
//安装依赖
npm install
//启动程序
npm run dev


//项目结构
SentinelGuard/
├── public/                  # 静态资源 (favicon, manifest 等) （暂时还未配置相应资源）
├── src/
│   ├── assets/              # 本地静态资源 (images, svgs, global styles)
│   │   └── noise.svg        # 纹理背景
│   ├── components/          # 通用 UI 组件
│   │   └── Sidebar.tsx      # 侧边栏导航
│   ├── pages/               # 页面级组件 (路由视图)
│   │   ├── Login.tsx
│   │   ├── ThreatTracing.tsx
│   │   ├── HostMonitoring.tsx
│   │   └── ... (其他页面)
│   ├── services/            # ★ 核心对接层 (API, Chain, AI)
│   │   ├── connector.ts     # 后端/区块链/IDS 连接器
│   │   └── geminiService.ts # AI 分析服务
│   ├── types/               # TypeScript 类型定义
│   │   └── index.ts         # (原 types.ts)
│   ├── utils/               # 工具与常量
│   │   └── constants.tsx    # (原 constants.tsx) 模拟数据与常量
│   ├── App.tsx              # 路由配置
│   ├── main.tsx             # (原 index.tsx) 应用入口
│   ├── index.css            # 全局样式
│   └── vite-env.d.ts        # Vite 类型声明
├── .env                     # 环境变量 (API地址, Keys)
├── .gitignore               # Git 忽略文件
├── index.html               # 页面入口
├── package.json             # 项目依赖
├── postcss.config.js        # PostCSS 配置 (新增，用于 Tailwind)
├── tailwind.config.js       # Tailwind 配置
├── tsconfig.json            # TS 编译配置
├── tsconfig.node.json       # TS Node 配置 (新增)
└── vite.config.ts           # Vite 构建配置
