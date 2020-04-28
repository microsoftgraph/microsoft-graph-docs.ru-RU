---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 25303f527a8ba440e9a1e413379bf8037e551168
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454355"
---
# <a name="certificateauthority-resource-type"></a>Тип ресурса Цертификатеаусорити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет центр сертификации.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательный. Строка в кодировке Base64, представляющая общедоступный сертификат.|
|цертификатеревокатионлистурл|String|URL-адрес списка отзыва сертификатов.|
|делтацертификатеревокатионлистурл|String|URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.|
|исрутаусорити|Boolean|Обязательный. **true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.|
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