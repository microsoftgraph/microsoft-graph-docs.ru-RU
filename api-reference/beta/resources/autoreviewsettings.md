---
title: Тип ресурса autoReviewSettings (не рекомендуется)
description: Указывает поведение при завершении проверки доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 593c07266432a389b0f63891675fa9f4823db784
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820261"
---
# <a name="autoreviewsettings-resource-type-deprecated"></a>Тип ресурса autoReviewSettings (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Тип **ресурса autoReviewSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и указывает поведение при завершении проверки доступа.    

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| notReviewedResult | Строка | Возможные значения: `Approve`, или `Deny``Recommendation`.  Если `Recommendation`, **то accessRecommendationsEnabled** в **ресурсе accessReviewSettings** также должен иметь значение `true`. Если вы хотите, чтобы система выдала решение, даже если рецензент не делает выбор, задайте для свойства **autoReviewEnabled** в **ресурсе accessReviewSettings** `true` значение и включите объект **autoReviewSettings** со свойством **notReviewedResult** . Затем по завершении проверки на основе свойства **notReviewedResult** решение записывается как одно `Approve` или как `Deny`.|

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
