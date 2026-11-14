# 測試覆蓋度：APITestka

測量日期：2026-10-28。數字來自這台 Windows 機器上的一次實測，不是估計，也不是只數檔案。

| 項目 | 內容 |
|---|---|
| 直譯器 | 3.11.9 |
| 直譯器說明 | 專案 .venv |
| 工具 | coverage 7.15.0，`coverage run --branch` |
| 測量範圍 | `je_api_testka` |
| 測試路徑 | `test` |
| 命令 | `python -m coverage run --branch --source=je_api_testka -m pytest test` |
| 敘述覆蓋 | 92.62%（6174 / 6666） |
| 分支覆蓋 | 84.83%（1247 / 1470） |
| 測試結果 | 841 passed, 2 skipped, 1 warning in 82.82s (0:01:22) |
| 耗時 | 87.3 秒 |

敘述覆蓋是執行到的敘述數除以全部敘述數。分支覆蓋是執行到的分支數除以全部分支數。兩者分開算，沒有把分支混進敘述百分比。

## 覆蓋較低的檔案

只列這次測量裡敘述覆蓋最低的檔案，最多 12 個。

| 檔案 | 敘述覆蓋 | 已覆蓋 / 敘述 |
|---|---:|---:|
| `je_api_testka/__main__.py` | 0.0% | 0 / 41 |
| `je_api_testka/mcp_server/__main__.py` | 0.0% | 0 / 3 |
| `je_api_testka/utils/test_record/run_context.py` | 42.86% | 3 / 7 |
| `je_api_testka/utils/assert_result/schema_check.py` | 47.06% | 24 / 51 |
| `je_api_testka/gui/pages/tools_page.py` | 50.75% | 34 / 67 |
| `je_api_testka/gui/pages/environment_page.py` | 60.0% | 51 / 85 |
| `je_api_testka/utils/mock_server/flask_mock_server.py` | 67.92% | 36 / 53 |
| `je_api_testka/gui/pages/executor_page.py` | 69.81% | 37 / 53 |
| `je_api_testka/graphql_wrapper/graphql_method.py` | 71.43% | 15 / 21 |
| `je_api_testka/pytest_plugin/plugin.py` | 73.08% | 19 / 26 |
| `je_api_testka/security/auth_helpers.py` | 74.36% | 29 / 39 |
| `je_api_testka/gui/pages/mock_page.py` | 74.51% | 38 / 51 |
