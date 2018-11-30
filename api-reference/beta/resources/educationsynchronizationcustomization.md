---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
ms.openlocfilehash: 51799e01e5ab48fc5e686d72d2bdb5c85f191e1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075898"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса educationSynchronizationCustomization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. 

>**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:-|:-|:-|
| **optionalPropertiesToSync** | Набор типа string |  Коллекция имен свойств для синхронизации. Если задано значение null, все свойства будут синхронизированы.       |
| **synchronizationStartDate** | DateTime |  Дата начала для синхронизации. Это значение необходимо задать в будущем. Если параметр имеет значение null, ресурс будет синхронизирован после завершения настройки профиля. **Примечание:** Применяется только к свойству **StudentEnrollment** .      |
|**isSyncDeferred** |Логический | Указывает, будет ли синхронизация родительской сущности откладывается на более позднюю дату. |
| **allowDisplayNameUpdate** | Логический |  Указывает, является ли отображаемое имя ресурса может быть перезаписана при синхронизации.         |


## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
