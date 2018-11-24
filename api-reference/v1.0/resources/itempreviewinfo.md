---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2018
ms.locfileid: "26606419"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса itemPreviewInfo

Ресурс **itemPreviewInfo** содержит сведения о том, как внедрить Предварительный просмотр [driveItem](driveitem.md).

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
