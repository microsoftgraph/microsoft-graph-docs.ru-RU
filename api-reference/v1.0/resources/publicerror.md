---
title: тип ресурса publicError
description: Представляет общую ошибку и ее сведения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 4aa4f336ab2b5404e2e82d26f7c38a9ed9b239d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044295"
---
# <a name="publicerror-resource-type"></a>тип ресурса publicError

Пространство имен: microsoft.graph

Представляет общую ошибку и ее сведения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|string| Представляет код ошибки.
|details|[коллекция publicErrorDetail](publicerrordetail.md)|Сведения об ошибке.|
|innerError|[publicInnerError](publicinnererror.md)|Сведения о внутренней ошибке.|
|message|string| Не локализованное сообщение для разработчика.
|target|String|Целевое значение ошибки.|

## <a name="relationships"></a>Отношения
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
