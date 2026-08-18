# 베이스라인 (내 변경 이전)

fork 직후 `1c3122e` (v0.26.0b1), macOS, `uv run pytest -q`:

```
3 failed, 2085 passed, 3 skipped, 3 warnings in 20.95s
```

기존 실패 3건 — **내 변경과 무관하며, PR 본문에서 회귀와 구분해 밝혀야 한다**:

- `tests/test_move_accounts.py::TestMoveUnreadableSourceIsNotAbsent::test_unreadable_enc_aborts_the_move_before_anything_changes`
- `tests/test_real_store_guard.py::test_c0_a_scratch_home_still_protects_the_os_account_home_store`
- `tests/test_swap_accounts.py::TestSwapUnreadableSourceIsNotAbsent::test_unreadable_enc_aborts_the_swap_before_anything_changes`
