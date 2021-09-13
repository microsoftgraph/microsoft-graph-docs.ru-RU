---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с userConsentRequest.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f59736f7cdb4aed235eeb1fa5831e69024057d11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067614"
---
# <a name="approval-resource-type"></a>Тип ресурса утверждения

Пространство имен: microsoft.graph

Представляет объект утверждения для решений, связанных с запросом.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор решения об утверждении.|
|stages|[коллекция approvalStage](../resources/approvalstage.md)|Набор этапов в решении об утверждении. |

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|stages|[коллекция approvalStage](../resources/approvalstage.md)|Набор этапов в решении об утверждении. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
