# scoop-thorium-bucket

Thorium Browser 用のカスタム Scoop bucket です。

## Packages

| パッケージ名 | 内容 | 実行コマンド |
|---|---|---|
| `thorium-avx2-beta` | Thorium Browser AVX2 beta portable build | `thorium-beta` |
| `thorium-sse3-beta` | Thorium Browser SSE3 beta portable build | `thorium-sse3-beta` |

## Install

```powershell
scoop bucket add mybucket https://github.com/neko12121/scoop-thorium-bucket
scoop install mybucket/thorium-avx2-beta
scoop install mybucket/thorium-sse3-beta
```

## Update

```powershell
scoop update
scoop update thorium-avx2-beta
scoop update thorium-sse3-beta
```

## Uninstall

```powershell
scoop uninstall thorium-avx2-beta
scoop uninstall thorium-sse3-beta
```

## Notes

- `thorium-avx2-beta` は AVX2 対応 CPU が必要です
- `thorium-sse3-beta` は AVX 非対応の古い CPU 向けです
- どちらも `gz83/thorium` の beta release を追跡しています
- GitHub Actions で 6 時間ごとにマニフェストを自動更新しています
