---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0d1a886557e37bb19b23c5e0c1d74b937112cc58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334119"
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
