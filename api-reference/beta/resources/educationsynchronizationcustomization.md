---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
author: mmast-msft
ms.openlocfilehash: d4f67c9f56198350731c18fe3da8b512522c4d71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350638"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса educationSynchronizationCustomization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. 

>**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **optionalPropertiesToSync** | Набор типа string |  Коллекция имен свойств для синхронизации. Если задано значение null, все свойства будут синхронизированы.       |
| **synchronizationStartDate** | DateTime. |  Дата начала для синхронизации. Это значение необходимо задать в будущем. Если параметр имеет значение null, ресурс будет синхронизирован после завершения настройки профиля. **Примечание:** Применяется только к свойству **StudentEnrollment** .      |
|**isSyncDeferred** |Boolean. | Указывает, будет ли синхронизация родительской сущности откладывается на более позднюю дату. |
| **allowDisplayNameUpdate** | Boolean. |  Указывает, является ли отображаемое имя ресурса может быть перезаписана при синхронизации.         |


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
