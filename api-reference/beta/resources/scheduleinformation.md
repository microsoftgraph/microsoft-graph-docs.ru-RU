---
title: Тип ресурса scheduleInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 0b7bbd861a044b28cd22603fd0ccc27d20f46fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078137"
---
# <a name="scheduleinformation-resource-type"></a>Тип ресурса scheduleInformation

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет доступности пользователя, ресурса или список рассылки для заданного периода времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|availabilityView |String |Представляет объединенное представление доступности всех элементов в `scheduleItems`. Представление состоит из слотами времени. Доступность во время каждого промежуток времени, обозначается: `0`свободен, = `1`= под вопросом, `2`= «занят», `3`= нет на месте, `4`= работа в другом месте.|
|error |[freeBusyError](freebusyerror.md) |Сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки. |
|scheduleId |String |SMTP-адрес пользователя, ресурса, идентифицирующий экземпляр **scheduleInformation**или список рассылки. |
|scheduleItems |[scheduleItem](scheduleitem.md) семейства сайтов |Содержит элементы, описывающие доступности пользователя или ресурса. |
|workingHours |[workingHours](workinghours.md) |Дни недели и часы работы пользователя в определенном часовом поясе. Они задаются в составе пользователя [mailboxSettings](mailboxsettings.md).|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->