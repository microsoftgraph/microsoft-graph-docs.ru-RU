---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: итемпревиевинфо
localization_priority: Normal
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7d2050a38e77e0cfa7176ba63756e9b9d8dcd384
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447628"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса Итемпревиевинфо

Пространство имен: Microsoft. Graph

Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [driveItem](driveitem.md).

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
| Команда         | строка | URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)
| постурл        | строка | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | строка | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Например:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачными.
