---
title: " Тип ресурса certificationControl"
description: Этот ресурс содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810390"
---
#  <a name="certificationcontrol-resource-type"></a>Тип ресурса certificationControl

Содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.

|Свойство |Тип |Описание |
|:--|:--|:--|
|name | строка | Имя элемента управления сертификации |
|url | строка | URL-адрес для службы Microsoft доверять портала |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
