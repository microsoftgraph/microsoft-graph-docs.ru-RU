---
title: тип ресурса certificateAuthority
description: Представляет полномочия сертификата.
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 067eeea8a341525f77427f518b02a07de38a05a1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067488"
---
# <a name="certificateauthority-resource-type"></a>тип ресурса certificateAuthority

Пространство имен: microsoft.graph

Представляет полномочия сертификата.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательное. Кодированная строка base64, представляющая общедоступный сертификат.|
|certificateRevocationListUrl|Строка|URL-адрес списка отзыва сертификата.|
|deltaCertificateRevocationListUrl|Строка|URL-адрес содержит список всех отозванных сертификатов с момента создания полного списка отзыва сертификатов.|
|isRootAuthority|Boolean|Обязательное. **верно,** если доверенный сертификат является корневым **органом,** ложным, если доверенный сертификат является промежуточным органом.|
|эмитент|Строка|Эмитент сертификата, вычисляемого из **значения сертификата.** Только для чтения. |
|issuerSki|Строка|Идентификатор ключа субъекта сертификата, вычисляемого из **значения сертификата.** Только для чтения.|

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
