---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513608"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса educationSynchronizationCustomization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. 

>**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **optionalPropertiesToSync** | Коллекция строк. |  Коллекция имен свойств для синхронизации. Если задано значение null, все свойства будут синхронизированы.       |
| **synchronizationStartDate** | DateTime |  Дата начала для синхронизации. Это значение необходимо задать в будущем. Если параметр имеет значение null, ресурс будет синхронизирован после завершения настройки профиля. **Примечание:** Применяется только к свойству **StudentEnrollment** .      |
|**isSyncDeferred** |Логическое | Указывает, будет ли синхронизация родительской сущности откладывается на более позднюю дату. |
| **allowDisplayNameUpdate** | Логическое |  Указывает, является ли отображаемое имя ресурса может быть перезаписана при синхронизации.         |


## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
