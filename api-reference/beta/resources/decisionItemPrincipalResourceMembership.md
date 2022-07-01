---
title: Тип ресурса decisionItemPrincipalResourceMembership
description: Каждое решение в проверке доступа представляет доступ субъекта к ресурсу. Объект decisionItemPrincipalResourceMembership предоставляет сведения о типе членства субъекта ресурсу, связанному с объектом accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9ff76ae47d8289827b9c6309288272d3b9c1e6c1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447786"
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
