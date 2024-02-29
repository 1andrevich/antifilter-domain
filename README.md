# Назначение

Форк оригинального проекта для сборки dat-файлов Geosite для проектов V2Fly, XRay и подобных на основе списков [Antifilter](https://antifilter.download/)
Сборка проводится автоматически ежедневно через GitHub Actions

## Использованные списки
- Файл ```geosite.dat``` собирается на основе списка <https://community.antifilter.download/list/domains.lst>

## Ссылки на скачивание

- **geosite.dat**：<https://github.com/1andrevich/antifilter-domain/releases/latest/download/geosite.dat>

## Пример использования

```json
{
  "routing": {
      "rules": [
      {
        "domain": [
          "ext:geosite.dat:antifilter"
        ],
        "type": "field",
        "outboundTag": "proxy"
      },
      {
        "type": "field",
        "outboundTag": "direct"
      }
    ]
  }
}
```
