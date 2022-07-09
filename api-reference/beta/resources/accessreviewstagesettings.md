---
title: Тип ресурса accessReviewStageSettings
description: В Azure AD проверки доступа accessReviewStageSettings представляет параметры этапов, связанных с многоэтабной проверкой доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8a7e0142f7f97f608544bc4ca4fc56ab4d3f11dd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697836"
---
# <a name="accessreviewstagesettings-resource-type"></a>Тип ресурса accessReviewStageSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет параметры этапов, связанных с объектом [проверки многоэтабного](accessreviewscheduledefinition.md) доступа. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|decisionsThatWillMoveToNextStage|Коллекция объектов string|Укажите, какие решения будут приняты на следующем этапе. Может быть подмноженым набором `Approve`, или `NotReviewed``Deny``Recommendation`. Если этот параметр не указан, все решения будут переходить к следующему этапу. Необязательное. |
|dependsOn|Коллекция String| Определяет последовательный или параллельный порядок этапов и зависит от **stageId**. В настоящее время поддерживаются только последовательные этапы. Например, если **stageId** имеет значение `2`, **то dependsOn должен** иметь значение .`1` Если **stageId** имеет значение `1`stageId, не указывайте **dependsOn**. Требуется, если **stageId** не является `1`. |
|durationInDays|Int32|Длительность этапа. Обязательный элемент.  <br/><br/>**ПРИМЕЧАНИЕ:** Совокупное значение этого свойства на всех этапах <br/> 1. Переопределяет параметр [instanceDurationInDays](accessReviewScheduleSettings.md) для [объекта accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) . <br/>2. Не может превышать длину одного повторения. То есть, если проверка выполняется еженедельно, совокупная **длительностьInDays** не может превышать 7. |
|fallbackReviewers|[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Если этот параметр указан, резервным рецензентам предлагается выполнить проверку, если основные рецензенты не существуют. Например, если руководители выбраны в качестве рецензентов, а проверяемая субъект не имеет руководителя в Azure AD, резервным рецензентам будет предложено проверить этот субъект. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр объекта [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) .|
|recommendationsEnabled|Логическое|Указывает, включены ли рекомендации для рецензентов. Обязательный элемент. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).[](accessReviewScheduleSettings.md)|
| recommendationInsightsSettings | [Коллекция accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) | Определяет, какие рекомендации следует отображать рецензентам. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий [параметр объекта](accessReviewScheduleSettings.md) [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationLookBackDuration | Длительность| Необязательное поле. Указывает период бездействия (в отношении даты начала экземпляра проверки), из которого будут настроены рекомендации. Рекомендация будет применяться, `deny` если пользователь неактивен в течение периода обратного просмотра. Для проверок групп и Azure AD ролей принимается любая длительность. Для проверок приложений максимальная длительность составляет 30 дней. Если не указано, длительность составляет 30 дней. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий [параметр объекта](accessReviewScheduleSettings.md) [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . |
|Авторам|[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Определяет, кто является рецензентом. Если они не указаны, проверка выполняется самостоятельно (пользователи проверяют собственный доступ).  Примеры параметров назначения рецензентов см. в статье "Назначение рецензентов определению проверки доступа с [помощью microsoft API Graph"](/graph/accessreviews-reviewers-concept). <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства переопределит соответствующий параметр в [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md). |
|stageId|Строка|Уникальный идентификатор **объекта accessReviewStageSettings**. **StageId будет** использоваться в **свойстве dependsOn**, чтобы указать связь стадии. Обязательный элемент. |

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

