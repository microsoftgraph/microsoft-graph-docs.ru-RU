---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр приложения в каталоге. Наследуется от directoryObject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: ac25e8c54b4e5201a484f139a39136027ac543fe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952510"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

Пространство имен: microsoft.graph

Представляет экземпляр приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/serviceprincipal-delta.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление servicePrincipals](../api/serviceprincipal-list.md) | Коллекция [servicePrincipal](serviceprincipal.md) | Получение списка объектов servicePrincipal. |
|[Создать servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Создание нового объекта servicePrincipal. |
|[Получение объекта servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Чтение свойств и связей объекта servicePrincipal.|
|[Обновить servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Удалить servicePrincipal](../api/serviceprincipal-delete.md) | Нет |Удаление объекта servicePrincipal.|
|[Перечисление createdObjects](../api/serviceprincipal-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов createdObject.|
|[Список ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов ownedObject.|
|[Получение разницы](../api/serviceprincipal-delta.md)|Коллекция servicePrincipal| Получение добавочных изменений для субъектов-служб. |
|**Назначение ролей приложений**| | |
|[Перечисление appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |Коллекция [appRoleAssignment](approleassignment.md)| Получение ролей приложений, которым назначен этот субъект-служба.|
|[Добавление объекта appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Назначение роли приложения субъекту-службе.|
|[Удаление объекта appRoleAssignment](../api/serviceprincipal-delete-approleassignments.md) | Нет | Удаление назначения роли приложения субъекта-службы.|
|[List appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |Коллекция [appRoleAssignment](approleassignment.md)| Создание пользователей, ролей и назначенных ролей приложений для этого субъекта-службы.|
|[Add appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Назначение роли для этого субъекта-службы пользователю, группе или субъекту-службе.|
|[Remove appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | Нет | Удаление назначенной роли этого субъекта-службы у пользователя, группы или субъекта-службы.|
|**Сертификаты и секреты**| | |
|[Добавление пароля](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Добавление стойкого пароля объекту servicePrincipal.|
|[Удаление пароля](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Удаление пароля из servicePrincipal.|
|[Добавление ключа](../api/serviceprincipal-addkey.md)|[keyCredential](keycredential.md)|Добавление учетных данных ключа объекту servicePrincipal.|
|[Удаление ключа](../api/serviceprincipal-removekey.md)|Нет|Удаление учетных данных ключа объекта servicePrincipal.|
|**Классификация делегированных разрешений**| | |
|[Список классификации делегированных разрешений](../api/serviceprincipal-list-delegatedpermissionclassifications.md) |Коллекция [delegatedPermissionClassification](delegatedpermissionclassification.md)| Получение классификаций для делегированных разрешений, предоставленных этим субъектом-службой.|
|[Добавление классификации делегированных разрешений](../api/serviceprincipal-post-delegatedpermissionclassifications.md) |[delegatedPermissionClassification](delegatedpermissionclassification.md) | Добавление классификации для делегированных разрешений, предоставленных этим субъектом-службой. |
|[Удаление классификации делегированных разрешений](../api/serviceprincipal-delete-delegatedpermissionclassifications.md) | Нет | Удаление классификации для делегированных разрешений, предоставленных этим субъектом-службой.|
|**Предоставление делегированных разрешений**| | |
|[Перечисление oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)| Получите предоставление делегированных разрешений, предоставляющих этому объекту-службе доступ к API от имени пользователя, вошедшего в систему.|
|**Членство**.| | |
|[Перечисление memberOf](../api/serviceprincipal-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп, непосредственным участником которых является субъект-служба, из свойства навигации memberOf.|
|[Перечисление транзитивных свойств memberOf](../api/serviceprincipal-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Перечисление групп, в которых участвует субъект-служба. Эта операция является транзитивной и включает группы, в которых состоит субъект-служба. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Коллекция String|Проверка участия в указанном списке групп.|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|Коллекция String|Проверка участия в указанном списке группы, роли каталога или объектах административных единиц.|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Коллекция String|Список групп, в которых участвует субъект-служба.|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Коллекция String|Список групп и ролей каталога, в которых участвует субъект-служба.|
|**Владельцы**| | |
|[Список владельцев](../api/serviceprincipal-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Добавление владельца](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Создание владельца путем добавления в коллекцию владельцев.|
|[Удаление владельца](../api/serviceprincipal-delete-owners.md) |Нет| Удаление владельца serviceprincipal.|
|**Политики**| | |
|[Назначение типа ресурса claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Назначение типа ресурса claimsMappingPolicy объекту.|
|[Перечисление типов ресурсов claimsMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Получение всех типов ресурсов claimsMappingPolicy, назначенных объекту.|
|[Удаление типа ресурса claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Удаление claimsMappingPolicy этого объекта.|
|[Назначение типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Назначение типа ресурса homeRealmDiscoveryPolicy объекту.|
|[Перечисление типов ресурсов homeRealmDiscoveryPolicy](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Получение всех типов ресурсов homeRealmDiscoveryPolicy, назначенных объекту.|
|[Удаление типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Удаление типа ресурса homeRealmDiscoveryPolicy из объекта.|
|[Назначить tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Присвойте tokenIssuancePolicy этому объекту.|
|[Перечислить tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Назначьте все tokenIssuancePolicies этому объекту.|
|[Убрать tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Удалите tokenIssuancePolicy из этого объекта.|
|[Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Назначение типа ресурса tokenLifetimePolicy объекту.|
|[Перечисление типов ресурсов tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Получение всех типов ресурсов tokenLifetimePolicies, назначенных объекту.|
|[Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Удаление типа ресурса tokenLifetimePolicy из объекта.|

## <a name="properties"></a>Свойства
| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.|
| addIns | Коллекция [addIn](addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online&preserve-view=true) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.|
|alternativeNames|Коллекция строк| Используется для получения субъектов-служб по подпискам, для идентификации групп ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).|
|appDescription|Строка|Описание, предоставляемое связанным приложением.|
|appDisplayName|String|Отображаемое имя, предоставляемое связанным приложением.|
|appId|String|Уникальный идентификатор для связанного приложения (его свойство **appId**).|
|applicationTemplateId|Строка|Уникальный идентификатор шаблона applicationTemplate, из которого создан объект servicePrincipal. Только для чтения.|
|appOwnerOrganizationId|Строка|Содержит идентификатор клиента, в котором зарегистрировано приложение. Применимо только для субъектов-служб на основе приложений.|
|appRoleAssignmentRequired|Boolean|Указывает, нужно ли предоставлять назначение роли пользователям или другим субъектам-службам для этого субъекта-службы, прежде чем пользователи смогут выполнять вход, а приложения — получать маркеры. Значение по умолчанию — **false**. Значение null не допускается. |
|appRoles|Коллекция [appRole](approle.md)|Роли, предоставляемые приложением, которое представляет этот субъект-служба. Дополнительные сведения см. в определении свойства **appRoles** для объекта [application](application.md). Значение null не допускается. |
| deletedDateTime | DateTimeOffset | Дата и время удаления субъекта-службы. Только для чтения. |
|description| String | Поле с произвольным текстом для предоставления внутренним пользователям описания субъекта-службы. На порталах конечных пользователей, например [MyApps](/azure/active-directory/user-help/my-apps-portal-end-user-access), в этом поле будет отображаться описание приложения. Максимальная длина — 1024 символа.|
|displayName|String|Отображаемое имя для субъекта-службы.|
|homepage|String|Главная или начальная страница приложения.|
|id|String|Уникальный идентификатор для субъекта-службы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
| info | [informationalUrl](informationalurl.md) | Базовые данные профиля для полученного приложения, такие как URL-адреса маркетинга, поддержки, условий обслуживания и заявления о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в статье [Добавление условий обслуживания и заявления о конфиденциальности для зарегистрированных приложений Azure AD](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
|keyCredentials|Коллекция [keyCredential](keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|loginUrl|String|Указывает URL-адрес, по которому поставщик услуг перенаправляет пользователя в Azure AD для проверки подлинности. Azure AD использует этот URL-адрес для запуска приложения из Microsoft 365 или из раздела "Мои приложения" в Azure AD. Если оставить пустое значение, Azure AD осуществляет вход на основе IdP для приложений, для которых настроен [единый вход на базе SAML](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). Пользователь запускает приложение из Microsoft 365, из раздела "Мои приложения" в Azure AD или по URL-адресу единого входа Azure AD.|
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html) OpenId Connect, [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|notes|String|Поле с произвольным текстом для записи сведений о субъекте-службе, обычно применяемых в рабочих целях. Максимальная длина — 1024 символа.|
|oauth2PermissionScopes|Коллекция [permissionScope](permissionScope.md)|Делегированные разрешения, предоставляемые приложением. Дополнительные сведения см. в описании свойства **oauth2PermissionScopes** в свойстве **api** объекта [application](application.md). Значение null не допускается.|
| notes | String | Поле с произвольным текстом для записи сведений о субъекте-службе, обычно применяемых в рабочих целях. Максимальная длина — 1024 символа. |
|notificationEmailAddresses|Коллекция строк|Указывает список адресов электронной почты, по которым Azure AD отправляет уведомление, когда приближается срок окончания действия активного сертификата. Используется только для сертификатов, с помощью которых подписан маркер SAML, выпущенный для приложений коллекции Azure AD.|
|preferredSingleSignOnMode|Строка|Указывает режим единого входа, настроенный для этого приложения. Azure AD использует предпочитаемый режим единого входа для запуска этого приложения из Microsoft 365 или из раздела "Мои приложения" Azure AD. Поддерживаемые значения: `password`, `saml`, `notSupported` и `oidc`.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|Коллекция для параметров, связанных с единым входом SAML.|
|ServicePrincipalNames|Коллекция объектов string|Содержит список объектов **identifiersUris**, скопированных из связанного объекта [application](application.md). К гибридным приложениям можно добавить дополнительные значения. С помощью этих значений можно идентифицировать разрешения, предоставленные этим приложением в Azure AD. Пример.<ul><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства, чтобы получать маркер доступа, который представляет собой URI, возвращенный в запросе "aud".</li></ul><br>Оператор "any" требуется для выражений фильтров, применяемых к многозначным свойствам. Значение null не допускается.|
|servicePrincipalType|Строка|Указывает, что представляет субъект-служба: приложение или управляемое удостоверение. Это значение устанавливается внутри Azure AD. Если субъект-служба представляет [приложение](./application.md), указывается значение __Application__. Если субъект-служба представляет [управляемое удостоверение](/azure/active-directory/managed-identities-azure-resources/overview), указывается значение __ManagedIdentity__.|
|tags|Коллекция объектов string| Настраиваемые строки, которые можно использовать для классификации и определения субъекта-службы. Значение null не допускается. |
| tokenEncryptionKeyId |String|Задает значение открытого ключа keyId из коллекции keyCredentials. Если это свойство настроено, Azure AD выпускает маркеры для этого приложения в зашифрованном виде; шифрование производится с помощью ключа, указанного эти свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Определяет проверенного издателя приложения, которое представляет этот субъект-служба.

## <a name="relationships"></a>Связи
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Назначение ролей приложений для приложения или службы, предоставляемых пользователям, группам и другим субъектам-службам.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Назначение роли приложения для другого приложения или службы, предоставляемых субъекту-службе.|
|claimsMappingPolicies|Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)|Типы ресурсов claimsMappingPolicy, назначенные субъекту-службе.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные субъектом-службой. Только для чтения. Допускается значение null.|
|homeRealmDiscoveryPolicies|Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)|Типы ресурсов homeRealmDiscoveryPolicy, назначенные субъекту-службе.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли, в которых участвует субъект-служба. Методы HTTP: GET. Только для чтения. Допускается значение null.|
|oauth2PermissionGrants|Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)|Предоставленные делегированные разрешения, разрешающие этому субъекту-службе доступ к API от имени пользователя, вошедшего в систему. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, принадлежащие субъекту-службе. Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие этим объектом servicePrincipal. Владельцы — это группа пользователей, не являющихся администраторами или объектами servicePrincipal, которым разрешено изменять этот объект. Только для чтения. Допускается значение null.|
|tokenIssuancePolicies|Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)|Политики tokenIssuancePoliciy, назначенные этому субъекту-службе.|
|tokenLifetimePolicies|Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)|Типы ресурсов tokenLifetimePolicy, назначенные субъекту-службе.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "endpoints",
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
  "alternativeNames": ["string"] ,
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "displayName": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "notes": "string",
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "replyUrls": ["string"],
  "servicePrincipalNames": ["string"],
  "servicePrincipalType": "string",
  "tags": ["string"],
  "tokenEncryptionKeyId": "String",
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"}
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
  "suppressions": [
    ]
}
-->

