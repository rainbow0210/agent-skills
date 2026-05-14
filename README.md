# agent-skills

## 概要
このリポジトリは、GitHub Copilotなどのコーディングエージェントのカスタムスキルを管理するためのものです。

## 使い方
### 前提条件
- Visual Studio Code
- Git
- GitHub Copilot が利用可能な環境

### インストール方法
```bash
git clone https://github.com/username/agent-skills.git
cd agent-skills
```

### 基本的な使い方
スキルの配置先は用途に応じて分けます。

1. プロジェクト固有のスキルは、リポジトリ単位で管理します。OS に依存せず、プロジェクトを開いているルートディレクトリからの相対パスで配置します。

	```text
	.github/skills/<スキル名>/SKILL.md
	```

2. パーソナルスキルは、PC 上の全プロジェクトで共通して利用します。ユーザーごとのホームディレクトリ配下に配置します。

	Mac の場合:

	```text
	/Users/<ユーザー名>/.copilot/skills/<スキル名>/skill.md
	```

	ターミナル表現:

	```text
	~/.copilot/skills/<スキル名>/SKILL.md
	```

	Windows の場合:

	```text
	C:\Users\<ユーザー名>\.copilot\skills\<スキル名>\skill.md
	```

## 各スキルの説明
### create-readme
README.md を生成するためのスキルです。リポジトリ内の構成や内容を読み取り、 README.md を作成する手順とテンプレートを提供します。

## 主な機能
- GitHub Copilot用のAgent Skillsを管理します。

## 設定
特別な環境変数や設定ファイルは必要ありません。
スキル定義の追加や修正は、`<スキル名>/skill.md` を編集して行います。

## ライセンス
MIT License
