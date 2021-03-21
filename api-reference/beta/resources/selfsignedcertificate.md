---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: luleonpla
ms.openlocfilehash: f73cb515ce400762771c7553f6f668c295645b90
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965256"
---
# <a name="selfsignedcertificate-resource-type"></a>тип ресурса selfSignedCertificate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит публичную часть сертификата подписи. Это возвращающий тип действия [addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md) Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.

## <a name="properties"></a>Свойства
Свойство|Тип|Описание
----|--|---
|customKeyIdentifier|Binary| Настраиваемый идентификатор ключа |
| displayName | Строка | Удобное имя для ключа. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z". |
|keyId|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z". |
|type|Строка|Тип учетных данных ключей. "AsymmetricX509Cert".|
|использование|Строка|Строка, описываемая цель, для которой можно использовать ключ. Например, "Проверка".|
|key|Двоичный| Значение для учетных данных ключа. Должно быть закодированное значение base-64. |
|отпечатки пальцев| Строка | Значение отпечатка пальца для ключа.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "binary",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "binary",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

