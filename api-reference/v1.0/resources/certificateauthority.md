---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50555ff47d81d96def360fe55fe8684f6ff07994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531952"
---
# <a name="certificateauthority-resource-type"></a>Тип ресурса Цертификатеаусорити

Пространство имен: microsoft.graph

Представляет центр сертификации.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательный элемент. Строка в кодировке Base64, представляющая общедоступный сертификат.|
|цертификатеревокатионлистурл|Строка|URL-адрес списка отзыва сертификатов.|
|делтацертификатеревокатионлистурл|Строка|URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.|
|исрутаусорити|Boolean|Обязательный элемент. **true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.|
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