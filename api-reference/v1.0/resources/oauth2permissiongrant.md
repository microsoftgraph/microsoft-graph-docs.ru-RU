---
title: тип ресурса oAuth2PermissionGrant
description: Представляет делегированную разрешения (области OAuth 2.0), которые были предоставлены приложению, часто в результате процесса согласия пользователя или администратора.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: c4db52f4d09d8437d8b37879f40245c0acb79e5b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015443"
---
# <a name="oauth2permissiongrant-resource-type"></a>тип ресурса oAuth2PermissionGrant

Пространство имен: microsoft.graph

Представляет делегированную лицензию, выданную директору службы приложения.

Гранты на делегирование разрешений могут создаваться в результате согласия пользователя на запрос приложения на доступ к API или непосредственного создания.

Делегирование разрешений иногда называется "области OAuth 2.0" или "scopes".

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Список oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md) | Получение списка делегирования разрешений. |
| [Получить oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Ознакомьтесь с одним делегированным разрешением.|
| [Создание oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Создание делегированного разрешения. |
| [Обновление oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Нет | Обновление объекта oAuth2PermissionGrant. |
| [Удаление oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Нет  | Удаление делегированного разрешения. |
|[Получение дельты](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Получить вновь созданные, обновленные или удаленные **объекты oauth2permissiongrant** без полного чтения всей коллекции ресурсов.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор **для oAuth2PermissionGrant**. Только для чтения.|
| clientId | String | ID **директора** клиентской службы для приложения, которому разрешено действовать от имени пользователя, входишего в него, при доступе к API. [](serviceprincipal.md) Обязательное. Поддерживает `$filter` (только `eq`). |
| consentType | Строка | Указывает, предоставляется ли клиентской приложению авторизация, чтобы выдать себя за всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию, чтобы выдать себя за всех пользователей. *Principal* указывает авторизацию, чтобы выдать себя за конкретного пользователя. Согласие от имени всех пользователей может быть предоставлено администратором. В некоторых случаях для некоторых делегированных разрешений пользователям, не относя правительственным администраторам, может быть разрешено согласие от имени самих себя. Обязательный. Поддерживает `$filter` (только `eq`). |
| principalId | Строка | ID **пользователя,** от имени которого клиент уполномочен получать доступ к ресурсу, если **consentType** является [](user.md) *основным.* Если **consentType** *— это AllPrincipals,* это значение является null. Обязательно, когда **consentType** является *основным*. |
| resourceId | String | ID **главного** ресурса [службы,](serviceprincipal.md) к которому разрешен доступ. При этом определяется API, который клиент уполномочен пытаться вызвать от имени подписанного пользователя. |
| scope | String | Разделенный пробелом список значений утверждений для делегирования разрешений, которые должны быть включены в маркеры доступа для приложения-ресурса (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения  должно совпадать с полем значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **publishedPermissionScopes** директора [службы ресурсов.](serviceprincipal.md) |

## <a name="relationships"></a>Связи

Отсутствуют.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/oauth2permissiongrant-delta.md).

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

