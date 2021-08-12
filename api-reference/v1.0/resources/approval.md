---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b2917825104d30813f6ad98237dd68492e4a269481d1013458edb1038208430c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212223"
---
# <a name="approval-resource-type"></a>Тип ресурса утверждения

Пространство имен: microsoft.graph

Представляет объект утверждения для решений, связанных с запросом.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор решения об утверждении.|
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
