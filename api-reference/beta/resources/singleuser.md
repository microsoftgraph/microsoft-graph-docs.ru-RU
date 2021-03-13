---
title: сложный тип singleUser
description: Определяет пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761046"
---
# <a name="singleuser-complex-type"></a>сложный тип singleUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Это значение указывает на то, что этот набор пользователей определяет конкретного пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или  `@odata.type` `#microsoft.graph.singleUser` рецензента.

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |String | ID пользователя в Azure AD. |
| description |String | Имя пользователя в Azure AD. Только для чтения. |
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
  "id": "string (identifier)",
  "description": "string"
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


