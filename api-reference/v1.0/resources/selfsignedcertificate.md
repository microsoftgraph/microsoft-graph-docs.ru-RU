---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: alamaral
ms.openlocfilehash: 6d17c2c1d41733423c1ef3d892df05c442b5ac71
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266415"
---
# <a name="selfsignedcertificate-resource-type"></a>тип ресурса selfSignedCertificate

Пространство имен: microsoft.graph

Содержит публичную часть сертификата подписи. 

Этот тип ресурса — возвращающий тип [действия addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md) Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.

## <a name="properties"></a>Свойства
Свойство|Тип|Описание
----|--|---
|customKeyIdentifier|Binary| Настраиваемый идентификатор ключа. |
| displayName | Строка | Удобное имя для ключа. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|keyId|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|type|Строка|Тип учетных данных ключей. "AsymmetricX509Cert".|
|использование|Строка|Строка, описываемая цель, для которой можно использовать ключ. Возможное значение `Verify` .|
|key|Двоичный| Значение для учетных данных ключа. Должно быть закодированное значение Base-64. |
|отпечатки пальцев| Строка | Значение отпечатка пальца для ключа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
  "@odata.type": "#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "String (Binary)",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "String (Binary)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "thumbprint": "String",
  "type": "String",
  "usage": "String"
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

