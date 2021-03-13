---
title: сложный тип groupMembers
description: Определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утверждения или рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0069cd6a8fd738c17a9035b519c4f141c3a5fa55
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761418"
---
# <a name="groupmembers-complex-type"></a>сложный тип groupMembers

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Значение "" указывает, что этот тип определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивателя, утверждения или рецензента, которые являются членами `@odata.type` `#microsoft.graph.groupMembers` определенной группы.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |String | ID группы в Azure AD. |
| description |String | Имя группы в Azure AD. Только для чтения. |
| isBackup | Boolean | Для **groupMembers** на стадии утверждения это свойство указывает, что участники группы являются резервным утверждением резервного копирования. |

## <a name="json-representation"></a>Представление JSON


Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


