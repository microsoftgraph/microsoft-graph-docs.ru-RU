---
title: Тип ресурса settingTemplateValue
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если этот параметр не создается.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 15110b88b62352476619501c50457a5bd1db5a89
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131630"
---
# <a name="settingtemplatevalue-resource-type"></a>Тип ресурса settingTemplateValue

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если этот параметр не создается.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultValue|string|Значение по умолчанию для параметра. Только для чтения.|
|description|string|Описание параметра. Только для чтения.|
|name|string|Имя параметра. Только для чтения.|
|type|string|Тип параметра. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


