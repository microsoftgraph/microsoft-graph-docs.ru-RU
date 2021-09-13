---
title: параметрTemplateValue типа ресурса
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 307161ccb879985942f0973b29fc4cbc370c230c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126655"
---
# <a name="settingtemplatevalue-resource-type"></a>параметрTemplateValue типа ресурса

Пространство имен: microsoft.graph

Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|defaultValue|String| Значение по умолчанию для параметра. |
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

