---
title: тип ресурса passwordCredential
description: Содержит учетные данные паролей, связанные с приложением или директором службы.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: 2a4fb91208a09ccf0ca8e06b5431e88b4793e4cc
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854715"
---
# <a name="passwordcredential-resource-type"></a>тип ресурса passwordCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетные данные паролей, связанные с приложением или директором службы. Свойство **passwordCredentials** сущностями application [и](application.md) [servicePrincipal](serviceprincipal.md) — это коллекция **объектов passwordCredential** .

> [!IMPORTANT]
> Использование POST или PATCH для **набора passwordCredential** не поддерживается. Используйте следующие методы addPassword и removePassword, чтобы обновить пароль для приложения или службыPrincipal:
>
> - [приложение: addPassword](../api/application-addpassword.md)
> - [приложение: removePassword](../api/application-removepassword.md)
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binary | Не следует использовать. |
| displayName | Строка | Удобное имя пароля. Необязательное свойство. |
| endDateTime | DateTimeOffset | Дата и время, в течение которых истекает срок действия пароля, представлены в формате ISO 8601 и всегда во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательное свойство. |
| подсказка | Строка | Содержит первые три символа пароля. Только для чтения. |
| keyId | GUID | Уникальный идентификатор пароля. |
| secretText | Строка | Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов. Сгенерированное значение пароля возвращается только во время первоначального запроса POST для [добавленияPassword](../api/application-addpassword.md). В будущем этот пароль не будет извлечен. |
| startDateTime | DateTimeOffset | Дата и время, в течение которых пароль становится допустимым. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательное свойство. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "GUID",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


