---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87d439a15f9668931f0488e065cde5beef87ab2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042704"
---
# <a name="certificateauthority-resource-type"></a>Тип ресурса Цертификатеаусорити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет центр сертификации.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательный. Строка в кодировке Base64, представляющая общедоступный сертификат.|
|цертификатеревокатионлистурл|Строка|URL-адрес списка отзыва сертификатов.|
|делтацертификатеревокатионлистурл|Строка|URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.|
|исрутаусорити|Boolean|Обязательный. **true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.|
|имени|Строка|Поставщик сертификата, рассчитанный на основе значения **сертификата** . Только для чтения. |
|иссуерски|Строка|Идентификатор ключа субъекта сертификата, рассчитанный на основе значения **сертификата** . Только для чтения.|

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

