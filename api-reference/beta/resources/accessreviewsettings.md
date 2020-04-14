---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 978b8f80b6a357ffeb2efced005e395787fedabf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457097"
---
# <a name="accessreviewsettings-resource-type"></a>Тип ресурса Акцессревиевсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| маилнотификатионсенаблед | boolean |  |
| реминдерсенаблед | boolean |  |
| жустификатионрекуиредонаппровал | boolean |  |
| рекурренцесеттингс | акцессревиеврекурренцесеттингс |  |
| ауторевиевенаблед | boolean |  |
| активитидуратиониндайс | Int32 |  |
| ауторевиевсеттингс | ауторевиевсеттингс |  |
| аутоапплиревиевресултсенаблед | boolean |  |
| акцессрекоммендатионсенаблед | boolean |  |


## <a name="relationships"></a>Связи
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



