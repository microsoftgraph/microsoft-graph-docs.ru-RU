---
title: Тип ресурса Ауторевиевсеттингс
description: Указывает поведение при завершении проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b9d0a621c4229476e0b3bcdadb869e44422e931
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330333"
---
# <a name="autoreviewsettings-resource-type"></a>Тип ресурса Ауторевиевсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса **ауторевиевсеттингс** используется в ресурсе [акцессревиевсеттингс](accessreviewsettings.md) и определяет поведение при завершении проверки доступа.    

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| нотревиеведресулт | Строка | Возможные значения: `Approve` , `Deny` , или `Recommendation` .  В `Recommendation` этом случае для **акцессрекоммендатионсенаблед** в ресурсе **акцессревиевсеттингс** также должно быть задано значение `true` . Если вы хотите, чтобы система предоставляла решение, даже если проверяющий не сделает выбор, установите свойство **ауторевиевенаблед** в ресурсе **акцессревиевсеттингс** в `true` и включите объект **ауторевиевсеттингс** со свойством **нотревиеведресулт** . После завершения анализа на основе свойства **нотревиеведресулт** решение записывается как `Approve` или `Deny` .|

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