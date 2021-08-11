---
title: тип ресурса certificateAuthority
description: Представляет полномочия сертификата.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4aa2ecb3c3d16ad942458da190247f1d6f6cb87babc926c97c95605d21d5418d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235683"
---
# <a name="certificateauthority-resource-type"></a>тип ресурса certificateAuthority

Пространство имен: microsoft.graph

Представляет полномочия сертификата.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательный элемент. Кодированная строка base64, представляющая общедоступный сертификат.|
|certificateRevocationListUrl|String|URL-адрес списка отзыва сертификата.|
|deltaCertificateRevocationListUrl|String|URL-адрес содержит список всех отозванных сертификатов с момента создания полного списка отзыва сертификатов.|
|isRootAuthority|Логическое|Обязательный элемент. **верно,** если доверенный сертификат является корневым **органом,** ложным, если доверенный сертификат является промежуточным органом.|
|эмитент|String|Эмитент сертификата, вычисляемого из **значения сертификата.** Только для чтения. |
|issuerSki|String|Идентификатор ключа субъекта сертификата, вычисляемого из **значения сертификата.** Только для чтения.|

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
