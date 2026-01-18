---
layout: center
highlighter: shiki
css: unocss
colorSchema: dark
transition: fade-out
title: OLCT Frontend Monorepo
info: |
  ## OLCT Frontend Monorepo
  A unified approach to frontend development
lineNumbers: false
drawings:
  persist: false
mdc: true
clicks: 0
preload: false
glowSeed: 229
routerMode: hash
---

<div
  translate-x-14
  transition duration-800 ease-out
>

<h1>
  OLCT Monorepo
</h1>

Consolidating multiple repositories into one unified codebase

</div>

<div
  v-click mt-8 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 scale-95' : 'opacity-100 scale-100'"
>
  <div
    border="2 solid white/10" bg="white/5" backdrop-blur-sm
    rounded-lg px-6 py-3 flex items-center gap-3
  >
    <span text-lg>Angular 21 | pnpm Workspaces | Shared Components</span>
  </div>
</div>

---
class: py-8
glowSeed: 100
---

# Executive Summary

<span>The 30-second overview for decision makers</span>

<div mt-6 />

<div grid grid-cols-2 gap-8>

<div>
  <div flex flex-col gap-4>
    <v-clicks>
      <div
        border="2 solid red-800" bg="red-800/20"
        rounded-lg px-5 py-4
      >
        <div flex items-center gap-3 mb-2>
          <div i-carbon:warning-alt text-red-400 text-2xl />
          <span font-bold text-lg>Current State</span>
        </div>
        <div text-sm opacity-80>5 separate frontend repos with duplicated code, inconsistent versions, and siloed maintenance</div>
      </div>
      <div
        border="2 solid green-800" bg="green-800/20"
        rounded-lg px-5 py-4
      >
        <div flex items-center gap-3 mb-2>
          <div i-carbon:checkmark-filled text-green-400 text-2xl />
          <span font-bold text-lg>Proposed Solution</span>
        </div>
        <div text-sm opacity-80>Single monorepo with shared packages, unified tooling, and centralized dependency management</div>
      </div>
      <div
        border="2 solid blue-800" bg="blue-800/20"
        rounded-lg px-5 py-4
      >
        <div flex items-center gap-3 mb-2>
          <div i-carbon:chart-line text-blue-400 text-2xl />
          <span font-bold text-lg>Expected Outcome</span>
        </div>
        <div text-sm opacity-80>Faster delivery, reduced maintenance burden, consistent user experience across all apps</div>
      </div>
    </v-clicks>
  </div>
</div>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
>
  <div bg="white/10" px-4 py-3 flex items-center>
    <div i-carbon:analytics text-cyan-300 text-xl mr-2 />
    <span font-semibold>Key Metrics</span>
  </div>
  <div px-5 py-4 flex flex-col gap-4>
    <div flex items-center justify-between>
      <span>Repositories</span>
      <div flex items-center gap-2>
        <span text-red-400 line-through>5 separate</span>
        <div i-carbon:arrow-right text-sm />
        <span text-green-400 font-bold>1 unified</span>
      </div>
    </div>
    <div flex items-center justify-between>
      <span>Version consistency</span>
      <div flex items-center gap-2>
        <span text-red-400 line-through>Manual</span>
        <div i-carbon:arrow-right text-sm />
        <span text-green-400 font-bold>Automatic</span>
      </div>
    </div>
    <div flex items-center justify-between>
      <span>Code sharing</span>
      <div flex items-center gap-2>
        <span text-red-400 line-through>Copy-paste</span>
        <div i-carbon:arrow-right text-sm />
        <span text-green-400 font-bold>Shared libs</span>
      </div>
    </div>
    <div flex items-center justify-between>
      <span>New app setup</span>
      <div flex items-center gap-2>
        <span text-red-400 line-through>Hours</span>
        <div i-carbon:arrow-right text-sm />
        <span text-green-400 font-bold>Seconds</span>
      </div>
    </div>
    <div flex items-center justify-between>
      <span>Disk usage</span>
      <div flex items-center gap-2>
        <span text-red-400 line-through>~6GB</span>
        <div i-carbon:arrow-right text-sm />
        <span text-green-400 font-bold>~400MB</span>
      </div>
    </div>
  </div>
</div>

</div>

---
class: py-8
glowSeed: 88
---

# Why Change Now?

<span>The strategic imperative for consolidation</span>

<div mt-6 grid grid-cols-3 gap-6>

<v-clicks>

<div
  border="2 solid amber-800" bg="amber-800/20"
  rounded-lg p-5 flex flex-col
>
  <div i-carbon:growth text-amber-400 text-4xl mb-4 />
  <div font-bold text-lg mb-2>Scaling Challenges</div>
  <div text-sm opacity-70>As we add more applications, the multi-repo overhead grows exponentially. Each new app multiplies maintenance burden.</div>
</div>

<div
  border="2 solid red-800" bg="red-800/20"
  rounded-lg p-5 flex flex-col
>
  <div i-carbon:security text-red-400 text-4xl mb-4 />
  <div font-bold text-lg mb-2>Security & Compliance</div>
  <div text-sm opacity-70>Vulnerability patches must be applied to 5+ repos separately. Delayed updates = increased exposure window.</div>
</div>

<div
  border="2 solid blue-800" bg="blue-800/20"
  rounded-lg p-5 flex flex-col
>
  <div i-carbon:user-multiple text-blue-400 text-4xl mb-4 />
  <div font-bold text-lg mb-2>Team Productivity</div>
  <div text-sm opacity-70>Developers context-switch between repos with different configs. Onboarding requires learning 5 different setups.</div>
</div>

</v-clicks>

</div>

<div
  v-click mt-6
  border="2 solid purple-800" bg="purple-800/20"
  rounded-lg px-6 py-4 flex items-center gap-4
>
  <div i-carbon:idea text-yellow-300 text-3xl />
  <div>
    <div font-bold text-lg>Industry Trend</div>
    <div text-sm opacity-80>Google, Meta, Microsoft, and Uber all use monorepos at scale. This approach is proven for organizations managing multiple related applications.</div>
  </div>
</div>

---
class: py-10
glowSeed: 100
---

# The Current State

<span>Before: 5 Separate Repositories</span>

<div mt-6 />

<div grid grid-cols-2 gap-8>

<div>
  <div flex flex-col gap-3>
    <v-clicks>
      <div flex items-center gap-3 bg="red-800/80" border="2 solid red-800/50" rounded-lg px-4 py-3>
        <div i-carbon:copy text-red-300 text-xl />
        <div>
          <div font-semibold>Duplicated dependencies</div>
          <div text-sm opacity-70>Same packages installed 5 times</div>
        </div>
      </div>
      <div flex items-center gap-3 bg="red-800/60" border="2 solid red-800/50" rounded-lg px-4 py-3>
        <div i-carbon:warning-alt text-red-300 text-xl />
        <div>
          <div font-semibold>Version drift</div>
          <div text-sm opacity-70>Different Angular versions in each repo</div>
        </div>
      </div>
      <div flex items-center gap-3 bg="red-800/40" border="2 solid red-800/50" rounded-lg px-4 py-3>
        <div i-carbon:code text-red-300 text-xl />
        <div>
          <div font-semibold>Copy-paste code</div>
          <div text-sm opacity-70>No proper sharing mechanism</div>
        </div>
      </div>
      <div flex items-center gap-3 bg="red-800/20" border="2 solid red-800/50" rounded-lg px-4 py-3>
        <div i-carbon:settings-check text-red-300 text-xl />
        <div>
          <div font-semibold>Inconsistent tooling</div>
          <div text-sm opacity-70>Different configs everywhere</div>
        </div>
      </div>
    </v-clicks>
  </div>
</div>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
>
  <div bg="white/10" px-4 py-2 flex items-center>
    <div i-carbon:folder text-amber-300 text-xl mr-2 />
    <span font-semibold>Repository Structure</span>
  </div>
  <div px-4 py-3 font-mono text-sm>
    <div text-red-300>repo-app-a/</div>
    <div text-xs pl-4 opacity-70>├── package.json  # Angular 17.0.0</div>
    <div text-xs pl-4 opacity-70>└── shared/       # Copy-pasted utils</div>
    <div mt-2 text-red-300>repo-app-b/</div>
    <div text-xs pl-4 opacity-70>├── package.json  # Angular 17.2.0</div>
    <div text-xs pl-4 opacity-70>└── shared/       # Different version!</div>
    <div mt-2 text-red-300>repo-app-c/</div>
    <div text-xs pl-4 opacity-70>├── package.json  # Angular 16.x (!!) </div>
    <div mt-2 text-red-300>repo-app-d/</div>
    <div text-xs pl-4 opacity-70>└── package.json  # Angular 17.1.0</div>
    <div mt-2 text-red-300>repo-app-e/</div>
    <div text-xs pl-4 opacity-70>└── package.json  # Angular 15.3.1</div>
  </div>
</div>

</div>

---
class: py-10
glowSeed: 185
---

# The Real Problem: Dependency Chaos

<span>When every repository becomes an island</span>

<div mt-6 />

<div flex items-center justify-center gap-8>
  <div
    v-click="1"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid red-800" bg="red-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:warning-alt text-red-300 text-2xl mr-2 />
        <span font-bold text-xl>Multi-Repo with npm</span>
      </div>
      <div grid grid-cols-2 gap-4>
        <!-- Repo 1 -->
        <div bg="red-900/30" rounded-lg p-3>
          <div flex items-center gap-2 mb-2>
            <div i-carbon:folder text-amber-300 />
            <span font-semibold>ctv-app</span>
          </div>
          <div text-sm space-y-1>
            <div flex items-center gap-1>
              <div i-carbon:cube text-xs />
              <span text-xs>Angular 17.0.0</span>
            </div>
            <div flex items-center gap-1>
              <div i-carbon:package text-xs />
              <span text-xs>node_modules: 1.2GB</span>
            </div>
            <div text-xs text-red-300 mt-2>package-lock.json #1</div>
          </div>
        </div>
        <!-- Repo 2 -->
        <div bg="red-900/30" rounded-lg p-3>
          <div flex items-center gap-2 mb-2>
            <div i-carbon:folder text-blue-300 />
            <span font-semibold>sov-app</span>
          </div>
          <div text-sm space-y-1>
            <div flex items-center gap-1>
              <div i-carbon:cube text-xs />
              <span text-xs>Angular 17.2.0</span>
            </div>
            <div flex items-center gap-1>
              <div i-carbon:package text-xs />
              <span text-xs>node_modules: 1.2GB</span>
            </div>
            <div text-xs text-red-300 mt-2>package-lock.json #2</div>
          </div>
        </div>
      </div>
      <div mt-3 text-center>
        <span text-xl text-red-400 font-bold>Same deps, different versions</span>
        <div text-sm text-red-300>Installed separately, maintained separately!</div>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    flex items-center
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0' : 'opacity-100'"
  >
    <div i-carbon:arrow-right text-4xl text-green-400 animate-pulse />
  </div>

  <div
    v-click="3"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid green-800" bg="green-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:share-knowledge text-green-300 text-2xl mr-2 />
        <span font-bold text-xl>Monorepo + pnpm Catalogs</span>
      </div>
      <div bg="green-900/30" rounded-lg p-3 mb-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:catalog text-green-300 />
          <span font-semibold>pnpm-workspace.yaml</span>
        </div>
        <div text-sm space-y-1>
          <div flex items-center gap-1>
            <div i-carbon:cube text-xs />
            <span text-xs>Angular: ^21.1.0 (catalog)</span>
          </div>
          <div flex items-center gap-1>
            <div i-carbon:package text-xs />
            <span text-xs>Shared store: ~400MB</span>
          </div>
          <div text-xs text-green-300 mt-2>Single pnpm-lock.yaml</div>
        </div>
      </div>
      <div grid grid-cols-2 gap-2>
        <div flex items-center gap-1 text-sm>
          <div i-carbon:link text-green-400 />
          <span>ctv → uses catalog</span>
        </div>
        <div flex items-center gap-1 text-sm>
          <div i-carbon:link text-green-400 />
          <span>sov → uses catalog</span>
        </div>
      </div>
    </div>
  </div>
</div>

<div
  v-click="3"
  mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0' : 'opacity-100'"
>
  <div bg="blue-900/30" border="2 solid blue-800" rounded-lg px-5 py-3>
    <div flex items-center gap-3>
      <div i-carbon:analytics text-blue-300 text-2xl />
      <div>
        <div text-lg font-bold>The Difference</div>
        <div text-sm>5 repos × 1.2GB each = <span text-red-400 line-through>6GB + version chaos</span> → <span text-green-400>~400MB + perfect sync</span></div>
      </div>
    </div>
  </div>
</div>

---
class: py-8
glowSeed: 120
---

# The Cost of Inaction

<span>What happens if we continue on the current path</span>

<div mt-6 grid grid-cols-2 gap-8>

<div flex flex-col gap-4>
  <v-clicks>
    <div
      border="2 solid red-800" bg="red-800/20"
      rounded-lg px-5 py-4 flex items-start gap-4
    >
      <div i-carbon:time text-red-400 text-3xl mt-1 />
      <div>
        <div font-bold text-lg>Compounding Tech Debt</div>
        <div text-sm opacity-70 mt-1>Every feature added to one app that should be shared gets copy-pasted. Divergence increases over time.</div>
      </div>
    </div>
    <div
      border="2 solid orange-800" bg="orange-800/20"
      rounded-lg px-5 py-4 flex items-start gap-4
    >
      <div i-carbon:currency-dollar text-orange-400 text-3xl mt-1 />
      <div>
        <div font-bold text-lg>Multiplied Maintenance</div>
        <div text-sm opacity-70 mt-1>Bug fixes and updates must be applied 5 times. Developer time spent on repetitive work instead of innovation.</div>
      </div>
    </div>
    <div
      border="2 solid yellow-800" bg="yellow-800/20"
      rounded-lg px-5 py-4 flex items-start gap-4
    >
      <div i-carbon:user-activity text-yellow-400 text-3xl mt-1 />
      <div>
        <div font-bold text-lg>Inconsistent UX</div>
        <div text-sm opacity-70 mt-1>Users notice when apps behave differently, and require much more context switching</div>
      </div>
    </div>
  </v-clicks>
</div>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
>
  <div bg="red-900/40" px-4 py-3 flex items-center>
    <div i-carbon:warning-alt text-red-300 text-xl mr-2 />
    <span font-semibold>Risk Scenario</span>
  </div>
  <div px-5 py-4>
    <div text-sm opacity-80 mb-4>
      A critical security vulnerability is discovered in Angular...
    </div>
    <div flex flex-col gap-3>
      <div bg="red-900/30" rounded-lg p-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:close-filled text-red-400 />
          <span font-semibold>Multi-Repo Response</span>
        </div>
        <div text-xs opacity-70>
          • Open 5 PRs in 5 repos<br/>
          • Coordinate 5 different CI pipelines<br/>
          • Test each app separately<br/>
          • Deploy 5 times<br/>
          • Hope nothing was missed
        </div>
      </div>
      <div bg="green-900/30" rounded-lg p-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:checkmark-filled text-green-400 />
          <span font-semibold>Monorepo Response</span>
        </div>
        <div text-xs opacity-70>
          • Update catalog: 1 line change<br/>
          • Run `pnpm install`<br/>
          • All apps updated atomically<br/>
          • Single PR, single review
        </div>
      </div>
    </div>
  </div>
</div>

</div>

---
layout: center
class: text-center
glowSeed: 205
---

# The Solution

<div
  v-click flex flex-col items-center transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'translate-y-10 opacity-0' : 'translate-y-0 opacity-100'"
>
  <div text-8xl font-bold bg-gradient-to-r from-blue-400 to-green-400 bg-clip-text text-transparent>
    Monorepo
  </div>

  <div mt-8 text-xl opacity-80>
    One repository. Unified tooling. Shared code.
  </div>

  <div mt-8 flex gap-6>
    <div
      v-after
      border="2 solid blue-800" bg="blue-800/20"
      rounded-lg px-4 py-3 flex items-center gap-2
      transition duration-500 ease-in-out
      :class="$clicks < 1 ? 'scale-90 opacity-0' : 'scale-100 opacity-100'"
    >
      <div i-carbon:folder-shared text-blue-300 text-xl />
      <span>Single Source of Truth</span>
    </div>
    <div
      v-after
      border="2 solid green-800" bg="green-800/20"
      rounded-lg px-4 py-3 flex items-center gap-2
      transition duration-500 ease-in-out
      :class="$clicks < 1 ? 'scale-90 opacity-0' : 'scale-100 opacity-100'"
    >
      <div i-carbon:checkmark-outline text-green-300 text-xl />
      <span>Consistent Versions</span>
    </div>
    <div
      v-after
      border="2 solid purple-800" bg="purple-800/20"
      rounded-lg px-4 py-3 flex items-center gap-2
      transition duration-500 ease-in-out
      :class="$clicks < 1 ? 'scale-90 opacity-0' : 'scale-100 opacity-100'"
    >
      <div i-carbon:share text-purple-300 text-xl />
      <span>Shared Components</span>
    </div>
  </div>
</div>

---
class: py-8
glowSeed: 338
---

# Business Value

<span>Benefits for stakeholders and delivery teams</span>

<div mt-4 grid grid-cols-2 gap-8>

<div>
  <div flex items-center gap-2 mb-4>
    <div i-carbon:enterprise text-green-300 text-2xl />
    <span text-xl font-bold>For Business Owners</span>
  </div>

  <div flex flex-col gap-3>
    <v-clicks>
      <div
        border="2 solid green-800" bg="green-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:user-multiple text-green-400 />
          <span font-bold>Consistent User Experience</span>
        </div>
        <div text-sm opacity-70 mt-1>All applications look and behave the same way</div>
      </div>
      <div
        border="2 solid blue-800" bg="blue-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:flash text-blue-400 />
          <span font-bold>Faster Time to Market</span>
        </div>
        <div text-sm opacity-70 mt-1>Reusable components accelerate feature delivery</div>
      </div>
      <div
        border="2 solid purple-800" bg="purple-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:security text-purple-400 />
          <span font-bold>Reduced Security Risk</span>
        </div>
        <div text-sm opacity-70 mt-1>Centralized vulnerability management across all apps</div>
      </div>
      <div
        border="2 solid orange-800" bg="orange-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:currency-dollar text-orange-400 />
          <span font-bold>Lower Total Cost of Ownership</span>
        </div>
        <div text-sm opacity-70 mt-1>One codebase to maintain instead of five</div>
      </div>
    </v-clicks>
  </div>
</div>

<div>
  <div flex items-center gap-2 mb-4>
    <div i-carbon:group text-cyan-300 text-2xl />
    <span text-xl font-bold>For Teams</span>
  </div>

  <div flex flex-col gap-3>
    <v-clicks>
      <div
        border="2 solid cyan-800" bg="cyan-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:diagram text-cyan-400 />
          <span font-bold>Architectural Consistency</span>
        </div>
        <div text-sm opacity-70 mt-1>Enforce patterns and standards across all applications</div>
      </div>
      <div
        border="2 solid pink-800" bg="pink-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:version text-pink-400 />
          <span font-bold>Simplified Governance</span>
        </div>
        <div text-sm opacity-70 mt-1>Single place to manage dependencies and versions</div>
      </div>
      <div
        border="2 solid yellow-800" bg="yellow-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:network-3 text-yellow-400 />
          <span font-bold>Cross-Cutting Changes</span>
        </div>
        <div text-sm opacity-70 mt-1>Update shared code once, all apps benefit immediately</div>
      </div>
      <div
        border="2 solid teal-800" bg="teal-800/20"
        rounded-lg px-4 py-3
        transition duration-500 ease-in-out
      >
        <div flex items-center gap-2>
          <div i-carbon:code text-teal-400 />
          <span font-bold>Code Discoverability</span>
        </div>
        <div text-sm opacity-70 mt-1>All code in one place makes audits and reviews easier</div>
      </div>
    </v-clicks>
  </div>
</div>

</div>

---
class: py-10
glowSeed: 175
---

# Monorepo Structure

<span>A well-organized codebase for all applications</span>

<div mt-6 grid grid-cols-2 gap-8>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
>
  <div bg="white/10" px-4 py-2 flex items-center>
    <div i-carbon:tree-view text-green-300 text-xl mr-2 />
    <span font-semibold>Directory Layout</span>
  </div>
  <div px-4 py-3 font-mono text-sm>
    <div mb-4 text-green-300>olct-frontend/</div>
    <div pl-4>├── <span text-blue-300>apps/</span>                # All applications</div>
    <div pl-8 opacity-70>├── ctv/</div>
    <div pl-8 opacity-70>├── sov/</div>
    <div pl-8 opacity-70>├── heli/</div>
    <div pl-8 opacity-70>├── fuel/</div>
    <div mb-4 pl-8 opacity-70>└── odex/</div>
    <div pl-4>├── <span text-purple-300>packages/</span>           # Shared libraries</div>
    <div pl-8 opacity-70>├── core/           # Utilities & services</div>
    <div pl-8 opacity-70>└── ui/             # UI components</div>
    <div mt-4 pl-4>├── <span text-amber-300>pnpm-workspace.yaml</span></div>
    <div pl-4>└── <span text-amber-300>package.json</span></div>
  </div>
</div>

<div flex flex-col gap-4>
  <v-clicks>
    <div
      border="2 solid blue-800" bg="blue-800/20"
      rounded-lg overflow-hidden
      transition duration-500 ease-in-out
    >
      <div bg="blue-800/40" px-4 py-2 flex items-center>
        <div i-carbon:application text-blue-300 text-xl mr-2 />
        <span font-bold>Apps</span>
      </div>
      <div px-4 py-3>
        <div text-sm opacity-80>Production applications live here</div>
        <div flex gap-2 mt-2>
          <div bg="blue-900/50" rounded px-2 py-1 text-xs>CTV</div>
          <div bg="blue-900/50" rounded px-2 py-1 text-xs>SOV</div>
          <div bg="blue-900/50" rounded px-2 py-1 text-xs>Heli</div>
          <div bg="blue-900/50" rounded px-2 py-1 text-xs>Fuel</div>
          <div bg="blue-900/50" rounded px-2 py-1 text-xs>ODEX</div>
        </div>
      </div>
    </div>
    <div
      border="2 solid purple-800" bg="purple-800/20"
      rounded-lg overflow-hidden
      transition duration-500 ease-in-out
    >
      <div bg="purple-800/40" px-4 py-2 flex items-center>
        <div i-carbon:package text-purple-300 text-xl mr-2 />
        <span font-bold>Packages</span>
      </div>
      <div px-4 py-3>
        <div text-sm opacity-80>Shared code used by all apps</div>
        <div flex gap-2 mt-2>
          <div bg="purple-900/50" rounded px-2 py-1 text-xs>@olct/core</div>
          <div bg="purple-900/50" rounded px-2 py-1 text-xs>@olct/ui</div>
        </div>
      </div>
    </div>
    <div
      border="2 solid amber-800" bg="amber-800/20"
      rounded-lg overflow-hidden
      transition duration-500 ease-in-out
    >
      <div bg="amber-800/40" px-4 py-2 flex items-center>
        <div i-carbon:settings text-amber-300 text-xl mr-2 />
        <span font-bold>Central Config</span>
      </div>
      <div px-4 py-3>
        <div text-sm opacity-80>One place for all dependency versions</div>
      </div>
    </div>
  </v-clicks>
</div>

</div>

---
class: py-10
glowSeed: 123
---

# How It Works: pnpm Catalogs

<span>All dependency versions defined in one place</span>

<div mt-6 flex gap-8>

<div
  v-click w="1/2"
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
>
<div border="2 solid white/10" bg="white/5" backdrop-blur-sm rounded-lg overflow-hidden>
<div bg="white/10" px-4 py-2 flex items-center>
<div i-carbon:document-tasks text-cyan-300 text-xl mr-2 />
<span font-semibold>pnpm-workspace.yaml</span>
</div>
<div px-1 py-1>

```yaml
catalog:
  # Angular - all apps use the same version
  '@angular/aria': ^21.1.0
  '@angular/cdk': ^21.1.0
  '@angular/core': ^21.1.0

  # Styling
  'tailwindcss': ^4.1.18

  # Testing
  '@playwright/test': ^1.57.0
  'vitest': ^4.0.17
```

</div>
</div>
</div>

<div w="1/2" flex flex-col gap-4>
<v-clicks>

<div border="2 solid green-800" bg="green-800/20" rounded-lg px-4 py-4 flex items-start gap-4 transition duration-500 ease-in-out>
<div bg="green-700" rounded-full w-10 h-10 min-w-10 flex items-center justify-center text-xl font-bold>1</div>
<div>
<div font-bold>Change version once</div>
<div text-sm opacity-80>Edit a single line in the catalog</div>
</div>
</div>

<div border="2 solid blue-800" bg="blue-800/20" rounded-lg px-4 py-4 flex items-start gap-4 transition duration-500 ease-in-out>
<div bg="blue-700" rounded-full w-10 h-10 min-w-10 flex items-center justify-center text-xl font-bold>2</div>
<div>
<div font-bold>Run one command</div>
<div text-sm font-mono bg="black/30" rounded px-2 py-1 mt-1>pnpm install</div>
</div>
</div>

<div border="2 solid purple-800" bg="purple-800/20" rounded-lg px-4 py-4 flex items-start gap-4 transition duration-500 ease-in-out>
<div bg="purple-700" rounded-full w-10 h-10 min-w-10 flex items-center justify-center text-xl font-bold>3</div>
<div>
<div font-bold>All apps updated</div>
<div text-sm opacity-80>Consistent versions everywhere</div>
</div>
</div>

</v-clicks>
</div>

</div>

---
class: py-10
glowSeed: 180
---

# How It Works: Shared Packages

<span>Build once, use everywhere</span>

<div mt-6 grid grid-cols-2 gap-8>

<div
  v-click border="2 solid blue-800" bg="blue-800/20" rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
>
<div bg="blue-800/40" px-4 py-3 flex items-center>
<div i-carbon:code text-blue-300 text-xl mr-2 />
<span font-bold>@olct/core</span>
</div>
<div px-4 py-4>
<div text-sm opacity-80 mb-4>Shared utilities and services</div>
<div flex flex-col gap-3>
<div flex items-center gap-3 bg="blue-900/30" rounded-lg px-3 py-2>
<div i-carbon:function text-blue-300 text-lg />
<span text-sm>Helper functions</span>
</div>
<div flex items-center gap-3 bg="blue-900/30" rounded-lg px-3 py-2>
<div i-carbon:data-class text-green-300 text-lg />
<span text-sm>Type definitions</span>
</div>
<div flex items-center gap-3 bg="blue-900/30" rounded-lg px-3 py-2>
<div i-carbon:api text-purple-300 text-lg />
<span text-sm>API services</span>
</div>
</div>
</div>
</div>

<div
  v-click border="2 solid orange-800" bg="orange-800/20" rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 2 ? 'opacity-0 translate-x-10' : 'opacity-100 translate-x-0'"
>
<div bg="orange-800/40" px-4 py-3 flex items-center>
<div i-carbon:touch-1 text-orange-300 text-xl mr-2 />
<span font-bold>@olct/ui</span>
</div>
<div px-4 py-4>
<div text-sm opacity-80 mb-4>Reusable UI components</div>
<div flex flex-col gap-3>
<div flex items-center gap-3 bg="orange-900/30" rounded-lg px-3 py-2>
<div i-carbon:checkbox-checked text-orange-300 text-lg />
<span text-sm>Buttons, inputs, forms</span>
</div>
<div flex items-center gap-3 bg="orange-900/30" rounded-lg px-3 py-2>
<div i-carbon:table text-cyan-300 text-lg />
<span text-sm>Tables, cards, layouts</span>
</div>
<div flex items-center gap-3 bg="orange-900/30" rounded-lg px-3 py-2>
<div i-carbon:color-palette text-pink-300 text-lg />
<span text-sm>Consistent styling</span>
</div>
</div>
</div>
</div>

</div>

<div
  v-click mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
>
<div border="2 solid green-800" bg="green-800/20" rounded-lg px-6 py-4 flex items-center gap-3>
<div i-carbon:flash text-yellow-300 text-2xl />
<span text-lg>Fix a bug in <span font-mono bg="black/30" px-2 py-1 rounded>@olct/ui</span> and all 5 apps get the fix instantly</span>
</div>
</div>

---
class: py-10
glowSeed: 150
---

# Before vs After

<span>The transformation in action</span>

<div mt-6 grid grid-cols-2 gap-6>

<div
  v-click border="2 solid red-800" bg="red-800/20" rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
>
<div bg="red-800/40" px-4 py-2 flex items-center>
<div i-carbon:close-filled text-red-300 text-xl mr-2 />
<span font-bold>Before: Separate Repos</span>
</div>
<div px-4 py-4>
<div bg="black/30" rounded-lg p-3 font-mono text-sm>
<div opacity-70># Updating Angular across 5 repos</div>
<div text-xs>cd repo-app-a && npm install @angular/core@21</div>
<div text-xs>cd repo-app-b && npm install @angular/core@21</div>
<div text-xs>cd repo-app-c && npm install @angular/core@21</div>
<div text-xs>cd repo-app-d && npm install @angular/core@21</div>
<div text-xs>cd repo-app-e && npm install @angular/core@21</div>
<div mt-2 opacity-70># 5 different lock files</div>
<div opacity-70># 5 different CI pipelines</div>
<div opacity-70># Hope nothing breaks!</div>
</div>
<div mt-4 bg="red-900/30" rounded-lg p-3 flex items-center gap-2>
<div i-carbon:warning-alt text-red-400 />
<span text-sm>Requires coordination across teams and repos</span>
</div>
</div>
</div>

<div
  v-click border="2 solid green-800" bg="green-800/20" rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 2 ? 'opacity-0 translate-x-10' : 'opacity-100 translate-x-0'"
>
<div bg="green-800/40" px-4 py-2 flex items-center>
<div i-carbon:checkmark-filled text-green-300 text-xl mr-2 />
<span font-bold>After: Monorepo</span>
</div>
<div px-4 py-4>
<div bg="black/30" rounded-lg p-3 font-mono text-sm>
<div opacity-70># Edit pnpm-workspace.yaml</div>
<div text-green-300>catalog:</div>
<div pl-4 text-green-300>  '@angular/core': ^21.1.0</div>
<div mt-3 opacity-70># Run one command</div>
<div text-cyan-300>pnpm install</div>
<div mt-4 opacity-70># Done!</div>
</div>
<div mt-9 bg="green-900/30" rounded-lg p-3 flex items-center gap-2>
<div i-carbon:checkmark-outline text-green-400 />
<span text-sm>One change. One command. All apps updated.</span>
</div>
</div>
</div>

</div>

---
class: py-10
glowSeed: 250
---

# Technology Stack

<span>Modern tools for modern development</span>

<div mt-8 grid grid-cols-2 gap-8>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 1 ? 'opacity-0 translate-x--10' : 'opacity-100 translate-x-0'"
>
  <div bg="white/10" px-4 py-2 flex items-center>
    <div i-carbon:application-web text-blue-300 text-xl mr-2 />
    <span font-semibold>Core Stack</span>
  </div>
  <div px-4 py-4 flex flex-col gap-3>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:angular-icon text-xl />
        <span>Framework</span>
      </div>
      <span font-mono text-blue-300>Angular 21</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:typescript-icon text-xl />
        <span>Language</span>
      </div>
      <span font-mono text-blue-300>TypeScript 5.9</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:pnpm text-xl />
        <span>Package Manager</span>
      </div>
      <span font-mono text-orange-300>pnpm 10</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:tailwindcss-icon text-xl />
        <span>Styling</span>
      </div>
      <span font-mono text-cyan-300>TailwindCSS 4</span>
    </div>
  </div>
</div>

<div
  v-click
  border="2 solid white/10" bg="white/5" backdrop-blur-sm
  rounded-lg overflow-hidden
  transition duration-500 ease-in-out
  :class="$clicks < 2 ? 'opacity-0 translate-x-10' : 'opacity-100 translate-x-0'"
>
  <div bg="white/10" px-4 py-2 flex items-center>
    <div i-carbon:tools text-green-300 text-xl mr-2 />
    <span font-semibold>Developer Tools</span>
  </div>
  <div px-4 py-4 flex flex-col gap-3>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:vitest text-xl />
        <span>Testing</span>
      </div>
      <span font-mono text-green-300>Vitest + Playwright</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-logos:eslint text-xl />
        <span>Code Quality</span>
      </div>
      <span font-mono text-purple-300>ESLint + Prettier</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-carbon:build text-xl text-amber-400 />
        <span>Build</span>
      </div>
      <span font-mono text-amber-300>ng-packagr</span>
    </div>
    <div flex items-center justify-between bg="white/5" rounded-lg px-3 py-2>
      <div flex items-center gap-2>
        <div i-carbon:version text-xl text-pink-400 />
        <span>Version Control</span>
      </div>
      <span font-mono text-pink-300>Changesets</span>
    </div>
  </div>
</div>

</div>

<div
  v-click mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
>
  <div
    border="2 solid blue-800" bg="blue-800/20"
    rounded-lg px-6 py-3 flex items-center gap-3
  >
    <div i-carbon:idea text-yellow-300 text-xl />
    <span>All using the latest stable versions, managed centrally through pnpm catalogs</span>
  </div>
</div>

---
class: py-10
clicks: 3
glow: bottom
glowSeed: 290
---

# New App Setup: From Hours to Seconds

<span>Pre-configured scaffolding for rapid development</span>

<div mt-6 />

<div flex>
  <div
    v-click="1"
    w="1/2" pr-4
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div
      border="2 solid indigo-800" bg="indigo-800/20"
      rounded-lg overflow-hidden relative h-70
    >
      <div bg="indigo-800/40" px-4 py-2 flex items-center>
        <div i-carbon:application text-blue-300 text-xl mr-2 />
        <span font-bold>Monorepo App Scaffolding</span>
      </div>
      <div
        absolute left-0 right-0 top-12 bottom-0
        class="bg-[url('/bg-grid.svg')] bg-center"
      >
        <div
          v-for="(item, idx) in [
            { x: 20, y: 20, r: 45, color: 'rgba(59, 130, 246, 0.5)', label: '@olct/core' },
            { x: 130, y: 45, r: 40, color: 'rgba(59, 130, 246, 0.5)', label: '@olct/ui' },
            { x: 70, y: 110, r: 35, color: 'rgba(147, 51, 234, 0.5)', label: 'ESLint' },
            { x: 210, y: 15, r: 38, color: 'rgba(147, 51, 234, 0.5)', label: 'Prettier' },
            { x: 290, y: 40, r: 42, color: 'rgba(144, 57, 94, 0.5)', label: 'Vitest' },
            { x: 150, y: 130, r: 35, color: 'rgba(34, 197, 94, 0.5)', label: 'Tailwind' }
          ]"
          :key="idx"
          absolute
          class="rounded-full flex items-center justify-center"
          :style="{
            left: `${item.x}px`,
            top: `${item.y}px`,
            width: `${item.r*2}px`,
            height: `${item.r*2}px`,
            backgroundColor: item.color,
            border: '2px solid rgba(59, 130, 246, 0.8)',
            transitionDelay: `${300 + idx * 200}ms`,
            transitionProperty: 'all',
            transitionDuration: '800ms'
          }"
        >
          <span font-bold text-xs text-center>{{item.label}}</span>
        </div>
        <div absolute right-4 bottom-4 flex flex-col gap-3>
          <div flex items-center gap-2 bg="blue-900/60" px-3 py-1.5 rounded-lg text-sm>
            <div i-carbon:checkmark-outline text-green-400 />
            <span>Pre-configured</span>
          </div>
          <div flex items-center gap-2 bg="blue-900/60" px-3 py-1.5 rounded-lg text-sm>
            <div i-carbon:checkmark-outline text-green-400 />
            <span>Shared packages</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    w="1/2" pl-4
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div
      border="2 solid blue-800" bg="blue-800/20"
      rounded-lg overflow-hidden relative h-70
    >
      <div bg="blue-800/40" px-4 py-2 flex items-center>
        <div i-carbon:time text-green-300 text-xl mr-2 />
        <span font-bold>Setup Timeline Comparison</span>
      </div>
      <div px-3 py-4>
        <div flex justify-between items-center>
          <div text-sm text-zinc-400>Setup Timeline</div>
          <div text-sm text-zinc-400>Time Savings</div>
        </div>
        <div mt-4 relative h-40>
          <!-- Traditional timeline -->
          <div absolute top-0 left-0 right-0 flex flex-col gap-1>
            <div flex items-center>
              <div w-24 text-xs pr-2 text-right text-red-400>Traditional</div>
              <div h-6 rounded-l bg="red-900/50" w-10 flex items-center justify-center text-xs>10m</div>
              <div h-6 bg="red-800/50" w-16 flex items-center justify-center text-xs>30m</div>
              <div h-6 bg="red-700/50" w-24 flex items-center justify-center text-xs>1.5h</div>
              <div h-6 rounded-r bg="red-600/50" w-20 flex items-center justify-center text-xs>2h+</div>
            </div>
            <div flex items-center text="[10px]" text-zinc-400 pl-24>
              <div w-10 text-center text-nowrap>Repo</div>
              <div w-16 text-center text-nowrap>Config</div>
              <div w-24 text-center text-nowrap>Tooling</div>
              <div w-20 text-center text-nowrap>Components</div>
            </div>
          </div>
          <!-- Monorepo timeline -->
          <div absolute bottom-0 left-0 right-0 flex flex-col gap-1>
            <div flex items-center>
              <div w-24 text-xs pr-2 text-right text-green-400>With Monorepo</div>
              <div h-6 rounded bg="green-900/50" w-6 flex items-center justify-center text-xs>30s</div>
              <div h-6 w-8 flex items-center justify-center text-lg text-green-400 animate-pulse>⚡️</div>
            </div>
            <div flex items-center text="[10px]" text-zinc-400 pl-21>
              <div w-12 text-center>pnpm generate</div>
            </div>
          </div>
          <!-- Time saved indicator -->
          <div absolute right-8 top="1/2" transform translate-y="1/4" flex flex-col items-center>
            <div text-green-400 text-3xl font-bold>95%</div>
            <div text-sm text-zinc-400>Time Saved</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div
  v-click="3"
  mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
>
  <div
    flex items-center bg="green-900/30"
    rounded-lg py-3 px-6 gap-4
  >
    <div i-carbon:rocket text-green-300 text-3xl />
    <div>
      <div text-xl font-bold>From <span text-red-400>hours of manual setup</span> to <span text-green-400>production-ready in seconds</span></div>
      <div text-sm text-zinc-300 mt-1>New developers can start contributing immediately</div>
    </div>
  </div>
</div>

---
layout: center
glowSeed: 215
---

# Benefits at a Glance

<div grid grid-cols-3 gap-4 mt-8>

<v-clicks>

<div border="2 solid blue-800" bg="blue-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:data-center text-blue-300 text-5xl mb-4 mx-auto />
<div text-3xl font-bold mb-2>1</div>
<div font-bold text-lg mb-2>Single Source of Truth</div>
<div text-sm opacity-70>All versions in one catalog</div>
</div>

<div border="2 solid green-800" bg="green-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:share text-green-300 text-5xl mb-4 mx-auto />
<div text-3xl font-bold mb-2>5x+</div>
<div font-bold text-lg mb-2>Less Duplication</div>
<div text-sm opacity-70>Shared packages, not copy-paste</div>
</div>

<div border="2 solid purple-800" bg="purple-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:checkmark-outline text-purple-300 text-5xl mb-4 mx-auto />
<div text-3xl font-bold mb-2>0</div>
<div font-bold text-lg mb-2>Version Conflicts</div>
<div text-sm opacity-70>Impossible to drift</div>
</div>

</v-clicks>

</div>

<div grid grid-cols-3 gap-4 mt-4>

<v-clicks>

<div border="2 solid orange-800" bg="orange-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:commit text-orange-300 text-4xl mb-4 mx-auto />
<div font-bold text-lg>Atomic Changes</div>
<div text-sm opacity-70 mt-2>One commit updates everything</div>
</div>

<div border="2 solid pink-800" bg="pink-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:tools text-pink-300 text-4xl mb-4 mx-auto />
<div font-bold text-lg>Unified Tooling</div>
<div text-sm opacity-70 mt-2>Same standards everywhere</div>
</div>

<div border="2 solid cyan-800" bg="cyan-800/20" rounded-lg p-6 text-center backdrop-blur-sm transition duration-500 ease-in-out flex flex-col items-center>
<div i-carbon:user-favorite text-cyan-300 text-4xl mb-4 mx-auto />
<div font-bold text-lg>Faster Onboarding</div>
<div text-sm opacity-70 mt-2>One repo to learn</div>
</div>

</v-clicks>

</div>

---
class: py-8
glowSeed: 195
---

# Addressing Common Concerns

<span>Questions you might be asking</span>

<div mt-6 grid grid-cols-2 gap-6>

<v-clicks>

<div border="2 solid white/10" bg="white/5" rounded-lg overflow-hidden>
  <div bg="amber-800/40" px-4 py-2 flex items-center>
    <div i-carbon:help text-amber-300 text-xl mr-2 />
    <span font-semibold>"Won't the repo get too large?"</span>
  </div>
  <div px-4 py-3 text-sm opacity-80>
    pnpm's content-addressable store means packages are stored once globally, not in each project. The monorepo will actually use <span text-green-400 font-bold>less disk space</span> than 5 separate repos.
  </div>
</div>

<div border="2 solid white/10" bg="white/5" rounded-lg overflow-hidden>
  <div bg="amber-800/40" px-4 py-2 flex items-center>
    <div i-carbon:help text-amber-300 text-xl mr-2 />
    <span font-semibold>"What about CI/CD complexity?"</span>
  </div>
  <div px-4 py-3 text-sm opacity-80>
    Modern CI tools support monorepos natively. We can configure pipelines to only build/test apps affected by changes, making CI <span text-green-400 font-bold>faster, not slower</span>.
  </div>
</div>

<div border="2 solid white/10" bg="white/5" rounded-lg overflow-hidden>
  <div bg="amber-800/40" px-4 py-2 flex items-center>
    <div i-carbon:help text-amber-300 text-xl mr-2 />
    <span font-semibold>"How do we handle team ownership?"</span>
  </div>
  <div px-4 py-3 text-sm opacity-80>
    CODEOWNERS files define who owns which directories. Teams still have autonomy over their apps while sharing common infrastructure.
  </div>
</div>

<div border="2 solid white/10" bg="white/5" rounded-lg overflow-hidden>
  <div bg="amber-800/40" px-4 py-2 flex items-center>
    <div i-carbon:help text-amber-300 text-xl mr-2 />
    <span font-semibold>"What's the migration effort?"</span>
  </div>
  <div px-4 py-3 text-sm opacity-80>
    Migration can be done incrementally. We can start with shared packages while keeping existing apps, then migrate apps one at a time.
  </div>
</div>

</v-clicks>

</div>

<div
  v-click mt-4
  border="2 solid green-800" bg="green-800/20"
  rounded-lg px-6 py-3 flex items-center gap-3
>
  <div i-carbon:checkmark-filled text-green-400 text-2xl />
  <span>These concerns are valid but solved problems. Google, Meta, and Microsoft all use monorepos successfully at massive scale.</span>
</div>

---
class: py-8
glowSeed: 280
---

# Migration Approach

<span>A phased approach to minimize risk</span>

<div mt-6 />

<div flex items-center justify-between gap-4>

<v-clicks>

<div flex-1 border="2 solid blue-800" bg="blue-800/20" rounded-lg p-4>
  <div flex items-center gap-2 mb-3>
    <div bg="blue-700" rounded-full w-8 h-8 flex items-center justify-center font-bold>1</div>
    <span font-bold>Foundation</span>
  </div>
  <div text-sm opacity-80>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Set up monorepo structure</span>
    </div>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Configure pnpm workspaces</span>
    </div>
    <div flex items-center gap-2>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Create shared package scaffolds</span>
    </div>
  </div>
</div>

<div i-carbon:arrow-right text-2xl text-white />

<div flex-1 border="2 solid purple-800" bg="purple-800/20" rounded-lg p-4>
  <div flex items-center gap-2 mb-3>
    <div bg="purple-700" rounded-full w-8 h-8 flex items-center justify-center font-bold>2</div>
    <span font-bold>Extract Shared Code</span>
  </div>
  <div text-sm opacity-80>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Identify common utilities</span>
    </div>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Build @olct/core package</span>
    </div>
    <div flex items-center gap-2>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Build @olct/ui components</span>
    </div>
  </div>
</div>

<div i-carbon:arrow-right text-2xl text-white />

<div flex-1 border="2 solid green-800" bg="green-800/20" rounded-lg p-4>
  <div flex items-center gap-2 mb-3>
    <div bg="green-700" rounded-full w-8 h-8 flex items-center justify-center font-bold>3</div>
    <span font-bold>Migrate Apps</span>
  </div>
  <div text-sm opacity-80>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Move apps one at a time</span>
    </div>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Update to use shared packages</span>
    </div>
    <div flex items-center gap-2>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Deprecate old repos</span>
    </div>
  </div>
</div>

<div i-carbon:arrow-right text-2xl text-white />

<div flex-1 border="2 solid orange-800" bg="orange-800/20" rounded-lg p-4>
  <div flex items-center gap-2 mb-3>
    <div bg="orange-700" rounded-full w-8 h-8 flex items-center justify-center font-bold>4</div>
    <span font-bold>Optimize</span>
  </div>
  <div text-sm opacity-80>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Tune CI/CD pipelines</span>
    </div>
    <div flex items-center gap-2 mb-1>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Refine shared packages</span>
    </div>
    <div flex items-center gap-2>
      <div i-carbon:checkmark-outline text-green-400 text-xs />
      <span>Document best practices</span>
    </div>
  </div>
</div>

</v-clicks>

</div>

<div
  v-click mt-6
  border="2 solid cyan-800" bg="cyan-800/20"
  rounded-lg px-6 py-4 flex items-center gap-4
>
  <div i-carbon:information text-cyan-300 text-2xl />
  <div>
    <div font-bold>Low-Risk, Incremental Migration</div>
    <div text-sm opacity-80>Each phase delivers value independently. We can pause between phases if needed without losing progress.</div>
  </div>
</div>

---
class: py-6
glowSeed: 310
---

# Summary: The Measurable Impact

<span>What this initiative delivers</span>

<div mt-2 />

<div
  grid grid-cols-3 gap-3
  transition duration-500 ease-in-out h-90
  :class="$clicks < 1 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
>
  <v-clicks>
  <div
    border="2 solid lime-800" bg="lime-800/20"
    rounded-lg p-4 flex flex-col items-center
    transition-all duration-500 h-full
  >
    <div mb-3 flex-1 flex items-center justify-center>
      <div i-carbon:folder-shared text-green-500 text="[80px]" />
    </div>
    <div font-bold text-lg>Single Repository</div>
    <div
      text-lime-300 text-2xl font-bold mt-1
      flex items-center gap-1
    >
      <span>5+ → 1</span>
      <div i-carbon:arrow-down text-green-400 />
    </div>
    <div text-sm opacity-70 mt-1>Consolidated codebase</div>
    <div text-xs mt-2 bg="lime-900/30" rounded-lg px-3 py-1>
      Easier maintenance
    </div>
  </div>

  <div
    border="2 solid cyan-800" bg="cyan-800/20"
    rounded-lg p-4 flex flex-col items-center
    transition-all duration-500 h-full
  >
    <div mb-3 flex-1 flex items-center justify-center>
      <div i-carbon:renew text-cyan-500 text="[80px]" />
    </div>
    <div font-bold text-lg>Version Sync</div>
    <div
      text-cyan-300 text-2xl font-bold mt-1
      flex items-center gap-1
    >
      <span>100%</span>
      <div i-carbon:checkmark text-green-400 />
    </div>
    <div text-sm opacity-70 mt-1>Automatic via catalogs</div>
    <div text-xs mt-2 bg="cyan-900/30" rounded-lg px-3 py-1>
      Zero version drift
    </div>
  </div>

  <div
    border="2 solid purple-800" bg="purple-800/20"
    rounded-lg p-4 flex flex-col items-center
    transition-all duration-500 h-full
  >
    <div mb-3 flex-1 flex items-center justify-center>
      <div i-carbon:lightning text-yellow-500 text="[80px]" />
    </div>
    <div font-bold text-lg>App Setup Time</div>
    <div
      text-purple-300 text-2xl font-bold mt-1
      flex items-center gap-1
    >
      <span>95%</span>
      <div i-carbon:arrow-down text-green-400 />
    </div>
    <div text-sm opacity-70 mt-1>Pre-configured scaffolding</div>
    <div text-xs mt-2 bg="purple-900/30" rounded-lg px-3 py-1>
      Hours → seconds
    </div>
  </div>

  </v-clicks>
</div>

---
layout: center
class: text-center
glowSeed: 229
---

<div
  flex flex-col items-center
  transition duration-800 ease-out
>
  <div text-6xl font-bold mb-6>Thank You</div>

  <div
    flex gap-4
    transition duration-500 ease-in-out
  >
    <div
      border="2 solid green-800" bg="green-800/20"
      rounded-lg px-6 py-4 flex items-center gap-3
    >
      <div i-carbon:rocket text-green-400 text-2xl />
      <span>OLCT Monorepo Initiative by VINLI</span>
    </div>
  </div>

</div>
