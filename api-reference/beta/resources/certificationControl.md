---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bafd2c9d66c0d696649944f88e4fcfbdea4bcca6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507763"
---
#  <a name="certificationcontrol-resource-type"></a>Тип ресурса Цертификатионконтрол

Пространство имен: microsoft.graph

Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.

|Свойство |Тип |Описание |
|:--|:--|:--|
|name | string | Имя элемента управления сертификацией |
|url | string | URL-адрес портала доверия службы Майкрософт |

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
