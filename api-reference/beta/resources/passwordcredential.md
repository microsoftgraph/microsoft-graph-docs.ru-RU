---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы. Свойство **пассвордкредентиалс** объекта servicePrincipal и сущности приложения является коллекцией **пассвордкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2b62d2e4f0b93e8b7090fe20984faf1644ae2f6b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999425"
---
# <a name="passwordcredential-resource-type"></a>Тип ресурса Пассвордкредентиал

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетные данные пароля, связанные с приложением или субъектом службы. Свойство **пассвордкредентиалс** [приложения](application.md) и [servicePrincipal](serviceprincipal.md) ентититес — это коллекция объектов **пассвордкредентиал** .

> [!IMPORTANT]
> Использование POST или PATCH для установки **пассвордкредентиал** не поддерживается. Используйте методы Аддпассворд и Ремовепассворд для обновления пароля приложения или servicePrincipal:
>
> - [Приложение: Аддпассворд](../api/application-addpassword.md)
> - [Приложение: Ремовепассворд](../api/application-removepassword.md)
> - [servicePrincipal: Аддпассворд](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: Ремовепассворд](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| кустомкэйидентифиер | Binary | Не следует использовать. |
| displayName | String | Понятное имя для пароля. Необязательный параметр. |
| endDateTime | DateTimeOffset | Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Необязательный параметр. |
| сказок | String | Содержит первые три символа пароля. Только для чтения. |
| Него значение KeyID | GUID | Уникальный идентификатор пароля. |
| секреттекст | String | Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов. Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md). В будущем невозможно получить этот пароль. |
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
