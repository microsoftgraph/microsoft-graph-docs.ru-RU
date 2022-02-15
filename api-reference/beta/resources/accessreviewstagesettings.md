---
title: тип ресурса accessReviewStageSettings
description: В обзорах доступа к Azure AD accessReviewStageSettings представляет параметры этапов, связанных с многоэтапным обзором доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: daa7b139aa5a9321965bfe6391c92c16fbc52ffc
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816219"
---
# <a name="accessreviewstagesettings-resource-type"></a>тип ресурса accessReviewStageSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет параметры этапов, связанных с объектом [проверки многоступенчатого доступа](accessreviewscheduledefinition.md) . 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|decisionsThatWillMoveToNextStage|Коллекция String|Указать, какие решения будут приняты на следующем этапе. Может быть подустройка `Approve`, или `Recommendation``Deny``NotReviewed`. Если не предоставлено, все решения будут переходить к следующему этапу. Необязательное свойство. |
|dependsOn|Коллекция строк| Определяет последовательное или параллельное порядок этапов и зависит от **stageId**. В настоящее время поддерживаются только последовательное этапы. Например, если **stageId** является `2`, то **dependsOn** должен быть `1`. Если **stageId** есть `1`, не укажите **dependsOn**. Обязательно, **если stageId** не является `1`. |
|durationInDays|Int32|Продолжительность этапа. Обязательный элемент.  <br/><br/>**ПРИМЕЧАНИЕ:** Совокупное значение этого свойства на всех этапах <br/> 1. Переопределит параметр [instanceDurationInDays](accessReviewScheduleSettings.md) на [объекте accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) . <br/>2. Не может превышать длину одного рецидива. То есть, если обзор повторяется еженедельно, совокупная **продолжительностьInDays** не может превышать 7. |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|При условии, если основные рецензенты не существуют, рецензентам откатов будет предложено завершить проверку. Например, если менеджеры выбраны в качестве рецензентов, а у проверяемого директора нет менеджера в Azure AD, проверятелям откатов будет предложено просмотреть этот принцип. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр объекта [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) .|
|recommendationsEnabled|Логический|Указывает, включено ли отображение рекомендаций рецензентам. Обязательный элемент. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр на [объекте accessReviewScheduleDefinition](accessreviewscheduledefinition.md).[](accessReviewScheduleSettings.md)|
| recommendationInsightsSettings | [accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) collection | Определяет, какие рекомендации показывать рецензентам. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит [соответствующий параметр](accessReviewScheduleSettings.md) объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationLookBackDuration | Длительность| Необязательное поле. Указывает период времени бездействия (в отношении даты начала экземпляра обзора), из чего будут настроены рекомендации. Рекомендация будет в том случае `deny` , если пользователь неактивно во время периода обратного назад. Для обзоров групп и ролей Azure AD принимается любая продолжительность. Для отзывов приложений максимальная продолжительность — 30 дней. Если не указано, продолжительность — 30 дней. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит [соответствующий параметр](accessReviewScheduleSettings.md) объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . |
|рецензенты|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Определяет, кто такие рецензенты. Если нет указаны, обзор является самообнаверяемой (пользователи просматривают собственный доступ).  Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept) <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр [в accessReviewScheduleDefinition](accessReviewScheduleDefinition.md). |
|stageId|Строка|Уникальный идентификатор **accessReviewStageSettings**. **StageId будет** использоваться в **свойстве dependsOn** для указать отношение стадии. Обязательный элемент. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewStageSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStageSettings",
  "stageId": "String",
  "dependsOn": [
    "String"
  ],
  "durationInDays": "Integer",
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "String (duration)",
  "decisionsThatWillMoveToNextStage": [
    "String"
  ],
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

