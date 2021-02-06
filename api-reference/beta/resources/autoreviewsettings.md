---
title: Тип ресурса autoReviewSettings
description: Указывает поведение, которое будет происходить после завершения проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f46ef4b57a921cc08fbb8f3768597eef12c1ce4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136936"
---
# <a name="autoreviewsettings-resource-type"></a>Тип ресурса autoReviewSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип **ресурса autoReviewSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и определяет поведение после завершения проверки доступа.    

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| notReviewedResult | Строка | Возможные значения: `Approve` , `Deny` , или `Recommendation` .  Если `Recommendation` , **то accessRecommendationsEnabled** в **ресурсе accessReviewSettings** также должен быть установлен в `true` . Если вы хотите, чтобы система предоставила решение, даже если проверяющий не делает выбор, установите свойство **autoReviewEnabled** в **ресурсе accessReviewSettings** и включите объект `true` **autoReviewSettings** со свойством **notReviewedResult.** Затем, когда проверка завершается на основе свойства **notReviewedResult,** решение регистрируются как либо `Approve` либо `Deny` .|

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.autoReviewSettings"
}-->
```json
{
  "notReviewedResult": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "autoReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
