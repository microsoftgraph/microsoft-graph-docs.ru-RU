---
title: сложный тип singleUser
description: Определяет пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или рецензента.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7ccc22478a470047e6f65387419bfc0364bf548
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60290248"
---
# <a name="singleuser-complex-type"></a>сложный тип singleUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Это значение указывает на то, что этот userSet идентифицирует определенного пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или  `@odata.type` `#microsoft.graph.singleUser` рецензента.

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |Строка | ID пользователя в Azure AD. |
| description |Строка | Имя пользователя в Azure AD. Только для чтения. |
| isBackup | Boolean | Для **одного пользователя на** стадии утверждения указывает, является ли пользователь резервным кодом. |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "String (identifier)",
  "description": "String"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


