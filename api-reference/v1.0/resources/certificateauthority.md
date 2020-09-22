---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 17ec5cc3c17cb4acf8e530bc4c1225ab4061b7f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037922"
---
# <a name="certificateauthority-resource-type"></a>Тип ресурса Цертификатеаусорити

Пространство имен: microsoft.graph

Представляет центр сертификации.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательно. Строка в кодировке Base64, представляющая общедоступный сертификат.|
|цертификатеревокатионлистурл|String|URL-адрес списка отзыва сертификатов.|
|делтацертификатеревокатионлистурл|String|URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.|
|исрутаусорити|Boolean|Обязательно. **true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.|
|имени|String|Поставщик сертификата, рассчитанный на основе значения **сертификата** . Только для чтения. |
|иссуерски|String|Идентификатор ключа субъекта сертификата, рассчитанный на основе значения **сертификата** . Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
