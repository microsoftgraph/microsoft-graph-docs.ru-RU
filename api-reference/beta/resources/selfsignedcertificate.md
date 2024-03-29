---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 09e6ed6adfdfe2803e287bb60496e1b0eeb96a6b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723684"
---
# <a name="selfsignedcertificate-resource-type"></a>тип ресурса selfSignedCertificate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит публичную часть сертификата подписи. Это возвращающий тип действия [addTokenSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md). Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.

## <a name="properties"></a>Свойства

| Свойство            | Тип           | Описание                                                                                                                                                                                                                           |
| ------------------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| customKeyIdentifier | Binary         | Настраиваемый идентификатор ключа.                                                                                                                                                                                                                |
| displayName         | String         | Удобное имя для ключа.                                                                                                                                                                                                        |
| endDateTime         | DateTimeOffset | Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.       |
| keyId               | Guid           | Уникальный идентификатор (GUID) для ключа.                                                                                                                                                                                             |
| startDateTime       | DateTimeOffset | Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| type                | String         | Тип учетных данных ключей. "AsymmetricX509Cert".                                                                                                                                                                                     |
| использование               | String         | Строка, описываемая цель, для которой можно использовать ключ. Например, "Проверка".                                                                                                                                             |
| key                 | Двоичный         | Значение для учетных данных ключа. Должно быть закодированное значение base-64.                                                                                                                                                                  |
| отпечатки пальцев          | String         | Значение отпечатка пальца для ключа.                                                                                                                                                                                                     |

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
