<template>
  <h1>Vite Playground</h1>
  <TestEnv />
  <h2>Async Component</h2>
  <TestAsync />
  <TestModuleResolve />
  <TestHmr />
  <TestPostCss />
  <TestScopedCss />
  <TestCssModules />
  <TestCssAtImport />
  <TestPreprocessors />
  <TestAssets />
  <TestSrcImport />
  <TestJsonImport />
  <TestTs />
  <TestJsx />
  <TestAlias />
  <TestTransform />
  <TestRewriteOptimized />
  <TestCustomBlocks />
  <TestOptimizeLink />
  <TestRewriteUnoptimized />
  <TestNormalizePublicPath />
  <TestDynamicImport />
</template>

<script>
import { defineAsyncComponent } from 'vue'
import TestEnv from './TestEnv.vue'
import TestModuleResolve from './TestModuleResolve.vue'
import TestHmr from './TestHmr/TestHmr.vue'
import TestPostCss from './TestPostCss.vue'
import TestScopedCss from './TestScopedCss.vue'
import TestCssModules from './TestCssModules.vue'
import TestPreprocessors from './TestPreprocessors.vue'
import TestSrcImport from './src-import/TestBlockSrcImport.vue'
import TestAssets from './test-assets/TestAssets.vue'
import TestJsonImport from './TestJsonImport.vue'
import TestTs from './ts/TestTs.vue'
import TestJsx from './TestJsx.vue'
import TestAlias from './TestAlias.vue'
import TestTransform from './TestTransform.vue'
import TestRewriteOptimized from './rewrite-optimized/TestRewriteOptimized.vue'
import TestCssAtImport from './css-@import/TestCssAtImport.vue'
import TestCustomBlocks from './custom-blocks/TestCustomBlocks.vue'
import TestOptimizeLink from './optimize-linked/TestOptimizeLink.vue'
import TestRewriteUnoptimized from './rewrite-unoptimized/TestRewriteUnoptimized.vue'
import TestNormalizePublicPath from './TestNormalizePublicPath.vue'
import TestDynamicImport from './dynamic-import/TestDynamicImport.vue'

export default {
  components: {
    TestEnv,
    TestModuleResolve,
    TestHmr,
    TestPostCss,
    TestScopedCss,
    TestCssModules,
    TestPreprocessors,
    TestCssAtImport,
    TestSrcImport,
    TestAssets,
    TestJsonImport,
    TestTs,
    TestJsx,
    TestAlias,
    TestTransform,
    TestAsync: defineAsyncComponent(() => import('./TestAsync.vue')),
    TestRewriteOptimized,
    TestCustomBlocks,
    TestOptimizeLink,
    TestRewriteUnoptimized,
    TestNormalizePublicPath,
    TestDynamicImport
  }
}
</script>
