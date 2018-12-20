---
title: " Тип ресурса certificationControl"
description: Этот ресурс содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380947"
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
