---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 201f0c0ac11a0e26174661aa4d8a63baf23f7f3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024572"
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





