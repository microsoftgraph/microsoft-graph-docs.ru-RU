---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароля, связанные с приложением или основным приложением-службой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6f7906f2f7411c680eb07c94166e5d324e922d67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137664"
---
# <a name="passwordcredential-resource-type"></a>Тип ресурса passwordCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетные данные пароля, связанные с приложением или основным приложением-службой. Свойство **passwordCredentials** объектов [application](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **объектов passwordCredential.**

> [!IMPORTANT]
> Использование POST или PATCH для применения **passwordCredential** не поддерживается. Используйте методы addPassword и removePassword для обновления пароля приложения или servicePrincipal:
>
> - [application: addPassword](../api/application-addpassword.md)
> - [application: removePassword](../api/application-removepassword.md)
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binary | Не следует использовать. |
| displayName | Строка | Удобное имя пароля. Необязательный параметр. |
| endDateTime | DateTimeOffset | Дата и время истечения срока действия пароля представлены в формате ISO 8601 и всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательный параметр. |
| hint | Строка | Содержит первые три символа пароля. Только для чтения. |
| keyId | Guid | Уникальный идентификатор пароля. |
| secretText | Строка | Только для чтения; Содержит надежные пароли, созданные в Azure AD длиной от 16 до 64 символов. Созданный пароль возвращается только во время первоначального запроса POST для [addPassword.](../api/application-addpassword.md) В будущем получить этот пароль будет не нужно. |
| startDateTime | DateTimeOffset | Дата и время, когда пароль становится действительным. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательный параметр. |

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


## <a name="json-representation"></a>Представление в формате JSON

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
  "keyId": "Guid",
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


