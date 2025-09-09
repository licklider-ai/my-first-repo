## https://github.com/licklider-ai/my-first-repo.git へ PUSH するまでの流れ

### 1. hello-world の実行
PowerShell または コマンドプロンプト（Windows）を開き、以下を実行します。

```bash
docker run hello-world
```

➡ `Hello from Docker!` というメッセージが表示されれば、Docker が正常に動作しています。

---

### 2. GitHub リポジトリの作成
1. GitHub にログインし、トップページ右上の **+** をクリックして **New repository** を選択
2. リポジトリ名を入力（例: `my-first-repo`）
3. **Public** または **Private** を選択
4. **Create repository** をクリックしてリポジトリを作成

---

### 3. ローカルでの README.md 作成と初期化
特定のプロジェクト専用のフォルダを作成して、その中でGit を初期化します。

```bash
mkdir my-first-repo
git init
```

README.md を作成して内容を記述します。

```bash
echo "# My First Repository" >> README.md
```

変更をコミットします。

```bash
git add .
git commit -m "Add initial README"
```

---

### 4. リモートリポジトリを追加して PUSH
GitHub のリポジトリページに表示されている URL をコピーして、以下を実行します。

```bash
git remote add origin <GitHubリポジトリのURL>
git push -u origin main
```