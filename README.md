# Morok releases

Signed lists and binaries of the protocol engines of Morok. The program reads this repository
when it checks for engine updates. There is no source code here.

| What | Where |
|---|---|
| The list of engine versions and its signature | `index/engines.json`, `index/engines.json.minisig` |
| Camouflage presets and their signature | `index/presets.json`, `index/presets.json.minisig` |
| Engine binaries | GitHub releases tagged `<engine>-v<version>`, with `SHA256SUMS` |

The lists are signed with minisign (Ed25519); the public key is built into the program. An engine file is
accepted only if its size and SHA-256 match the signed list, so a file changed on the way is rejected. Every
signed list stays in the git history of this repository.

---

Подписанные списки и файлы движков протоколов Morok. Программа читает этот репозиторий, когда
проверяет обновления движков. Исходного кода здесь нет.

| Что | Где |
|---|---|
| Список версий движков и его подпись | `index/engines.json`, `index/engines.json.minisig` |
| Пресеты маскировки и их подпись | `index/presets.json`, `index/presets.json.minisig` |
| Файлы движков | выпуски GitHub с тегом `<движок>-v<версия>`, рядом `SHA256SUMS` |

Списки подписаны minisign (Ed25519); открытый ключ вшит в программу. Файл движка принимается, только если его
размер и SHA-256 совпали с подписанным списком, — изменённый по дороге файл отбрасывается. Каждый подписанный
список остаётся в истории git этого репозитория.
