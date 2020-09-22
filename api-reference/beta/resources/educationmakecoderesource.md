---
title: Тип ресурса Едукатионмакекодересаурце
description: Ресурс Макекоде
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 49e0a563a190056159c8c910cc46398a6adee41d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076451"
---
# <a name="educationmakecoderesource-resource-type"></a>Тип ресурса Едукатионмакекодересаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, представляющий проект [макекоде](https://www.microsoft.com/en-us/makecode) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|projectId|String|ИДЕНТИФИКАТОР проекта Макекоде|
|хоствебурл|String|Узел для типа ресурса Макекоде (например, аркаде, Микробит)|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "projectId": "String",
  "hostWebUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

