---
title: сложный тип userSet
description: Абстрактный базовый тип для типов, используемых в параметрах проверки запросов, утверждений и назначений политики назначения пакетов доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bd16a117b7b1bd93db1977ffb50ba501b4e801ed
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289534"
---
# <a name="userset-complex-type"></a>сложный тип userSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Это абстрактный базовый тип, унаследованный следующими типами ресурсов:
+ [singleUser](singleuser.md)
+ [groupMembers](groupmembers.md)
+ [connectedOrganizationMembers](connectedorganizationmembers.md)
+ [requestorManager](requestormanager.md)
+ [internalSponsors](internalsponsors.md)
+ [externalSponsors](externalsponsors.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Для пользователя на стадии утверждения это свойство указывает, является ли он резервным копией. |

## <a name="json-representation"></a>Представление JSON

Ниже представленА JSON-представление userSet. [UserSet](userset.md) — это абстрактный базовый класс, поэтому он не будет отправлен или получен.  Вместо этого будет использоваться одно из следующих значений, представляющих `@odata.type` унаследованные типы:
+ `#microsoft.graph.singleUser`
+ `#microsoft.graph.groupMembers`
+ `#microsoft.graph.connectedOrganizationMembers`
+ `#microsoft.graph.requestorManager`
+ `#microsoft.graph.internalSponsors`
+ `#microsoft.graph.externalSponsors`

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.userSet",
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


