# Graph Report - /Users/muxing/workspace/content/wewrite  (2026-04-11)

## Corpus Check
- Corpus is ~26,801 words - fits in a single context window. You may not need a graph.

## Summary
- 410 nodes · 639 edges · 17 communities detected
- Extraction: 94% EXTRACTED · 6% INFERRED · 0% AMBIGUOUS · INFERRED: 40 edges (avg confidence: 0.54)
- Token cost: 0 input · 0 output

## God Nodes (most connected - your core abstractions)
1. `WeChatConverter` - 32 edges
2. `Theme` - 29 edges
3. `Eight-Step Publishing Pipeline` - 17 edges
4. `extract_exemplar()` - 13 edges
5. `_make_result()` - 13 edges
6. `WeWrite Content Pipeline` - 13 edges
7. `ImageProvider` - 12 edges
8. `analyze_styles()` - 9 edges
9. `_download_image()` - 9 edges
10. `main()` - 8 edges

## Surprising Connections (you probably didn't know these)
- `playbook.md Learned Rules` --semantically_similar_to--> `Exemplar Style Library`  [INFERRED] [semantically similar]
  references/learn-edits.md → SKILL.md
- `WeWrite Python Dependencies` --implements--> `Eight-Step Publishing Pipeline`  [INFERRED]
  requirements.txt → SKILL.md
- `WeWrite Python Dependencies` --conceptually_related_to--> `WeChat Rendering Constraints`  [INFERRED]
  requirements.txt → references/wechat-constraints.md
- `Writing Persona Presets` --conceptually_related_to--> `Exemplar Style Library`  [INFERRED]
  references/onboard.md → SKILL.md
- `Markdown to WeChat-compatible HTML converter.  Forked from wechat_article_skills` --uses--> `Theme`  [INFERRED]
  toolkit/converter.py → toolkit/theme.py

## Hyperedges (group relationships)
- **End-to-End WeChat Content Pipeline** — topic-selection_topic_selection_scoring, frameworks_seven_writing_frameworks, content-enhance_content_enhancement_strategies, writing-guide_humanized_writing_rules, seo-rules_wechat_seo_rules, visual-prompts_visual_ai_prompt_system, wechat-constraints_wechat_rendering_constraints [EXTRACTED 1.00]
- **Author Adaptation System** — onboard_onboarding_setup_flow, style-template_style_yaml_configuration, onboard_writing_persona_presets, learn-edits_playbook_learned_rules, skill_exemplar_style_library, learn-edits_edit_learning_flywheel [EXTRACTED 1.00]
- **Performance Feedback System** — effect-review_performance_review_loop, skill_history_yaml_article_ledger, topic-selection_topic_selection_scoring, frameworks_seven_writing_frameworks, content-enhance_content_enhancement_strategies [EXTRACTED 1.00]

## Communities

### Community 0 - "CLI Publishing Flow"
Cohesion: 0.04
Nodes (61): _build_gallery_html(), cmd_gallery(), cmd_image_post(), cmd_learn_theme(), cmd_preview(), cmd_publish(), cmd_themes(), _gallery_sample_markdown() (+53 more)

### Community 1 - "Image Provider Stack"
Cohesion: 0.05
Nodes (38): AzureOpenAIProvider, _build_provider(), _build_provider_chain(), _build_provider_from_entry(), _compress_image(), DashScopeProvider, DoubaoProvider, _download_image() (+30 more)

### Community 2 - "Humanness Scoring"
Cohesion: 0.07
Nodes (43): _bell_curve(), build_param_scores(), calibrate_tiers(), compute_composite(), main(), _make_result(), _print_verbose(), Split text by Chinese sentence-ending punctuation. (+35 more)

### Community 3 - "Theme Learning"
Cohesion: 0.09
Nodes (32): adjust_lightness(), analyze_styles(), _attach_title(), derive_darkmode(), extract_styles(), fetch_article(), generate_theme_yaml(), is_gray() (+24 more)

### Community 4 - "Exemplar Extraction"
Cohesion: 0.1
Nodes (29): compute_paragraph_cv(), compute_vocab_temperature(), count_short_paragraphs(), detect_category(), extract_closing(), extract_emotional_peak(), extract_exemplar(), extract_headings() (+21 more)

### Community 5 - "Diagnostic Checks"
Cohesion: 0.15
Nodes (22): check_config(), check_dependencies(), check_dimensions(), check_enhancements(), check_style(), compute_summary(), file_status_map(), format_json() (+14 more)

### Community 6 - "Edit Learning"
Cohesion: 0.15
Nodes (21): aggregate_patterns(), compute_confidence(), compute_diff(), extract_title(), fetch_wechat_draft(), load_all_lessons(), load_text(), main() (+13 more)

### Community 7 - "Writing System Docs"
Cohesion: 0.22
Nodes (22): Content Enhancement Strategies, Share-Worthy Angle Discovery, Performance Review Loop, Seven Writing Frameworks, Compounding Style Adaptation, Edit Learning Flywheel, playbook.md Learned Rules, Onboarding Setup Flow (+14 more)

### Community 8 - "Article Fetching"
Cohesion: 0.15
Nodes (19): _elem_to_md(), _extract_metadata(), fetch_article(), _fetch_camoufox(), fetch_html(), _fetch_playwright(), _fetch_requests(), _has_content() (+11 more)

### Community 9 - "Draft Publishing API"
Cohesion: 0.22
Nodes (10): create_draft(), create_image_post(), DraftResult, get_draft(), html_to_plaintext(), ImagePostResult, Create a WeChat image post (小绿书/图片帖) draft.      This uses article_type="newspic, Create a draft in WeChat.     API: POST https://api.weixin.qq.com/cgi-bin/draft/ (+2 more)

### Community 10 - "Stats Sync"
Cohesion: 0.29
Nodes (9): fetch_article_summary(), fetch_article_total(), _get_access_token(), _load_toolkit_config(), main(), Fetch daily article summary.     API: POST /datacube/getarticlesummary     date, Fetch cumulative article stats.     API: POST /datacube/getarticletotal, Match stats to history.yaml entries and update. (+1 more)

### Community 11 - "Playbook Analysis"
Cohesion: 0.29
Nodes (9): build_analysis_batches(), compute_corpus_stats(), load_corpus(), main(), output_analysis_prompt(), Load all markdown files from corpus directory., Compute aggregate statistics from the corpus., Split articles into batches for LLM analysis. (+1 more)

### Community 12 - "Hot Topic Fetchers"
Cohesion: 0.22
Nodes (9): deduplicate(), fetch_baidu(), fetch_toutiao(), fetch_weibo(), main(), Remove duplicates by exact title match., Fetch Weibo hot search., Fetch Toutiao hot board. (+1 more)

### Community 13 - "WeChat Media API"
Cohesion: 0.27
Nodes (9): get_access_token(), _guess_content_type(), Get access_token with caching.     Cache key: appid     API: GET https://api.wei, Detect content type from file extension., Upload image for use inside article content.     API: POST https://api.weixin.qq, Upload cover image as permanent material.     API: POST https://api.weixin.qq.co, TokenResult, upload_image() (+1 more)

### Community 14 - "OpenClaw Builder"
Cohesion: 0.33
Nodes (8): build(), main(), Remove Claude Code-specific frontmatter keys., Apply all body transformations., Split YAML frontmatter from body. Returns (frontmatter, body)., split_frontmatter(), transform_body(), transform_frontmatter()

### Community 15 - "SEO Keyword Analysis"
Cohesion: 0.36
Nodes (7): analyze_keyword(), baidu_suggestions(), main(), Get Baidu search autocomplete suggestions — proxy for search volume., Get 360 search suggestions — second source for search volume proxy., Analyze a keyword's SEO potential., so360_suggestions()

### Community 16 - "Image Generation"
Cohesion: 1.0
Nodes (1): Generate an image and return raw bytes.

## Knowledge Gaps
- **136 isolated node(s):** `Fetch daily article summary.     API: POST /datacube/getarticlesummary     date`, `Fetch cumulative article stats.     API: POST /datacube/getarticletotal`, `Match stats to history.yaml entries and update.`, `Load all markdown files from corpus directory.`, `Compute aggregate statistics from the corpus.` (+131 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `Image Generation`** (1 nodes): `Generate an image and return raw bytes.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Are the 9 inferred relationships involving `WeChatConverter` (e.g. with `Theme` and `Load config from first found config.yaml.`) actually correct?**
  _`WeChatConverter` has 9 INFERRED edges - model-reasoned connections that need verification._
- **Are the 26 inferred relationships involving `Theme` (e.g. with `ConvertResult` and `WeChatConverter`) actually correct?**
  _`Theme` has 26 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Fetch daily article summary.     API: POST /datacube/getarticlesummary     date`, `Fetch cumulative article stats.     API: POST /datacube/getarticletotal`, `Match stats to history.yaml entries and update.` to the rest of the system?**
  _136 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `CLI Publishing Flow` be split into smaller, more focused modules?**
  _Cohesion score 0.04 - nodes in this community are weakly interconnected._
- **Should `Image Provider Stack` be split into smaller, more focused modules?**
  _Cohesion score 0.05 - nodes in this community are weakly interconnected._
- **Should `Humanness Scoring` be split into smaller, more focused modules?**
  _Cohesion score 0.07 - nodes in this community are weakly interconnected._
- **Should `Theme Learning` be split into smaller, more focused modules?**
  _Cohesion score 0.09 - nodes in this community are weakly interconnected._