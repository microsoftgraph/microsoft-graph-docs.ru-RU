---
title: тип ресурса resultTemplate
description: Представляет словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3951c86846966d12292bad242ebb1545f80b1b7c
ms.sourcegitcommit: 7deb4fad6acc69fd6bc02cd4e2f6774de5784c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2022
ms.locfileid: "62894791"
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
      "body":{
         "@odata.type":"microsoft.graph.Json"
      }
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


