---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535415"
---
#  <a name="certificationcontrol-resource-type"></a>Тип ресурса Цертификатионконтрол

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
