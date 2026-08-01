https://www.linkedin.com/in/shakib-mia-529b77316
realtime-chat-platform/
├── .github/
│   └── workflows/
│       ├── ci.yml
│       ├── deploy-api.yml
│       └── deploy-web.yml
│
├── apps/
│   ├── web/                              # Next.js + React + TypeScript
│   │   ├── public/
│   │   │   ├── icons/
│   │   │   └── sounds/
│   │   │       └── notification.mp3
│   │   │
│   │   ├── src/
│   │   │   ├── app/
│   │   │   │   ├── (auth)/
│   │   │   │   │   ├── login/
│   │   │   │   │   │   └── page.tsx
│   │   │   │   │   ├── register/
│   │   │   │   │   │   └── page.tsx
│   │   │   │   │   └── layout.tsx
│   │   │   │   │
│   │   │   │   ├── (chat)/
│   │   │   │   │   ├── conversations/
│   │   │   │   │   │   ├── [conversationId]/
│   │   │   │   │   │   │   ├── loading.tsx
│   │   │   │   │   │   │   └── page.tsx
│   │   │   │   │   │   └── page.tsx
│   │   │   │   │   ├── settings/
│   │   │   │   │   │   └── page.tsx
│   │   │   │   │   └── layout.tsx
│   │   │   │   │
│   │   │   │   ├── api/
│   │   │   │   │   └── health/
│   │   │   │   │       └── route.ts
│   │   │   │   ├── error.tsx
│   │   │   │   ├── global-error.tsx
│   │   │   │   ├── layout.tsx
│   │   │   │   ├── not-found.tsx
│   │   │   │   └── page.tsx
│   │   │   │
│   │   │   ├── components/
│   │   │   │   ├── chat/
│   │   │   │   │   ├── ChatHeader.tsx
│   │   │   │   │   ├── ChatWindow.tsx
│   │   │   │   │   ├── ConversationItem.tsx
│   │   │   │   │   ├── ConversationList.tsx
│   │   │   │   │   ├── MessageBubble.tsx
│   │   │   │   │   ├── MessageComposer.tsx
│   │   │   │   │   ├── MessageList.tsx
│   │   │   │   │   ├── OnlineIndicator.tsx
│   │   │   │   │   ├── ReadReceipt.tsx
│   │   │   │   │   └── TypingIndicator.tsx
│   │   │   │   ├── common/
│   │   │   │   │   ├── ErrorBoundary.tsx
│   │   │   │   │   ├── InfiniteScroll.tsx
│   │   │   │   │   └── LoadingScreen.tsx
│   │   │   │   └── ui/
│   │   │   │       ├── Avatar.tsx
│   │   │   │       ├── Button.tsx
│   │   │   │       ├── Dialog.tsx
│   │   │   │       ├── Input.tsx
│   │   │   │       └── Skeleton.tsx
│   │   │   │
│   │   │   ├── features/
│   │   │   │   ├── auth/
│   │   │   │   │   ├── auth.api.ts
│   │   │   │   │   ├── auth.schema.ts
│   │   │   │   │   ├── auth.store.ts
│   │   │   │   │   └── auth.types.ts
│   │   │   │   ├── conversations/
│   │   │   │   │   ├── conversations.api.ts
│   │   │   │   │   ├── conversations.store.ts
│   │   │   │   │   └── conversations.types.ts
│   │   │   │   ├── messages/
│   │   │   │   │   ├── messages.api.ts
│   │   │   │   │   ├── messages.store.ts
│   │   │   │   │   └── messages.types.ts
│   │   │   │   ├── presence/
│   │   │   │   │   ├── presence.store.ts
│   │   │   │   │   └── presence.types.ts
│   │   │   │   └── notifications/
│   │   │   │       └── notifications.service.ts
│   │   │   │
│   │   │   ├── hooks/
│   │   │   │   ├── useAuth.ts
│   │   │   │   ├── useDebounce.ts
│   │   │   │   ├── useInfiniteMessages.ts
│   │   │   │   ├── useOnlinePresence.ts
│   │   │   │   ├── useSocket.ts
│   │   │   │   └── useTypingIndicator.ts
│   │   │   │
│   │   │   ├── lib/
│   │   │   │   ├── api-client.ts
│   │   │   │   ├── query-client.ts
│   │   │   │   ├── socket-client.ts
│   │   │   │   ├── storage.ts
│   │   │   │   └── utils.ts
│   │   │   │
│   │   │   ├── providers/
│   │   │   │   ├── AuthProvider.tsx
│   │   │   │   ├── QueryProvider.tsx
│   │   │   │   ├── SocketProvider.tsx
│   │   │   │   └── ThemeProvider.tsx
│   │   │   │
│   │   │   ├── store/
│   │   │   │   └── index.ts
│   │   │   ├── styles/
│   │   │   │   └── globals.css
│   │   │   └── middleware.ts
│   │   │
│   │   ├── next.config.ts
│   │   ├── package.json
│   │   ├── postcss.config.js
│   │   ├── tailwind.config.ts
│   │   └── tsconfig.json
│   │
│   └── server/                           # Node.js + TypeScript
│       ├── src/
│       │   ├── config/
│       │   │   ├── database.ts
│       │   │   ├── env.ts
│       │   │   ├── logger.ts
│       │   │   └── redis.ts
│       │   │
│       │   ├── core/
│       │   │   ├── errors/
│       │   │   │   ├── AppError.ts
│       │   │   │   └── ErrorCodes.ts
│       │   │   ├── events/
│       │   │   │   └── EventBus.ts
│       │   │   ├── http/
│       │   │   │   └── ApiResponse.ts
│       │   │   └── security/
│       │   │       ├── encryption.ts
│       │   │       ├── password.ts
│       │   │       └── tokens.ts
│       │   │
│       │   ├── modules/
│       │   │   ├── auth/
│       │   │   │   ├── auth.controller.ts
│       │   │   │   ├── auth.repository.ts
│       │   │   │   ├── auth.routes.ts
│       │   │   │   ├── auth.schema.ts
│       │   │   │   └── auth.service.ts
│       │   │   ├── users/
│       │   │   │   ├── user.controller.ts
│       │   │   │   ├── user.repository.ts
│       │   │   │   ├── user.routes.ts
│       │   │   │   └── user.service.ts
│       │   │   ├── conversations/
│       │   │   │   ├── conversation.controller.ts
│       │   │   │   ├── conversation.repository.ts
│       │   │   │   ├── conversation.routes.ts
│       │   │   │   └── conversation.service.ts
│       │   │   ├── messages/
│       │   │   │   ├── message.controller.ts
│       │   │   │   ├── message.repository.ts
│       │   │   │   ├── message.routes.ts
│       │   │   │   └── message.service.ts
│       │   │   ├── attachments/
│       │   │   │   ├── attachment.controller.ts
│       │   │   │   ├── attachment.routes.ts
│       │   │   │   └── attachment.service.ts
│       │   │   └── notifications/
│       │   │       └── notification.service.ts
│       │   │
│       │   ├── realtime/
│       │   │   ├── handlers/
│       │   │   │   ├── conversation.handler.ts
│       │   │   │   ├── message.handler.ts
│       │   │   │   ├── presence.handler.ts
│       │   │   │   └── typing.handler.ts
│       │   │   ├── middleware/
│       │   │   │   ├── socket-auth.ts
│       │   │   │   └── socket-rate-limit.ts
│       │   │   ├── socket-events.ts
│       │   │   ├── socket-server.ts
│       │   │   └── socket-session.ts
│       │   │
│       │   ├── middleware/
│       │   │   ├── authenticate.ts
│       │   │   ├── error-handler.ts
│       │   │   ├── rate-limit.ts
│       │   │   ├── request-id.ts
│       │   │   └── validate.ts
│       │   │
│       │   ├── jobs/
│       │   │   ├── cleanup-presence.job.ts
│       │   │   ├── notification.job.ts
│       │   │   └── queue.ts
│       │   │
│       │   ├── app.ts
│       │   └── server.ts
│       │
│       ├── tests/
│       │   ├── integration/
│       │   │   ├── auth.test.ts
│       │   │   ├── conversations.test.ts
│       │   │   └── messages.test.ts
│       │   └── unit/
│       │       ├── message.service.test.ts
│       │       └── socket-auth.test.ts
│       │
│       ├── Dockerfile
│       ├── package.json
│       └── tsconfig.json
│
├── packages/
│   ├── database/
│   │   ├── prisma/
│   │   │   ├── migrations/
│   │   │   ├── schema.prisma
│   │   │   └── seed.ts
│   │   ├── src/
│   │   │   └── client.ts
│   │   └── package.json
│   │
│   ├── contracts/                        # Shared API/socket contracts
│   │   ├── src/
│   │   │   ├── api.ts
│   │   │   ├── auth.ts
│   │   │   ├── conversation.ts
│   │   │   ├── message.ts
│   │   │   ├── socket-events.ts
│   │   │   └── user.ts
│   │   └── package.json
│   │
│   ├── validation/
│   │   ├── src/
│   │   │   ├── auth.schema.ts
│   │   │   ├── message.schema.ts
│   │   │   └── shared.schema.ts
│   │   └── package.json
│   │
│   └── config/
│       ├── eslint/
│       ├── typescript/
│       └── package.json
│
├── infrastructure/
│   ├── docker/
│   │   └── docker-compose.yml
│   ├── kubernetes/
│   │   ├── api-deployment.yaml
│   │   ├── web-deployment.yaml
│   │   ├── redis-deployment.yaml
│   │   └── ingress.yaml
│   └── terraform/
│       ├── main.tf
│       ├── database.tf
│       └── variables.tf
│
├── scripts/
│   ├── setup.sh
│   ├── migrate.sh
│   └── seed.sh
│
├── .env.example
├── .gitignore
├── eslint.config.js
├── package.json
├── pnpm-lock.yaml
├── pnpm-workspace.yaml
├── README.md
├── tsconfig.base.json
└── turbo.json
