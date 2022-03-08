---
title: accessReviewHistoryScheduleSettings
description: В обзорах доступа Azure AD accessReviewHistoryScheduleSettings представляет параметры, связанные с серией определений истории обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32c8eff3229b0597a5dc05cfeffa66fe8ed2d851
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337881"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>accessReviewHistoryScheduleSettings

Пространство имен: microsoft.graph

Определяет параметры объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Подробные параметры для повторения с помощью стандартного объекта Outlook повторения. <br/><br/>**Примечание:** **Поддерживаются только свойства dayOfMonth**, **интервал** и **тип** (`weekly`, `absoluteMonthly`). Используйте свойство **startDate на** **recurrenceRange** , чтобы определить день начала проверки. Обязательный элемент. |
|reportRange|String|Строка продолжительности в формате isO 8601, указывав период ожидания созданных данных истории обзоров. Например, если определение истории планируется выполнить 1-го каждого месяца, **reportRange** — это `P1M`. В этом случае в первой части каждого месяца будут собираться данные истории обзоров доступа, содержащие только данные обзоров предыдущего месяца. <br/><br/>**Примечание:** **Поддерживаются** **только свойства** **ISO** 8601, которые поддерживаются только годами, месяцами и днями. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryScheduleSettings",
  "reportRange": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```
