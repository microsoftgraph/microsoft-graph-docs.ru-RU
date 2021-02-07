---
title: Тип ресурса keyCredential
description: Содержит учетные данные ключа, связанные с приложением или основным компонентом-службой. Свойство **keyCredentials** объектов application и servicePrincipal — это коллекция **объектов keyCredential.**
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80583c40b61324b2b150c0ab377e4756f227ce39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135900"
---
# <a name="keycredential-resource-type"></a>Тип ресурса keyCredential

Пространство имен: microsoft.graph

Содержит учетные данные ключа, связанные с приложением <!--or a service principal-->. Свойство **keyCredentials** [приложения](application.md) <!--and [servicePrincipal](serviceprincipal.md)--> объект — это коллекция **keyCredential.**

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| Идентификатор пользовательского ключа |
| displayName | String | Имя ключа. Необязательное свойство. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|keyId|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, когда учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|type|String|Тип учетных данных ключа; например, "Symmetric".|
|usage|String|Строка, описывая назначение, для которого можно использовать ключ; например, "Verify".|
|key|Двоичный| Необработанные данные сертификата в массиве byte, преобразованных в строку Base64; например, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` . |

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
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
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

