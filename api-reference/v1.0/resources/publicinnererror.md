---
title: тип ресурса publicInnerError
description: Представляет внутренние сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f089c120ac4ba1307f0b0ffa2f08f8578613eaa1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467522"
---
# <a name="publicinnererror-resource-type"></a>тип ресурса publicInnerError

Пространство имен: microsoft.graph

Представляет внутренние сведения [publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код ошибки.|
|подробности|[коллекция publicErrorDetail](../resources/publicerrordetail.md)|Коллекция сведений об ошибках.|
|message|String|Сообщение об ошибке.|
|target|String|Целевое значение ошибки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```
