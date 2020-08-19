---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f6ecfa2ffddd362ba6c166d9dc839aedaf6f4723
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810582"
---
#  <a name="certificationcontrol-resource-type"></a>Тип ресурса Цертификатионконтрол

Пространство имен: microsoft.graph

Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.

|Свойство |Тип |Описание |
|:--|:--|:--|
|name | string | Имя элемента управления сертификацией |
|url | string | URL-адрес портала доверия службы Майкрософт |

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
