---
title: тип ресурса shiftPreferences
description: Представляет доступность пользователя, который должен быть назначен сдвиги в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b807ba99eb811fb534276ae8ff7b4e180a3c94818fc00b5e57e111a6f75bf62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230433"
---
# <a name="shiftpreferences-resource-type"></a>тип ресурса shiftPreferences

Пространство имен: microsoft.graph

Представляет доступность пользователя, назначенного сменами в [расписании.](schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/shiftpreferences-get.md) | [shiftPreferences](shiftpreferences.md) | Ознакомьтесь с свойствами и отношениями объекта **shiftPreferences.** |
| [Обновление](../api/shiftpreferences-put.md) | [shiftPreferences](shiftpreferences.md) | Обновление **объекта shiftPreferences.** |

## <a name="properties"></a>Свойства

|Свойство          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | Идентификатор сущности. |
| @odata.etag | `Edm.String` | Ключ изменения для объекта. |
| availability | [коллекция shiftAvailability](shiftavailability.md) | Доступность пользователя, который должен быть запланирован для работы, и его шаблон повторения. |
| createdDateTime | `Edm.DateTimeOffset` | Timestamp, соответствующий моменту создания объекта. |
| lastModifiedDateTime | `Edm.DateTimeOffset` | Время, соответствующее времени последнего изменения объекта. |
| lastModifiedBy | [identitySet](identityset.md) | Удостоверение человека, который в последний раз изменил объект. |

## <a name="relationships"></a>Связи

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

