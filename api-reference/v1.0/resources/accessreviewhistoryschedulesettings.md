---
title: Тип ресурса accessReviewHistoryScheduleSettings
description: В Azure AD проверки доступа accessReviewHistoryScheduleSettings представляет параметры, связанные с рядом определений журнала проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 70483c049a555bf2315a8f0cb49bd652893bef91
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696520"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>Тип ресурса accessReviewHistoryScheduleSettings

Пространство имен: microsoft.graph

Определяет параметры объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Подробные параметры повторения с использованием стандартного объекта повторения Outlook. <br/><br/>**Примечание:** **Поддерживаются только свойства dayOfMonth**, **interval** и **type** (`weekly`, `absoluteMonthly`). Используйте свойство **startDate для** **recurrenceRange** , чтобы определить день начала проверки. Обязательный элемент. |
|reportRange|String|Строка длительности в формате ISO 8601, указывав период просмотра созданных данных журнала проверки. Например, если определение журнала запланировано на 1-е время каждого месяца, **reportRange** будет равно `P1M`. В этом случае в первый раз каждый месяц будут собираться данные журнала проверки доступа, содержащие только данные о проверке за предыдущий месяц. <br/><br/>**Примечание:** **Поддерживаются** только **свойства** **ISO** 8601 только для лет, месяцев и дней. Обязательный элемент.|

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
