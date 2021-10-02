---
title: тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностями для синхронизации и их настроек, если таковые есть.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 30792f67b04606235a99e131d58ffb72bebe8ebd
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068589"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>тип ресурса educationSynchronizationCustomizations

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит список сущностями для синхронизации и их настроек, если таковые есть.

> [!NOTE]
> Настройка свойств для синхронизации не применяется к реестрам учащихся или реестрам преподавателей.

Этот ресурс является членом следующих поставщиков данных:

- [educationCsvDataProvider](educationcsvdataprovider.md)
- [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Свойства

| Свойство          | Тип                                    | Описание                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| школа            | [educationSynchronizationCustomization] | Настройка для сущностями школы.     |
| section           | [educationSynchronizationCustomization] | Настройка для сущностями Раздела.    |
| student           | [educationSynchronizationCustomization] | Настройки для сущностями учащихся.    |
| teacher           | [educationSynchronizationCustomization] | Настройка для сущностями Teacher.    |
| studentEnrollment | [educationSynchronizationCustomization] | Настройки для регистрации учащихся. |
| teacherRoster     | [educationSynchronizationCustomization] | Настройки для реестров учителей.     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  }
}
```


