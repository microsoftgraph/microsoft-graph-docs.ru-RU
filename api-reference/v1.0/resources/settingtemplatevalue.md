---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c39762290577c6279a4ecb52bd832ac9c961dbdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009200"
---
# <a name="settingtemplatevalue-resource-type"></a>Тип ресурса Сеттингтемплатевалуе

Пространство имен: microsoft.graph

Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|Значение|String| Значение по умолчанию для параметра. |
|description|String| Описание параметра. |
|name|String| Имя параметра. |
|type|String| Тип параметра. |

### <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

