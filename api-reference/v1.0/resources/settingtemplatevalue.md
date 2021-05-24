---
title: параметрTemplateValue типа ресурса
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547052"
---
# <a name="settingtemplatevalue-resource-type"></a>параметрTemplateValue типа ресурса

Пространство имен: microsoft.graph

Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|defaultValue|Строка| Значение по умолчанию для параметра. |
|description|Строка| Описание параметра. |
|name|String| Имя параметра. |
|type|Строка| Тип параметра. |

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

