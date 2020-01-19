---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр приложения в каталоге. Наследуется от directoryObject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 37a4311fe59498a8d210b3ccf6d7184e1263bfb5
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234028"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/serviceprincipal-delta.md).

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
|[Назначение типа ресурса claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Назначение типа ресурса claimsMappingPolicy объекту.|
|[Перечисление типов ресурсов claimsMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Получение всех типов ресурсов claimsMappingPolicy, назначенных объекту.|
|[Удаление типа ресурса claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Удаление типа ресурса tokenLifetimePolicy из объекта.|
|[Назначение типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Назначение типа ресурса homeRealmDiscoveryPolicy объекту.|
|[Перечисление типов ресурсов homeRealmDiscoveryPolicy](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Получение всех типов ресурсов homeRealmDiscoveryPolicy, назначенных объекту.|
|[Удаление типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Удаление типа ресурса homeRealmDiscoveryPolicy из объекта.|
|[Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Назначение типа ресурса tokenLifetimePolicy объекту.|
|[Перечисление типов ресурсов tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Получение всех типов ресурсов tokenLifetimePolicies, назначенных объекту.|
|[Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Удаление типа ресурса tokenLifetimePolicy из объекта.|
|[Перечисление oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)| Получение коллекции объектов oAuth2PermissionGrant.|
|[Перечисление ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов ownedObject.|
|[Добавление владельца](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Создание владельца путем добавления в коллекцию владельцев.|
|[Перечисление владельцев](../api/serviceprincipal-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Обновление](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Удаление](../api/serviceprincipal-delete.md) | Нет. |Удаление объекта servicePrincipal. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Коллекция String|Проверка участия в указанном списке групп.|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|Коллекция String|Проверка участия в указанном списке группы, роли каталога или объектах административных единиц.|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Коллекция String|Список групп, в которых участвует субъект-служба.|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Коллекция String|Список групп и ролей каталога, в которых участвует субъект-служба.|
|[delta](../api/serviceprincipal-delta.md)|Коллекция servicePrincipal| Получение добавочных изменений для субъектов-служб. |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Создание набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|Нет|Удаление набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Получение набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|Нет|Обновление набора учетных данных для пользователя или группы, указанных в основном тексте.|

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
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Субъекты (пользователи, группы и субъекты-службы), которые назначены для субъекта-службы. Только для чтения.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Приложения, которым назначен субъект-служба. Только для чтения. Допускается значение null.|
|claimsMappingPolicies|Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)|Типы ресурсов claimsMappingPolicy, назначенные субъекту-службе.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные субъектом-службой. Только для чтения. Допускается значение null.|
|homeRealmDiscoveryPolicies|Коллекция [homeRealmDiscoveryPolicy](homeRealmDiscoveryPolicy.md)|Типы ресурсов homeRealmDiscoveryPolicy, назначенные субъекту-службе.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли, в которых участвует субъект-служба. Методы HTTP: GET. Только для чтения. Допускается значение null.|
|oauth2PermissionGrants|Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)|Олицетворения пользователя, связанные с субъектом-службой. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, принадлежащие субъекту-службе. Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие субъектом-службой. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Только для чтения. Допускается значение null.|
|tokenLifetimePolicies|Коллекция [tokenLifetimePolicy](tokenLifetimePolicy.md)|Типы ресурсов tokenLifetimePolicy, назначенные субъекту-службе.|

## <a name="json-representation"></a>Представление JSON

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
