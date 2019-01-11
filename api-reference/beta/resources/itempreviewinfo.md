---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857346"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса ItemPreviewInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **ItemPreviewInfo** содержит сведения о том, как внедрить Предварительный просмотр [DriveItem](driveitem.md).

## <a name="json-representation"></a>Представление JSON

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Свойства

| Имя           | Тип   | Описание
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)
| postUrl        | string | URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)
| postParameters | string | Параметры отправки для включения при использовании postUrl

В зависимости от текущего состояния поддержка указанные параметры могут быть возвращены getUrl, postUrl или оба.

postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом. Пример:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адреса и параметры должны считаться непрозрачный.
