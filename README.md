# Fictional Machines

[日本語](#日本語) | [English](#english)

## 日本語

現実には存在しない機械を、工学的な設計とフィクションの両面から構築し、実際に動作する形で実現するための基本構想と分類体系です。

- [Fictional_Machines.md](Fictional_Machines.md)：基本構想・設計原則・分類体系（F／T／D／L／E／M／S／V／N）と、個別プロジェクトの共通記述フォーマット。版は文書の冒頭に記載（作業中の版で、随時更新します）。
- [Fictional_Machines.en.md](Fictional_Machines.en.md)：英語版（翻訳）。内容が異なる場合は日本語版を正とします。
- [Documentation_Rules.md](Documentation_Rules.md)：個別プロジェクトの文書管理ルール。仕様・物語・部品・製品デザイン・実装・決定記録・課題台帳を種類ごとに分けて管理します。実装のフォルダ構成（エミュレータ、ファームウェア、SDK、ハードウェア）も定めます。

### Claude Code プラグイン

このリポジトリは Claude Code のプラグインとしても使えます。文書管理の skill（`fictional-machines:project-docs`）と雛形が入ります。

```
/plugin install fictional-machines --marketplace gameguys-jp/fictional-machines
```

### 個別プロジェクト

- [fc85](https://github.com/gameguys-jp/fc85)：1985年に完成したが発売されなかった家庭用多目的コンピュータ

## English

A concept and classification system for building machines that do not exist in reality, through both engineering design and fiction, and for making them actually work.

- [Fictional_Machines.en.md](Fictional_Machines.en.md): The concept, design principles, and classification system (F / T / D / L / E / M / S / V / N), plus a common description format for individual projects. The version is given at the top of the document (a working draft, updated as needed).
- [Fictional_Machines.md](Fictional_Machines.md): The Japanese original. If the two versions differ, the Japanese original takes precedence.
- [Documentation_Rules.md](Documentation_Rules.md): Documentation rules for individual projects (Japanese only). Specifications, story, parts, product design, implementation, decision records, and open issues are kept in separate documents. It also defines the repository layout for implementations (emulator, firmware, SDK, hardware).

### Claude Code plugin

This repository also works as a Claude Code plugin. It provides a documentation skill (`fictional-machines:project-docs`) and templates.

```
/plugin install fictional-machines --marketplace gameguys-jp/fictional-machines
```

### Projects

- [fc85](https://github.com/gameguys-jp/fc85): A home multipurpose computer that was completed in 1985 but never released (documentation is in Japanese)

## License / ライセンス

[MIT](LICENSE)
