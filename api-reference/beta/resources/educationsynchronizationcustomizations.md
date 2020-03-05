---
title: Тип ресурса Едукатионсинчронизатионкустомизатионс
description: Содержит список сущностей для синхронизации и их настройки, если они есть.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2ff93d6a91d522c5d1140035e278e9832332321
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500452"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатионс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), если они есть.

> **Примечание:** Настройка свойств для синхронизации не применяется к объектам **студентенроллмент** и **теачерростер** .

Этот ресурс является членом следующих поставщиков данных:

* [едукатионксвдатапровидер](educationcsvdataprovider.md)
* [едукатионповерсчулдатапровидер](educationpowerschooldataprovider.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Название** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для учебного объекта School.        |
| **section** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта Section.         |
| **student** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта Student.         |
| **teacher** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка для объекта учителя.         |
| **студентенроллмент** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |  Настройка регистрации для учащихся.           |
| **теачерростер** | [едукатионсинчронизатионкустомизатион](educationsynchronizationcustomization.md) |       Настройка для списка преподавателей.    |

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
