---
title: Тип ресурса educationSynchronizationCustomizations
description: Содержит список сущностей для синхронизации и их настройки, при их наличии.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 3254915887afc1e6b0da0b3b6c44b59689219ab1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918191"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>Тип ресурса educationSynchronizationCustomizations

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит список сущностей для синхронизации и их [настройки](educationsynchronizationcustomization.md), при их наличии.

> **Примечание:** Настройка свойств для синхронизации не применяется к **studentEnrollment** и **teacherRoster** сущности.

Этот ресурс, принадлежит следующие поставщики данных:

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **School** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Настройка для сущности school.        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Настройка раздела сущности.         |
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Настройка для учащихся сущности.         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Настройка для преподавателей сущности.         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Настройка для регистрации учащихся.           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       Настройка для преподавателей участников.    |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
