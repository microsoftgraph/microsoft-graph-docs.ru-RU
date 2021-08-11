---
title: параметрTemplateValue типа ресурса
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f83eab2fb8cd0368338813f8a4c63309d43070a5e33f7e41aa2882d0e2308bbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54228992"
---
# <a name="settingtemplatevalue-resource-type"></a>параметрTemplateValue типа ресурса

Пространство имен: microsoft.graph

Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|defaultValue|String| Значение по умолчанию для параметра. |
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

