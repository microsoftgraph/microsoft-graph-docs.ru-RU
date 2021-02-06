---
title: Тип ресурса apiApplication
description: Указывает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 499cc3d86ccab8706838dd3cf883b879d8bcea12
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137104"
---
# <a name="apiapplication-resource-type"></a>Тип ресурса apiApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает параметры приложения, реализующего веб-API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Логический | Если имеет значение true, приложение может использовать сопоставление утверждений без указания пользовательского ключа подписи. |
|`knownClientApplications`| Коллекция объектов Guid |Используется для согласования согласия, если у вас есть решение, которое содержит две части: клиентского приложения и настраиваемого веб-приложения API. Если для appID клиентского приложения задано это значение, пользователь дает согласие только один раз для клиентского приложения. Azure AD знает, что предоставление согласия клиенту означает неявное согласие на веб-API и автоматическое предоставление обоих API-api- и автоматических условий для обоих API. Клиент и приложение веб-API должны быть зарегистрированы в одном клиенте.|
|`oauth2PermissionScopes`| Коллекция [permissionScope](permissionscope.md) | Определение делегирования разрешений, представляемого веб-API, представленным регистрацией этого приложения. Эти делегированные разрешения могут запрашиваться клиентской приложением и предоставляться пользователями или администраторами во время получения согласия. Делегирование разрешений иногда называется областью OAuth 2.0. |
|`preAuthorizedApplications`| [Коллекция preAuthorizedApplication](preauthorizedapplication.md) | Перечисляет клиентские приложения, предварительно авторизованные с помощью указанных делегированных разрешений на доступ к API этого приложения. Пользователи не обязаны соглашаться с любым предварительно авторизованном приложением (для указанных разрешений). Однако любые дополнительные разрешения, не указанные в preAuthorizedApplications (например, запрашиваются с помощью добавимого согласия), требуют согласия пользователя. |
|`requestedAccessTokenVersion`| Int32 | Указывает версию маркера доступа, ожидаемую этим ресурсом. Это изменяет версию и формат JWT независимо от конечной точки или клиента, используемых для запроса маркера доступа. <br><br> Используемая конечная точка версии 1.0 или 2.0 выбирается клиентом и влияет только на версию id_tokens. Ресурсы необходимо явно настроить, чтобы `requestedAccessTokenVersion` указать поддерживаемый формат маркера доступа. <br><br> Возможные `requestedAccessTokenVersion` значения: `1` `2` , или `null` . Если значение за этим значением, значение по умолчанию соответствует конечной точке `null` `1` 1.0. <br><br> Если `signInAudience` в приложении настроено значение, значение `AzureADandPersonalMicrosoftAccount` этого свойства должно быть `2` |

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


