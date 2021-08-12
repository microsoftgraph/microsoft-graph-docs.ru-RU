---
title: тип ресурса publicError
description: Представляет общую ошибку и ее сведения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: f378862ccd77b1a205e1997d7a5c31244717f728d60b9d8d6b505646db116a06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138355"
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
