---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр приложения в каталоге. Наследуется от directoryObject.
localization_priority: Priority
ms.openlocfilehash: cd0ac4d440b2e10f935c02393419754989394816
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571865"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

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
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal"
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
  "tags": ["string"],
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.            |
|appDisplayName|String|Отображаемое имя, предоставляемое связанным приложением.|
|appId|String|Уникальный идентификатор для связанного приложения (его свойство **appId**).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения. Значение null не допускается. |
|appRoles|Коллекция [appRole](approle.md)|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **appRoles** для объекта [application](application.md). Значение null не допускается. |
|displayName|String|Отображаемое имя для субъекта-службы.|
|errorUrl|String|            |
|homepage|String|URL-адрес домашней страницы связанного приложения.|
|keyCredentials|Коллекция [keyCredential](keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.  |
|oauth2Permissions|Коллекция [oAuth2Permission](oauth2permission.md)|Разрешения OAuth 2.0, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **oauth2Permissions** для объекта [application](application.md). Значение null не допускается.            |
|id|String|Уникальный идентификатор для субъекта-службы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|passwordCredentials|Коллекция [passwordCredential](passwordcredential.md)|Коллекция учетных данных паролей, связанных с субъектом-службой. Значение null не допускается. |
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях. |
|publisherName|String|Отображаемое имя клиента, в котором указано связанное приложение.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|samlMetadataUrl|String| |
|ServicePrincipalNames|Коллекция String|URI, определяющие связанное приложение. Дополнительные сведения см. в статье [Объекты приложения и объекты субъекта-службы](https://msdn.microsoft.com/library/azure/dn132633.aspx). Для выражений фильтра в случае многозначных свойств требуется оператор **any**.  Значение null не допускается. |
|tags|Коллекция String| Значение null не допускается. |

## <a name="relationships"></a>Связи
| Отношение | Тип |Описание|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Субъекты (пользователи, группы и субъекты-службы), которые назначены для субъекта-службы. Только для чтения.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Приложения, которым назначен субъект-служба. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные субъектом-службой. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли, в которых участвует субъект-служба. Методы HTTP: GET. Только для чтения. Допускается значение null.|
|oauth2PermissionGrants|Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)|Олицетворения пользователя, связанные с субъектом-службой. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, принадлежащие субъекту-службе. Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие субъектом-службой. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Только для чтения. Допускается значение null.|
|policy|Коллекция [policy](policy.md)|Политики, назначенные субъекту-службе.|

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Чтение свойств и связей объекта servicePrincipal.|
|[Перечисление servicePrincipals](../api/serviceprincipal-list.md) | Коллекция [servicePrincipal](serviceprincipal.md) | Получение списка объектов servicePrincipal. |
|[Создание объекта appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Создание объекта appRoleAssignment путем добавления в коллекцию appRoleAssignments.|
|[Перечисление appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |Коллекция [appRoleAssignment](approleassignment.md)| Получение коллекции объектов appRoleAssignment.|
|[Перечисление createdObjects](../api/serviceprincipal-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов createdObject.|
|[Перечисление memberOf](../api/serviceprincipal-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп, непосредственным участником которых является субъект-служба, из свойства навигации memberOf.|
|[Перечисление транзитивных свойств memberOf](../api/serviceprincipal-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Перечисление групп, в которых участвует субъект-служба. Эта операция является транзитивной и включает группы, в которых состоит субъект-служба. |
|[Перечисление назначенных политик](../api/policy-list-assigned.md)| Коллекция [policy](policy.md)| Получение всех политик, назначенных объекту.|
|[Перечисление oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)| Получение коллекции объектов oAuth2PermissionGrant.|
|[Перечисление ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов ownedObject.|
|[Добавление владельца](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Создание владельца путем добавления в коллекцию владельцев.|
|[Перечисление владельцев](../api/serviceprincipal-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Обновление](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Удаление](../api/serviceprincipal-delete.md) | Нет. |Удаление объекта servicePrincipal. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Коллекция String||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Коллекция String||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Коллекция String||
|[delta](../api/serviceprincipal-delta.md)|Коллекция servicePrincipal| Получение добавочных изменений для субъектов-служб. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
