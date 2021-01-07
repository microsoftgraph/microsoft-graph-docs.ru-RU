---
title: Сложный тип userSet
description: Абстрактный базовый тип для типов, используемых в параметрах проверки запросов, утверждений и назначений политики назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 541bce7c65eaa9b284e9da5b520913b1be4ca8a3
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777727"
---
# <a name="userset-complex-type"></a>Сложный тип userSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запроса, утверждения и назначения политики [назначения пакета доступа.](accesspackageassignmentpolicy.md) Абстрактный базовый тип для типов [singleUser,](singleuser.md)[groupMembers,](groupmembers.md) [connectedOrganizationMembers,](connectedorganizationmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md)и [externalSponsors.](externalsponsors.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Для пользователя на стадии утверждения это свойство указывает, является ли пользователь резервным утверждением резервной копии. |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление userSet в JSON.  Обратите внимание, что userSet — это абстрактный базовый класс, поэтому он не будет отправлен или получен.  Вместо этого будет использоваться один из `@odata.type` `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` , `#microsoft.graph.connectedOrganizationMembers` ", `#microsoft.graph.requestorManager` " `#microsoft.graph.internalSponsors` `#microsoft.graph.externalSponsors` или " .

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


