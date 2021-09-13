---
title: тип ресурса publicInnerError
description: Представляет внутренние сведения об ошибке.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c0189ee65de82edc87f1c9637351409241c00ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143820"
---
# <a name="publicinnererror-resource-type"></a>тип ресурса publicInnerError

Пространство имен: microsoft.graph

Представляет внутренние сведения [publicError](../resources/publicerrordetail.md). 
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код ошибки.|
|details|[коллекция publicErrorDetail](../resources/publicerrordetail.md)|Коллекция сведений об ошибках.|
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
