---
title: тип ресурса cloudPcLoginResult
description: Представляет сведения о входе облачного КОМПЬЮТЕРА в результатах.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: f7b083e679939b5d4d478f09ddba6af76a33ac49
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403077"
---
# <a name="cloudpcloginresult-resource-type"></a>тип ресурса cloudPcLoginResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о входе облачного КОМПЬЮТЕРА в результатах.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|time|DateTimeOffSet|Время действия подписи облачного КОМПЬЮТЕРА. Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLoginResult",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLoginResult",
  "time": "String (timestamp)"
}
```
