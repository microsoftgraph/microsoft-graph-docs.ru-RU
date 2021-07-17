---
title: тип ресурса publicErrorDetail
description: Представляет сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac86f2aa50e1447702099f3c73f31979b6e6eb16
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467525"
---
# <a name="publicerrordetail-resource-type"></a>тип ресурса publicErrorDetail

Пространство имен: microsoft.graph

Представляет сведения о [publicError](../resources/publicerror.md) или [publicInnerError](../resources/publicinnererror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код ошибки.|
|message|String|Сообщение об ошибке.|
|target|String|Целевое значение ошибки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```
