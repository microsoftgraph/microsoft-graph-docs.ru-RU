---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: итемпревиевинфо
localization_priority: Normal
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4d04384ba8efe27b369bfd4d73a560baf920cd53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009242"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса Итемпревиевинфо

Пространство имен: microsoft.graph

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
| Команда         | string | URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)
| постурл        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | string | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Например:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачными.

