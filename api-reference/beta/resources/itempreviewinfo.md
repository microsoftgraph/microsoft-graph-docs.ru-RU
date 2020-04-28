---
author: kevinlam
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра DriveItem.
ms.date: 3/16/2018
title: 'Итемпревиевинфо: API OneDrive'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4e4a26a9db6ebf4cbedb37fb60b177fa837c16d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523060"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса Итемпревиевинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [DriveItem](driveitem.md).

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

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Например:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачными.
