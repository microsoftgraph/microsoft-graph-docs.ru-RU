---
title: сложный тип Граупмемберс
description: Определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 576fd13962dcafaa876225393cc9165e5ef2ece2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078439"
---
# <a name="groupmembers-complex-type"></a>сложный тип Граупмемберс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md). `@odata.type`Значение " `#microsoft.graph.groupMembers` " указывает, что этот тип определяет коллекцию пользователей в клиенте, которые будут разрешены запрашивающими лицами, утверждающими лицами или рецензентами, которые являются участниками определенной группы.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |String | Идентификатор группы в Azure AD. |
| description |String | Имя группы в Azure AD. Только для чтения. |
| Создание резервной копии | Boolean | Для **граупмемберс** на этапе утверждения данное свойство указывает, что участники группы являются утверждающим резервным утверждающим. |

## <a name="json-representation"></a>Представление JSON


Ниже представлено представление типа в формате JSON.

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


