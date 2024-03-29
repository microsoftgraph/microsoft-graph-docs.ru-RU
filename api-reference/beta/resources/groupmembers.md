---
title: сложный тип groupMembers
description: Определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утверждения или рецензента.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ce18ed739e1701e004c92f408d0276ef17f5d264
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289961"
---
# <a name="groupmembers-complex-type"></a>сложный тип groupMembers

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Значение указывает, что этот тип определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утвержденного или рецензента, которые являются членами `@odata.type` `#microsoft.graph.groupMembers` определенной группы.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |Строка | ID группы в Azure AD. |
| description |Строка | Имя группы в Azure AD. Только для чтения. |
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
  "id": "String (identifier)",
  "description": "String",
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


