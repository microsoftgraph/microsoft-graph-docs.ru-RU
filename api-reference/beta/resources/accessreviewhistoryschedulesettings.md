---
title: accessReviewHistoryScheduleSettings
description: В обзорах доступа Azure AD accessReviewHistoryScheduleSettings представляет параметры, связанные с серией определений истории обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f1e10372fbd2db23ae70ea413e007993c6f85a0
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226333"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>accessReviewHistoryScheduleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет параметры объекта [accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Подробные параметры для повторения с помощью стандартного объекта Outlook повторения. <br/><br/>**Примечание:** Поддерживаются **только свойства dayOfMonth,** **интервал** и **тип** `weekly` (, ). `absoluteMonthly` Используйте свойство **startDate на** **recurrenceRange,** чтобы определить день начала проверки. Обязательный. |
|reportRange|String|Строка продолжительности в формате isO 8601, указывав период ожидания созданных данных истории обзоров. Например, если определение истории планируется выполнить 1-го каждого месяца, **reportRange** `P1M` — это . В этом случае в первой части каждого месяца будут собираться данные истории обзоров доступа, содержащие только данные обзоров предыдущего месяца. <br/><br/>**Примечание:** **Поддерживаются** **только** свойства **ISO** 8601, которые поддерживаются только годами, месяцами и днями. Обязательный элемент.|

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
