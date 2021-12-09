---
title: тип ресурса cloudPcLoginResult
description: Представляет сведения о том, как облачный КОМПЬЮТЕР вздыхает в результатах.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b0ab1d22d5eabeaed84e8ee0d15f9527d64387e7
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391179"
---
# <a name="cloudpcloginresult-resource-type"></a>тип ресурса cloudPcLoginResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о том, как облачный КОМПЬЮТЕР вздыхает в результатах.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|time|DateTimeOffSet|Время, когда облачный КОМПЬЮТЕР вздыхает в действии. Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'. Только для чтения.|

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
