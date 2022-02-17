---
title: тип ресурса resultTemplate
description: Представляет словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f6c3583ce13da2bc1c94325ed4a7db7353f329f0
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879293"
---
# <a name="resulttemplate-resource-type"></a>тип ресурса resultTemplate

Пространство имен: microsoft.graph

Представляет словарь **resultTemplateIds** и связанных с ними значений, который включает имя и схему JSON шаблонов результатов.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|body|Json|Схема шаблона результатов JSON.|
|displayName|Строка|Имя шаблона результатов.|
|ключа|Строка|ID шаблона результатов. Свойство **ключа** должно сопопозить **с resultTemplateId** в [коллекции searchHit](searchhit.md) .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
  "resultTemplateId": {
                        "displayName": "String",
                        "body": {"@odata.type": "microsoft.graph.Json"}
                      }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


