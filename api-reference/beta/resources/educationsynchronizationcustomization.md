---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9294af5796daeefb394ed1625a9a36128ae7b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860902"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса educationSynchronizationCustomization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. 

>**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
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
