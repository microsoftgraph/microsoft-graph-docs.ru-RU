---
title: Тип ресурса certificateAuthority
description: Представляет сертификатный орган.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64461015136129de452227cb0a8de5c7180cfb32
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135102"
---
# <a name="certificateauthority-resource-type"></a>Тип ресурса certificateAuthority

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сертификатный орган.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|certificate|Двоичный|Обязательный элемент. Строка в коде base64, представляющая общедоступный сертификат.|
|certificateRevocationListUrl|Строка|URL-адрес списка отзыва сертификатов.|
|deltaCertificateRevocationListUrl|Строка|URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка отзыва сертификатов.|
|isRootAuthority|Boolean|Обязательный элемент. **имеет** true, если доверенный  сертификат является корневым, false, если доверенный сертификат является промежуточным.|
|issuer|Строка|Вычисляется из значения **сертификата.** Только для чтения. |
|issuerSki|Строка|Идентификатор ключа субъекта сертификата, вычисляемого на **ключевых значениях сертификата.** Только для чтения.|

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

