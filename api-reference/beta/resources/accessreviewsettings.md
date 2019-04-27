---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348424"
---
# <a name="accessreviewsettings-resource-type"></a>Тип ресурса Акцессревиевсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| Маилнотификатионсенаблед | boolean |  |
| Реминдерсенаблед | boolean |  |
| Жустификатионрекуиредонаппровал | boolean |  |
| Рекурренцесеттингс | Акцессревиеврекурренцесеттингс |  |
| Ауторевиевенаблед | boolean |  |
| Активитидуратиониндайс | Int32 |  |
| Ауторевиевсеттингс | Ауторевиевсеттингс |  |
| Аутоапплиревиевресултсенаблед | boolean |  |
| Акцессрекоммендатионсенаблед | boolean |  |


## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



