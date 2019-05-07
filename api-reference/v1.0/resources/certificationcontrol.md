---
title: Тип ресурса Цертификатионконтрол
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629315"
---
#  <a name="certificationcontrol-resource-type"></a>Тип ресурса Цертификатионконтрол

Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|name|String|Имя элемента управления сертификацией |
|url|String|URL-адрес портала доверия службы Майкрософт |

## <a name="json-representation"></a>Представление в формате JSON

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
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
