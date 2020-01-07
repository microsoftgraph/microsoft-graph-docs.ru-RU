---
title: Тип ресурса Шифтпреференцес
description: Представляет доступность пользователя для назначения смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 083b0ad81ffee25d8a03bf5ff38815d2ca0155a8
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952274"
---
# <a name="shiftpreferences-resource-type"></a>Тип ресурса Шифтпреференцес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет доступность пользователя для назначения смен в [расписании](schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/shiftpreferences-get.md); | [шифтпреференцес](shiftpreferences.md) | Чтение свойств и связей объекта **шифтпреференцес** . |
| [обновление](../api/shiftpreferences-put.md). | [шифтпреференцес](shiftpreferences.md) | Обновление объекта **шифтпреференцес** . |

## <a name="properties"></a>Свойства

|Свойство          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | Идентификатор объекта. |
| @odata.etag | `Edm.String` | Ключ изменения для объекта. |
| availability | Коллекция [шифтаваилабилити](shiftavailability.md) | Доступность пользователя для планирования работы и расписания повторения. |
| createdDateTime | `Edm.DateTimeOffset` | Временная метка, соответствующая моменту создания объекта. |
| lastModifiedDateTime | `Edm.DateTimeOffset` | Временная метка, соответствующая дате последнего изменения объекта. |
| lastModifiedBy | [identitySet](identityset.md) | Идентификатор пользователя, который последним изменил объект. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
