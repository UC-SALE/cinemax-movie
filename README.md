# CINEMAX — Кино тасалбарын вэб

Энэ бол static HTML төсөл. GitHub Pages дээр шууд host хийж болно.

## GitHub Pages дээр host хийх алхамууд

### 1. Шинэ GitHub repo үүсгэх
1. https://github.com/new руу орно
2. Repository name: `cinemax` (эсвэл өөрийн дуртайгаар)
3. Public сонгоно (Pages-ийг үнэгүй ашиглахад)
4. **Add a README** болон бусад зүйлийг сонгох шаардлагагүй
5. **Create repository** дарна

### 2. Файлуудыг upload хийх
GitHub-ийн вэб дээрээс шууд:
1. Шинэ repo дотор **"uploading an existing file"** холбоосыг дарна
2. Энэ хавтас доторх бүх файлыг (`index.html`, `README.md`, `.nojekyll`, `404.html`) drag-and-drop хийнэ
3. **Commit changes** дарна

Эсвэл command line-аар:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin main
```

### 3. GitHub Pages-г идэвхжүүлэх
1. Repo-гийн **Settings** → зүүн талаас **Pages** дарна
2. **Source**: `Deploy from a branch` сонгоно
3. **Branch**: `main` болон `/ (root)` сонгоод **Save** дарна
4. 1-2 минутын дараа `https://<USERNAME>.github.io/<REPO>/` хаягаар нээгдэнэ

## Файлуудын тайлбар
- `index.html` — Үндсэн хуудас (бүх CSS, JS дотор нь багтсан)
- `404.html` — Олдоогүй хуудсыг index руу буцаана
- `.nojekyll` — GitHub-ийн Jekyll боловсруулалтыг идэвхгүй болгоно (зайлшгүй)
- `README.md` — Энэхүү заавар

## Custom domain холбох (заавал биш)
Settings → Pages → Custom domain хэсэгт өөрийн домэйнээ оруулаад, DNS дээрээ CNAME record нэмнэ.
