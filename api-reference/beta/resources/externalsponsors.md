---
title: сложный тип externalSponsors
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 361ac6ff85d5b4462b39aa10e4f978ce7d486e40
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761872"
---
# <a name="externalsponsors-complex-type"></a>сложный тип externalSponsors

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется на этапе утверждения политики [назначения пакета доступа.](accesspackageassignmentpolicy.md) Это подтип [userSet,](userset.md)в котором значение указывает, что автором утверждения должны быть внешние спонсоры связанной организации `@odata.type` `#microsoft.graph.externalSponsors` пользователя. Этот одобрение применимо только к запросам пользователей, которые являются частью связанной организации.  При создании этапа утверждения политики назначения пакета доступа с внешнимиSponsors также включаем другого участника, например одного пользователя или члена группы, в случае, если подключенная организация не имеет внешнего спонсора.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Указывает, является ли автор резервного копирования автором резервного копирования. |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


