---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет делегированные разрешения (области OAuth 2.0), которые были предоставлены приложению, часто в результате процесса предоставления согласия пользователя или администратора.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 300c44691aab3cc8f09bf621dd39bd89825dee2a
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118454"
---
# <a name="oauth2permissiongrant-resource-type"></a>Тип ресурса oAuth2PermissionGrant

Пространство имен: microsoft.graph

Представляет делегированные разрешения, предоставленные субъекту-службе приложения.

Делегированные разрешения можно создать в результате предоставления пользователем запроса приложения на доступ к API или создания напрямую.

Делегированные разрешения иногда называют "областями OAuth 2.0" или "областями".

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Перечисление oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md) | Получение списка делегированных разрешений. |
| [Получение oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Чтение одного делегированного разрешения.|
| [Создание oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Создайте делегированное предоставление разрешений. |
| [Обновление oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Нет | Обновление объекта oAuth2PermissionGrant. |
| [Удаление oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Нет  | Удаление делегированного разрешения. |
|[Получение дельты](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|Получение вновь созданных, обновленных или удаленных объектов **oauth2permissiongrant** без выполнения полного чтения всей коллекции ресурсов.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | Строка | Уникальный идентификатор **объекта oAuth2PermissionGrant**. Только для чтения.|
| clientId | String | Идентификатор **субъекта-службы** клиента для приложения, которому разрешено действовать от имени вошедвшего пользователя при доступе к API.[](serviceprincipal.md) Обязательный аргумент. Поддерживает `$filter` (только `eq`). |
| consentType | String | Указывает, предоставлена ли клиентским приложениям авторизация для олицетворения всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию для олицетворения всех пользователей. *Субъект* указывает авторизацию для олицетворения определенного пользователя. Согласие от имени всех пользователей может предоставить администратор. В некоторых случаях пользователи, не являемые администраторами, могут иметь разрешение на предоставление согласия от имени себя для некоторых делегированных разрешений. Обязательный аргумент. Поддерживает `$filter` (только `eq`). |
| principalId | String | Идентификатор **пользователя,** от имени [](user.md) которого клиент имеет право на доступ к ресурсу, если **consentType** имеет значение *Principal*. Если **consentType** имеет *значение AllPrincipals* , это значение равно NULL. Требуется, если **consentType является principal***.* Поддерживает `$filter` (только `eq`).|
| resourceId | String | Идентификатор **субъекта-службы** [ресурсов](serviceprincipal.md) , к которому авторизован доступ. Это определяет API, клиент которого имеет право на попытку вызова от имени вошедвшего пользователя. Поддерживает `$filter` (только `eq`). |
| scope | String | Разделенный пробелами список значений утверждений для делегированных разрешений, которые должны быть включены в маркеры доступа для приложения ресурсов (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения должно соответствовать полю значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **oauth2PermissionScopes**  субъекта-службы [ресурсов](serviceprincipal.md). |

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

