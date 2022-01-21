---
title: тип ресурса userLastSignInRecommendationInsightSetting
description: В обзорах доступа к Azure AD пользовательLastSignInRecommendationInsightSetting представляет параметры, связанные с представлением, которое основано на последней дате и времени регистрации пользователя и используется для оказания помощи рецензентам в принятии решений.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa1467ee59bbedd4765e2a64c22009e713a7e71a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137288"
---
# <a name="userlastsigninrecommendationinsightsetting-resource-type"></a>userlastsignInrecommendationinsightsetting resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**UserLastSignInRecommendationInsightSetting** позволяет настроить дату и время последнего входного пользователя в качестве понимания, чтобы помочь рецензентам принимать решения для [объекта accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Наследует [от accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md).

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| recommendationLookBackDuration | Длительность | Необязательное свойство. Указывает период времени бездействия (в отношении даты начала экземпляра обзора), из чего будут настроены рекомендации. Рекомендация будет в том `deny` случае, если пользователь неактивно во время периода обратного действия. Для обзоров групп и ролей Azure AD принимается любая продолжительность. Для отзывов приложений максимальная продолжительность — 30 дней. Если не указано, продолжительность — 30 дней. |
| signInScope | userSignInRecommendationScope | Указывает, рассчитывается ли неактивность на основе бездействия пользователя в клиенте или в приложении. Возможные значения `tenant` , `application` `unknownFutureValue` . `application` имеет значение только в том случае, если обзор доступа является отзывом о назначении приложению. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userLastSignInRecommendationInsightSetting",
  "baseType": "microsoft.graph.accessReviewRecommendationInsightSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userlastsignInrecommendationinsightsetting",
  "recommendationLookBackDuration": "Duration",
  "signInScope": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "userlastsignInrecommendationinsightsetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
