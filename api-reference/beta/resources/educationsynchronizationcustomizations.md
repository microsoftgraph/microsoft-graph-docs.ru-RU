---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d3bfbec774b0ce5ff749e78b0057799501f432c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055598"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит список сущностей для синхронизации и их настройки, если они есть.

> [!NOTE]
> Настройка свойств для синхронизации не относится к регистрационным спискам студентов или преподавателям.

Этот ресурс является членом следующих поставщиков данных:

- [едукатионксвдатапровидер](educationcsvdataprovider.md)
- [едукатионповерсчулдатапровидер](educationpowerschooldataprovider.md)

## <a name="properties"></a>Свойства

| Свойство          | Тип                                    | Описание                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| Название            | [едукатионсинчронизатионкустомизатион] | Настройки для учебных заведений.     |
| section           | [едукатионсинчронизатионкустомизатион] | Настройки для сущностей раздела.    |
| student           | [едукатионсинчронизатионкустомизатион] | Настройки для сущностей учащихся.    |
| teacher           | [едукатионсинчронизатионкустомизатион] | Настройки для сущностей преподавателей.    |
| студентенроллмент | [едукатионсинчронизатионкустомизатион] | Настройки для регистрации учащихся. |
| теачерростер     | [едукатионсинчронизатионкустомизатион] | Настройки для списков преподавателей.     |

[едукатионсинчронизатионкустомизатион]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```


