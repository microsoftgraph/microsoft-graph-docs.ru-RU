---
title: тип ресурса apiApplication
description: Указывает параметры приложения веб-API.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9cde2098a4ac7a1c9cd8d143513e0b6294a08cd0
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854694"
---
# <a name="apiapplication-resource-type"></a>тип ресурса apiApplication

Пространство имен: microsoft.graph

Задает параметры приложения, реализующего веб-API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|acceptMappedClaims| Логический | Когда `true`, позволяет приложению использовать сопоставление утверждений без указания пользовательского ключа подписи. |
|knownClientApplications| Коллекция GUID |Используется для согласования согласия, если у вас есть решение, которое содержит две части: клиентского приложения и настраиваемого веб-приложения API. Если приложение клиентского приложения установлено к этому значению, пользователь только один раз соглашается на это приложение. Azure AD знает, что согласие клиента означает неявное согласие на веб-API и автоматически предусматривает предоставление основных служб для обоих API одновременно. Клиент и приложение веб-API должны быть зарегистрированы в одном клиенте.|
|oauth2PermissionScopes| Коллекция [permissionScope](permissionscope.md) | Определение делегирования разрешений, выставленных веб-API, представленного этой регистрацией приложений. Эти делегированные разрешения могут запрашиваться клиентской заявкой и могут предоставляться пользователями или администраторами во время согласия. Делегирование разрешений иногда называется областью OAuth 2.0. |
|preAuthorizedApplications| [коллекция preAuthorizedApplication](preauthorizedapplication.md) | Списки клиентских приложений, предварительно авторизованных с указанными делегированных разрешений на доступ к API этого приложения. Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений). Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя. |
|requestedAccessTokenVersion| Int32 | Указывает версию маркера доступа, ожидаемую этим ресурсом. Это меняет версию и формат JWT, выпускаемого независимо от конечной точки или клиента, используемого для запроса маркера доступа. <br><br> Используемая конечная точка , v1.0 или v2.0, выбирается клиентом и влияет только на версию id_tokens. Ресурсы должны явно настроить **запрашиваемыйAccessTokenVersion** , чтобы указать поддерживаемый формат маркера доступа. <br><br> Возможные значения **для requestedAccessSTokenVersion** являются `1`, или `null``2`. Если значение такое `null`, это значение по умолчанию `1`соответствует конечной точке v1.0. <br><br> Если **signInAudience** в приложении настроен как `AzureADandPersonalMicrosoftAccount`, значение для этого свойства должно быть `2` |

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
  "knownClientApplications": ["GUID"],
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

