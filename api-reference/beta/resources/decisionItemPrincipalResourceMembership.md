---
title: Тип ресурса decisionItemPrincipalResourceMembership
description: Каждое решение в проверке доступа представляет доступ субъекта к ресурсу. Объект decisionItemPrincipalResourceMembership предоставляет сведения о типе членства субъекта ресурсу, связанному с объектом accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eed87ba5ad700330c1c2449060e9397c8eb6408c
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698263"
---
# <a name="decisionitemprincipalresourcemembership-resource-type"></a>Тип ресурса decisionItemPrincipalResourceMembership

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Каждое решение в проверке доступа представляет доступ субъекта к ресурсу. Объект **decisionItemPrincipalResourceMembership** предоставляет сведения о типе членства субъекта ресурсу, связанному с объектом [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . Например, субъект может иметь прямой или косвенный доступ к ресурсу.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|membershipType| decisionItemPrincipalResourceMembershipType | Тип членства, которое субъект имеет к ресурсу. Многозначные значения. Допустимые значения: `direct`, `indirect`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.decisionItemPrincipalResourceMembership",
  "membershipType": "String",
}
```
