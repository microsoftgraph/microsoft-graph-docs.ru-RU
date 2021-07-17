---
title: тип ресурса publicError
description: Представляет общую ошибку и ее сведения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: e9f5decf8edc2ebf3e11d00eb89e68236a6a73d4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467531"
---
# <a name="publicerror-resource-type"></a>тип ресурса publicError

Пространство имен: microsoft.graph

Представляет общую ошибку и ее сведения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|string| Представляет код ошибки.
|подробности|[коллекция publicErrorDetail](publicerrordetail.md)|Сведения об ошибке.|
|innerError|[publicInnerError](publicinnererror.md)|Сведения о внутренней ошибке.|
|message|string| Не локализованное сообщение для разработчика.
|target|String|Целевое значение ошибки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```
