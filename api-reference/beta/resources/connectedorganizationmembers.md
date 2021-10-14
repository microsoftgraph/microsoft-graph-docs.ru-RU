---
title: connectedOrganizationMembers сложный тип
description: Тип connectedOrganizationMembers определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивателя, утверждения или рецензента.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0baaea3f8d6e917d072b8e9f5933b3388e1a0324
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289240"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers сложный тип

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах запросов политики назначения [пакета доступа.](accesspackageassignmentpolicy.md) Значение указывает, что этот тип определяет коллекцию пользователей, связанных с подключенной организацией, которым будет разрешено `@odata.type` `#microsoft.graph.connectedOrganizationMembers` запрашивать пакет доступа. [](connectedorganization.md)

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |Строка | ID связанной организации в управлении правами. |
| description |Строка | Имя связанной организации. Только для чтения. |
| isBackup | Boolean | Не используется в настоящее время. |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
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
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


