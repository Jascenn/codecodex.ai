# 价格和运营时长更新清单

## 需要修改的文件列表

### 核心配置文件
1. `_config.yml`
   - title (标题中的价格)
   - description (描述中的价格和运营时长)
   - carpool_plans (套餐配置)
   - service_features (服务特点中的运营时长)

### 中文页面
2. `index.html`
   - description (价格和运营时长)
   - keywords (价格关键词)

3. `carpool.md`
   - description (价格和运营时长)
   - keywords (价格关键词)
   - 价格表格
   - 核心优势中的运营时长

4. `about.md`
   - description (运营时长)
   - 核心服务中的价格和运营时长

5. `comprehensive-guide.md`
   - 价格表格
   - 核心优势中的运营时长
   - 常见问题中的运营时长

6. `deployment-guide.md`
   - 第一步中的套餐价格
   - 底部推荐中的价格
   - 温馨提示中的运营时长

7. `faq.md`
   - Q1: 价格和运营时长
   - Q2: 周额度分配中的价格
   - 价格对比表
   - 其他多处运营时长引用

### 中文文章
8. `_posts/2026-02-27-claude-code-carpool-service.md`
   - summary (价格和运营时长)
   - 套餐价格表
   - 核心优势中的运营时长
   - 常见问题中的运营时长
   - 底部提示中的运营时长

9. `_posts/2025-09-30-why-choose-lioncc-claude-code-carpool.md`
   - 价格对比表
   - 灵活拼车选择中的价格
   - 服务保障中的运营时长
   - 用户反馈中的价格
   - 不太适合场景中的价格

10. `_posts/2025-11-07-bettafish-lioncc-api-deployment-guide.md`
    - 底部推荐中的价格

### 英文页面
11. `en/carpool.md`
    - description (价格和运营时长)
    - keywords (价格关键词)
    - 标题中的运营时长
    - 价格表格

12. `en/about.md`
    - description (运营时长)
    - 核心服务中的价格和运营时长

13. `en/comprehensive-guide.md`
    - 价格表格
    - 核心优势中的运营时长

14. `en/deployment-guide.md`
    - 第一步中的套餐价格
    - 底部推荐中的价格

15. `en/faq.md`
    - Q1: 价格和运营时长
    - Q2: 周额度分配中的价格

### 英文文章
16. `_posts_en/2025-11-06-claude-code-carpool-service.md`
    - summary (价格和运营时长)
    - description (价格和运营时长)
    - 价格表格

17. `_posts_en/2025-11-06-why-choose-lioncc-claude-code-carpool.md`
    - 价格对比表
    - 灵活拼车选择中的价格
    - 不太适合场景中的价格

18. `_posts_en/2025-11-07-bettafish-lioncc-api-deployment-guide.md`
    - 底部推荐中的价格

## 快速搜索命令

### 搜索所有价格引用
```bash
grep -rn "398\|768\|2200\|2400\|400元" --include="*.md" --include="*.yml" --include="*.html" | grep -v vendor | grep -v ".jekyll-cache" | grep -v "_site"
```

### 搜索运营时长引用
```bash
grep -rn "三个月\|3个月\|3 个月\|五个月\|5个月\|5 个月" --include="*.md" --include="*.yml" --include="*.html" | grep -v vendor | grep -v ".jekyll-cache" | grep -v "_site"
```

## 修改要点

### 价格修改
- 6人车：¥398 → ¥400
- 3人车：¥768 → 移除
- 1人车：¥2200 → ¥2400

### 周额度说明
- 6人车：周限额 100刀/人，累计 400刀/人
- 1人车：周限额 800刀，累计 3200刀

### 运营时长
- 3个月 → 5个月
- 3+ months → 5+ months

## 注意事项
1. 修改前先用 `Read` 工具读取文件
2. 使用 `Edit` 工具进行精确替换
3. 修改完成后重启 Jekyll 服务器查看效果
4. 英文文件中的价格保持人民币符号 ¥
5. **重要：修改文章后需要同步更新"最后更新时间"**
   - 中文格式：`*最后更新：2026年3月26日*`
   - 英文格式：`*Last updated: March 26, 2026*`
   - 搜索命令：`grep -rn "最后更新\|Last updated" --include="*.md"`
