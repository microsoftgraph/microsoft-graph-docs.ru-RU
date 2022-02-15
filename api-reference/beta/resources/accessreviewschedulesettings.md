---
title: тип ресурса accessReviewScheduleSettings
description: В функции обзоров доступа Azure AD представлены параметры, `accessReviewScheduleSettings` связанные с серией обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb7dbc40944d42f50b68b82cf2be8a2499020f8a
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816058"
---
# <a name="accessreviewschedulesettings-resource-type"></a>тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Логический | Указывает, включена ли электронная почта или отключена. Значение по умолчанию — `false`.               |
| reminderNotificationsEnabled|Логический  | Указывает, включены или отключены напоминания. Значение по умолчанию — `false`.  |
| justificationRequiredOnApproval|Логический | Указывает, требуются ли рецензенты для обоснования своего решения. Значение по умолчанию — `false`. |
| defaultDecisionEnabled|Логический | Указывает, включено или отключено решение по умолчанию, если рецензенты не отвечают. Значение по умолчанию — `false`. |
| defaultDecision|Строка | Решение, выбранное, если `defaultDecisionEnabled` включено. Может быть одним из `Approve`, или `Deny``Recommendation`. |
| instanceDurationInDays|Int32 | Продолжительность каждого повторения обзора (`accessReviewInstance`) в количестве дней. <br/>**ПРИМЕЧАНИЕ:** Если **определены этапыSettings** объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , вместо значения этого свойства будет использоваться параметр **durationInDays** . |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры для повторения с помощью стандартного объекта Outlook повторения. <br/><br/>**Примечание:** **Поддерживаются только свойства dayOfMonth**, **интервал** и **тип** (`weekly`, `absoluteMonthly`). Используйте свойство **startDate на** **recurrenceRange** , чтобы определить день начала проверки. |
| autoApplyDecisionsEnabled|Boolean | Указывает, применяются ли решения автоматически. Если установлено `false`, администратор должен применять решения вручную, как только рецензент завершит обзор доступа. При наборе `true`решения применяются автоматически после окончания срока действия экземпляра проверки доступа независимо от того, откликнулись ли рецензенты. Значение по умолчанию — `false`. |
| applyActions|[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction`. Поле должно быть указано только в случае `disableAndDeleteUserApplyAction`. |
| recommendationsEnabled|Логический | Указывает, включены или отключены рекомендации по принятию решений. <br/>**ПРИМЕЧАНИЕ:** Если **определены этапыSettings** объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , вместо значения этого свойства будут использоваться его параметр **recommendationsEnabled** . |
| recommendationLookBackDuration | Длительность| Необязательное поле. Указывает период бездействия (в отношении даты начала экземпляра проверки), из чего будут настроены рекомендации. Рекомендация будет в том `deny` случае, если пользователь неактивно во время периода обратного действия. Для обзоров групп и ролей Azure AD принимается любая продолжительность. Для отзывов приложений максимальная продолжительность — 30 дней. Если не указано, продолжительность — 30 дней. <br/><br/>**ПРИМЕЧАНИЕ:** Если **определены этапыSettings** объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , вместо значения этого свойства будет использоваться его параметр **recommendationLookBackDuration** . |
|decisionHistoriesForReviewersEnabled|Boolean| Указывает, доступны ли решения на предыдущих этапах проверки доступа для рецензентов на **accessReviewInstance** с несколькими последующими этапами. Если не предоставлено, по умолчанию отключено (`false`).|
| recommendationInsightSettings|[accessReviewRecommendationInsightSetting](../resources/accessReviewRecommendationInsightSetting.md) collection | Необязательное свойство. Описывает типы анализов, которые проверяют для принятия решений по обзору доступа. <br/><br/>**ПРИМЕЧАНИЕ:** Если определены **этапыSettings** объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , вместо значения этого свойства будет использоваться параметр **recommendationInsightSettings** . |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "Duration",
  "decisionHistoriesForReviewersEnabled": "Boolean",
  "recommendationInsightSettings": [
    {
      "@odata.type": "microsoft.graph.accessReviewRecommendationInsightSetting"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
