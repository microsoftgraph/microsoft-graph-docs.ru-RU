---
title: тип ресурса publicErrorDetail
description: Представляет сведения об ошибке.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3965fd862fee8e4e571055bdc37ade80909c9e97
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104070"
---
# <a name="publicerrordetail-resource-type"></a>тип ресурса publicErrorDetail

Пространство имен: microsoft.graph

Представляет сведения о [publicError](../resources/publicerror.md) или [publicInnerError](../resources/publicinnererror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код ошибки.|
|message|String|Сообщение об ошибке.|
|target|Строка|Целевое значение ошибки.|

## <a name="relationships"></a>Отношения
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
