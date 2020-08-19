---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a2046017dec6439c6db35169de15eb6bb49413b1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806739"
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

### <a name="json-representation"></a>Представление в формате JSON

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
