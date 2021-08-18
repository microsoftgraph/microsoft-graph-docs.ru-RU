---
title: тип ресурса publicInnerError
description: Представляет внутренние сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d0d14ffb803a084db080dc986ceb0dc83f14619dd3230b68aacf07401f13543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139118"
---
# <a name="publicinnererror-resource-type"></a>тип ресурса publicInnerError

Пространство имен: microsoft.graph

Представляет внутренние сведения [publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|Строка|Код ошибки.|
|details|[коллекция publicErrorDetail](../resources/publicerrordetail.md)|Коллекция сведений об ошибках.|
|message|String|Сообщение об ошибке.|
|target|Строка|Целевое значение ошибки.|

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

