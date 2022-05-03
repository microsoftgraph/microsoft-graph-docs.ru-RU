---
title: Тип ресурса printCertificateSigningRequest
description: Запрос подписи сертификата (CSR), используемый во время регистрации принтера в службе универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 466782f93ef6de645f8a1b90085e7a96538f1cba
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176916"
---
# <a name="printcertificatesigningrequest-resource-type"></a>Тип ресурса printCertificateSigningRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запрос подписи сертификата (CSR), используемый во время регистрации принтера в службе универсальной печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Запрос сертификата pkcs10 в кодировке Base64. Только для чтения.|
|transportKey|Строка|Общедоступная часть асимметричного ключа в кодировке Base64, создаваемая клиентом. Только для чтения.|

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


