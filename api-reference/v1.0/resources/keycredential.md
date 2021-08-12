---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: ec191064f0dd14cac67279a6802bc57849e4a740c1e1248cba8234e95ce32c96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196959"
---
# <a name="keycredential-resource-type"></a>тип ресурса keyCredential

Пространство имен: microsoft.graph

Содержит ключевые учетные данные, связанные с приложением <!--or a service principal-->. Свойство **keyCredentials** [приложения](application.md) <!--and [servicePrincipal](serviceprincipal.md)--> объект — это коллекция **keyCredential**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|В двоичном формате| Настраиваемый идентификатор ключа |
| displayName | String | Удобное имя для ключа. Необязательно. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|key|Двоичный| Необработанные данные сертификата в массиве byte, преобразованных в строку Base64; например, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` . |
|keyId|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|String|Тип учетных данных ключей; например, `Symmetric` .|
|использование|String|Строка, описываемая цель, для которой можно использовать ключ; например, `Verify` .|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

