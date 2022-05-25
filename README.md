## ESLint

코드 문법 체크

```bash
npm i eslint -D       // eslint 설치
npx eslint --init     // eslint init
npx eslint index.js   // index.js 테스트
npx eslint index.js --fix // index.js 자동 수정
```

## Prettier

An opinionated code formatter

```bash
npm i prettier -D     // prettier 설치
npx prettier index.js // index.js 테스트
npx prettier index.js --write // index.js 자동 수정
```

- .prettierrc.json 파일에 여러 설정 가능

## husky

Git hooks made easy
commit 전에 모든 파일 점검

```bash
git init
npm i husky -D
npx husky install
npx husky add .husky/pre-commit "npm test"
git add -A
git commit -m "husky test"
```

## lint-staged

Run linters on git staged files
ESLint, prettier, husky를 연결
커밋 직전에 staged된 파일을 점검
