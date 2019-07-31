---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972441"
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
