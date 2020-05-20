---
title: Тип ресурса Апиаппликатион
description: Задает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2b5676b9a6dce715121b6d5a711cab0e83f948f6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290590"
---
# <a name="apiapplication-resource-type"></a>Тип ресурса Апиаппликатион

Пространство имен: microsoft.graph

Задает параметры приложения, реализующего веб-API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Логический | Если значение равно true, приложение сможет использовать сопоставление утверждений без указания пользовательского ключа подписи. |
|`knownClientApplications`| Коллекция объектов Guid |Используется для предоставления согласия при наличии решения, содержащего две части: клиентское приложение и пользовательское приложение веб-API. Если задать для appID для клиентского приложения это значение, пользователь только один раз отправляется в клиентское приложение. В Azure AD известно, что при отправке клиенту неявным образом отправляются в веб-API и автоматически подготавливает субъекты-службы для обоих API одновременно. Клиентское приложение и веб-API должны быть зарегистрированы в одном клиенте.|
|`oauth2PermissionScopes`| Коллекция [permissionScope](permissionscope.md) | Определение делегированных разрешений, предоставляемых веб-API, представленной регистрацией приложения. Эти делегированные разрешения могут запрашиваться клиентским приложением и могут быть предоставлены пользователями или администраторами во время согласия пользователя. Делегированные разрешения иногда называются областями OAuth 2,0. |
|`preAuthorizedApplications`| Коллекция [preAuthorizedApplication](preauthorizedapplication.md) | Перечисляет клиентские приложения, которые предварительно авторизованы с указанными делегированными разрешениями для доступа к API этого приложения. Пользователям не требуется согласие с какими-либо из предварительно разрешенных приложений (для указанных разрешений). Однако все дополнительные разрешения, не указанные в Преаусоризедаппликатионс (например, по запросу добавочного согласия), требуют согласия пользователя. |
|`requestedAccessTokenVersion`| Int32 | Указывает версию маркера доступа, ожидаемую этим ресурсом. При этом изменяется версия и формат JWT, созданного независимо от конечной точки или клиента, используемого для запроса маркера доступа. <br><br> Используемая конечная точка, v 1.0 или v 2.0, выбирается клиентом и влияет только на версию id_tokens. Ресурсы необходимо явно настроить `requestedAccessTokenVersion` , чтобы указать поддерживаемый формат маркеров доступа. <br><br> Возможные значения `requestedAccessTokenVersion` : `1` , `2` , или `null` . Если задано значение `null` , по умолчанию используется значение `1` , соответствующее конечной точке версии 1.0. <br><br> Если `signInAudience` для приложения задано `AzureADandPersonalMicrosoftAccount` значение, то значение этого свойства должно быть`2` |

## <a name="json-representation"></a>Представление JSON

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
