---
title: Тип ресурса scheduleInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521910"
---
# <a name="scheduleinformation-resource-type"></a>Тип ресурса scheduleInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет доступности пользователя, ресурса или список рассылки для заданного периода времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
