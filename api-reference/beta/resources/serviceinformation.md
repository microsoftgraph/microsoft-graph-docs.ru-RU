---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ba13967a2b4373c1a3599baf2fcc856967fbb00c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939833"
---
# <a name="serviceinformation-resource-type"></a>Тип ресурса Сервицеинформатион

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
