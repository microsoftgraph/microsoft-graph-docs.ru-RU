---
title: Тип ресурса accessReviewScheduleSettings
description: Представляет параметры, связанные с рядом проверок доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb647faa01fe5dcc296f18c9dcc1ad00957c2253
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698438"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| mailNotificationsEnabled|Логический | Указывает, включены или отключены сообщения электронной почты. Значение по умолчанию — `false`.               |
| reminderNotificationsEnabled|Логический  | Указывает, включены или отключены напоминания. Значение по умолчанию — `false`.  |
| justificationRequiredOnApproval|Логический | Указывает, требуются ли рецензенты для предоставления обоснования своего решения. Значение по умолчанию — `false`. |
| defaultDecisionEnabled|Логический | Указывает, включено ли решение по умолчанию, если рецензенты не отвечают. Значение по умолчанию — `false`. |
| defaultDecision|Строка | Выбранное решение, **если defaultDecisionEnabled** имеет значение `true`. Может быть одним из `Approve`, `Deny`или `Recommendation`. |
| instanceDurationInDays|Int32 | Длительность каждого повторения проверки (**accessReviewInstance**) в днях. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры повторения с использованием стандартного объекта повторения Outlook.  <br/><br/>**Примечание:** **Поддерживаются только свойства dayOfMonth**, **interval** и **type** (`weekly`, `absoluteMonthly`). Используйте свойство **startDate для** **recurrenceRange** , чтобы определить день начала проверки. |
| autoApplyDecisionsEnabled|Логическое | Указывает, применяются ли решения автоматически. Если задано значение `false`,администратор должен применить решения вручную после завершения проверки доступа рецензентом. Если задано значение `true`,решения применяются автоматически по истечении срока действия экземпляра проверки доступа независимо от того, ответили ли рецензенты. Значение по умолчанию — `false`. |
| applyActions|[Коллекция accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживаются два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction`. Поле необходимо указать только в случае с `disableAndDeleteUserApplyAction`. |
| recommendationsEnabled|Логическое | Указывает, включены или отключены рекомендации по принятию решений. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```
