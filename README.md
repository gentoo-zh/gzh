# gzh

gentoo-zh overlay 维护用的确定性命令行工具：bump、依赖比对、Manifest、pkgcheck、构建测试、issue 批处理。原来放在 [gentoo-zh/skills](https://github.com/gentoo-zh/skills)，拆出来单独维护；skill 只写步骤，不依赖它。

```bash
pip install -e '.[test]'
python -m pytest -q
gzh --help
```

需要 Python 3.11、Portage、`pkgdev`、`pkgcheck`；在 overlay 工作树内运行，或设置 `GZH_OVERLAY_DIR`。
