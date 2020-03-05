---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7b121a1bd3369eebd752651fa412510daf943b76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520789"
---
# <a name="serviceinformation-resource-type"></a>Тип ресурса Сервицеинформатион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовые описательные данные о облачных службах, на которые пользователь выбрал ссылку из своей учетной записи.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                            |
|:-------------|:------------|:-------------------------------------------------------|
|name          | String      | Имя облачной службы (например, Twitter, Инстаграм). |
|webUrl        | String      | Содержит URL-адрес для службы, на которую указывает ссылка.     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
