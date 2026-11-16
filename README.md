# ripa-1603

Heavy files (page scans, engravings, thumbnails, data) for the book «Cesare Ripa, Iconologia, Roma 1603» of https://github.com/nfhours/library.
Published via GitHub Pages: https://nfhours.github.io/ripa-1603/

Source scans: Heidelberg University Library (Public Domain Mark 1.0, DOI 10.11588/diglit.3396), supplemented from Internet Archive copies (see `sources.json`).

## Структура
- `book.json`, `lib-thumb.webp`, `cover.webp` — паспорт книги и обложка (читаются сайтом через `library.json`, `path` — абсолютный URL этого репозитория)
- `scans/NNNN.webp` (высота 1600), `scans/thumb/`, `scans/sizes.json` — страницы (549; кадры 0550–0557 — чужой трактат и крышка, исключены), нумерация = номер кадра Heidelberg; плашка-ватермарк внизу срезана
- `pagemap.json` — скан ↔ печатная страница (`printed`), колонтитул, флаги сбоев нумерации печати, лист IA (`ia_leaf`)
- `entries.json` — 662 статьи по «Tavola delle Figure» (тексты пока пусты), `engravings.json` + `img/`, `thumb/` — гравюры по рамкам (сборка: `tools/build_ripa1603.py` в nfhours/library)
- `sources.json` — источники страниц
