---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр объекта приложения в каталоге. Наследуется от directoryObject.
ms.openlocfilehash: c3a08efb1dea1109bd32d59a479260e14089783d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080179"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет экземпляр объекта приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/serviceprincipal-delta.md)).

## <a name="json-representation"></a>Представление JSON
Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "@odata.type": "microsoft.graph.serviceprincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2Permissions": [{"@odata.type": "microsoft.graph.oAuth2Permission"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredTokenSigningKeyThumbprint": "string",
  "publisherName": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "servicePrincipalNames": ["string"],
  "tags": ["string"]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический| **значение true,** Если включена участника учетной записи службы. в противном случае — **false**.            |
|appDisplayName|String|Отображаемое имя, предоставляемые элементом соответствующего приложения.|
|appId|String|Уникальный идентификатор для соответствующего приложения (его свойство **appId** ).|
|appRoleAssignmentRequired|Логический|Указывает, будет ли **appRoleAssignment** пользователю или группе требуется перед Azure AD выпустит пользователя или маркер доступа к приложению. Значение null не допускается. |
|appRoles|Коллекция [роли приложения](approle.md)|Роли приложений, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **appRoles** на сущность [приложения](application.md) . Значение null не допускается. |
|displayName|String|Отображаемое имя участника-службы.|
|errorUrl|String|            |
|Домашняя страница|String|URL-адрес домашней страницы соответствующего приложения.|
|keyCredentials|[keyCredential](keycredential.md) коллекции|Коллекция ключей учетные данные, связанные со службой участника. Значение null не допускается.            |
|logoutUrl|String| Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML.  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md) коллекции|Разрешения OAuth 2.0, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **oauth2Permissions** на сущность [приложения](application.md) . Значение null не допускается.            |
|id|String|Уникальный идентификатор для участников-служб. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|passwordCredentials|[passwordCredential](passwordcredential.md) коллекции|Коллекция пароль учетных данных, связанных с участников-служб. Значение null не допускается. |
|preferredTokenSigningKeyThumbprint|String|Зарезервировано для внутреннего пользования. Не записывать или в противном случае использовать это свойство. Могут быть удалены в будущих версиях. |
|publisherName|String|Отображаемое имя клиента, в котором указаны соответствующего приложения.|
|replyUrls|Коллекция String|URL-адреса, что маркеры пользователей будут отправлены для входа с ним приложении или перенаправления коды авторизации коды URI, OAuth 2.0, и будут отправлены маркеры доступа для соответствующего приложения. Значение null не допускается. |
|samlMetadataUrl|String| |
|servicePrincipalNames|Коллекция String|Коды URI, определение соответствующего приложения. Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://msdn.microsoft.com/library/azure/dn132633.aspx). **Любой** оператор является обязательным для выражения фильтра с несколькими значениями свойств.  Значение null не допускается. |
|теги|Коллекция String| Значение null не допускается. |

## <a name="relationships"></a>Связи
| Связь | Тип |Description|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Субъекты (пользователи, группы и субъектов-служб), назначенные этой участников-служб. Только для чтения.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) коллекции|Приложения, которым назначена участников-служб. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Каталог объекты, созданные в этом участников-служб. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли, которые участника-службы является членом. Методы HTTP: GET только для чтения. Допускается значение null.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) коллекции|Предоставляет олицетворения пользователя, связанные с этой участников-служб. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, принадлежащие участников-служб. Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, являющиеся владельцами участников-служб. Владельцы — это набор пользователей без прав администратора, которые могут изменять этот объект. Только для чтения. Допускается значение null.|
|политика|[политики](policy.md) семейства сайтов|Политики, назначенные для участников-служб.|

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Чтение свойства и связи объекта servicePrincipal.|
|[Список servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) коллекции | Получение списка объектов servicePrincipal. |
|[Создание appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Создайте новый appRoleAssignment, отправку сообщений в коллекцию appRoleAssignments.|
|[Список appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) коллекции| Получите коллекцию объектов appRoleAssignment.|
|[Список createdObjects](../api/serviceprincipal-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получите коллекцию объектов createdObject.|
|[Перечисление memberOf](../api/serviceprincipal-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп, которые эта служба участника непосредственно входит из из свойства навигации член групп.|
|[Доверия транзитивных член списка](../api/serviceprincipal-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, которые участника-службы является членом. Эта операция доверия транзитивных и включает в себя группы, которые эта служба участника, вложенных входит. |
|[Список назначенных политик](../api/policy-list-assigned.md)| [политики](policy.md) семейства сайтов| Получите все политики, назначенные для этого объекта.|
|[Список oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) коллекции| Получите коллекцию объектов oAuth2PermissionGrant.|
|[Список ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получите коллекцию объектов ownedObject.|
|[Добавление владельца](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Создайте новый владелец, отправку сообщений владельцев семейства.|
|[Список владельцев](../api/serviceprincipal-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получите владельцем коллекции объектов.|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Delete](../api/serviceprincipal-delete.md) | Нет |Удалите объект servicePrincipal. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Коллекция String||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Коллекция String||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Коллекция String||
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal коллекции| Получите добавочные изменения субъектов-служб. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
