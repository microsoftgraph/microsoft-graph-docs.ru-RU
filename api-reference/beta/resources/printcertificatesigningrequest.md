---
title: Тип ресурса Принтцертификатесигнингрекуест
description: Запрос подписи сертификата (CSR), который будет использоваться при регистрации принтера с помощью универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 48b3921dbd9ec616290922fa232bfbbd47da00df
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007220"
---
# <a name="printcertificatesigningrequest-resource-type"></a>Тип ресурса Принтцертификатесигнингрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запрос подписи сертификата (CSR), который будет использоваться при регистрации принтера с помощью универсальной службы печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Запрос сертификата PKCS10 с кодировкой base64. Только для чтения.|
|транспорткэй|String|Общедоступная часть асимметричного ключа, созданного клиентом в кодировке Base64. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}-->

```json
{
  "content": "String",
  "transportKey": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printCertificateSigningRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
