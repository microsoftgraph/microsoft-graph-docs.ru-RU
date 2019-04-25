---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543205"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатионс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.

> **Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .

Этот ресурс является членом следующих поставщиков данных:

* [Едукатионксвдатапровидер](educationcsvdataprovider.md)
* [Едукатионповерсчулдатапровидер](educationpowerschooldataprovider.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Название** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для учебного объекта School.        |
| **section** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта Section.         |
| **student** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта Student.         |
| **teacher** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта учителя.         |
| **Студентенроллмент** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка регистрации для учащихся.           |
| **Теачерростер** | [Едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |       Настройка для списка преподавателей.    |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
