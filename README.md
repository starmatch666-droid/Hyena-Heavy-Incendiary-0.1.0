# R-4 鬣狗：重穿与强化燃烧

将 R-4 鬣狗的子弹由中甲穿透 AP3 提升为重甲穿透 AP4，保留原版普通燃烧类型，并把每发燃烧累积从 3 提高到 10。

- 基础人机工效：30 → 60
- 基础弹匣容量：15 → 20
- 保留原版 220 直击伤害、45 耐久伤害、备弹、后坐力与 190 RPM
- 仅修改 R-4 自身的 DamageInfo、WeaponMagazineComponent 和 WeaponDataComponent，不触碰全局燃烧规则

燃烧仍遵循游戏自身的目标易感性与状态规则。

## 依赖

**只需要 Bingus Shared Loader v15 及以上**（或兼容的新版本）。

无需其他前置，下载即用。

## 安装

导入本包到 Arsenal / HD2 Mod Manager，启用后部署，彻底退出游戏再重新启动。Loader 放到列表最后（若开启「首个 mod 优先」则放最前）。

## 版本与适配

- 适配游戏构建 **25327279**。
- 已通过离线验证；**未单独做运行时实测**。

## 日志

```
%LOCALAPPDATA%\CowboyBingus\Helldivers2\Logs\HyenaHeavyIncendiary.log
```

写入成功会记录 `applied_template_gameplay_unverified`；数据不匹配时记录 `*_not_write` 并**拒绝写入**，不会强行覆盖。

## 注意

- 内存模组属**客户端运行时改动**：只在本次游戏会话内生效，退出游戏即恢复原状。
- 联机表现可能与队友不一致，并存在**反作弊风险**。建议仅在知情固定队环境中使用。
- 卸载：用管理器禁用本包并重新部署；手动安装需保持 `patch_N` 编号连续，**不要直接删除中间编号的文件**。
