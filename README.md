# KTBX

## Tech Stack
### javascript
- Bun
- Svelte
- Sveltekit
- typescirpt
- tailwindcss
### rust
- tauri

## Commands
Using Svelte with SSG mode.  
### Development
- web: SSR with HR.
  ```bash
  # Run with SSR mode on HR.
  bun run dev
  ```
- web: SSG
  ```bash
  # To show SSG mode app, need to build first. build/ is generated.
  bun run build
  # Show app on build/ directory.
  bun run preview
  ```
- native
  ```bash
  # build javacript and rust both for devel
  bunx tauri dev
  ```
### Production
- build installer with bundling all.
  ```bash
  # build front(javascirpt), back(rust) and installer.
  bunx tauri build
  ```
- build front only
  ```bash
  bun run build
  ```
- build rust only
  ```bash
  # build rust code without tauri settings.
  cargo build --release
  ```
