---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: Итемпревиевинфо
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585239"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса Итемпревиевинфо

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
| Постурл        | строка | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | строка | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Пример:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачными.
