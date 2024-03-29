---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр приложения в каталоге. Наследуется от directoryObject.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: dca4b6168121846c6a006260bd741e205c8c1f80
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788761"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/serviceprincipal-delta.md). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление servicePrincipals](../api/serviceprincipal-list.md) | Коллекция [servicePrincipal](serviceprincipal.md) | Получение списка объектов servicePrincipal. |
|[Создать servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Создание нового объекта servicePrincipal. |
|[Получение объекта servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Чтение свойств и связей объекта servicePrincipal.|
|[Обновить servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Удалить servicePrincipal](../api/serviceprincipal-delete.md) | Нет |Удаление объекта servicePrincipal.|
|[Список удаленных servicePrincipals](../api/directory-deleteditems-list.md) | Коллекция [directoryObject](directoryobject.md) | Извлечь список недавно удаленных объектов servicePrincipal. |
|[Получить удаленный servicePrincipal](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Извлечение свойств недавно удаленного объекта servicePrincipal. |
|[Окончательное удаление servicePrincipal](../api/directory-deleteditems-delete.md) | Нет | Окончательное удаление объекта servicePrincipal. |
|[Восстановление удаленного servicePrincipal](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Восстановление недавно удаленного объекта servicePrincipal. |
|[Перечисление createdObjects](../api/serviceprincipal-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов createdObject.|
|[Список ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов ownedObject.|
|[delta](../api/serviceprincipal-delta.md)|Коллекция servicePrincipal| Получение добавочных изменений для субъектов-служб. |
|**Назначение ролей приложений**| | |
|[Перечисление appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |Коллекция [appRoleAssignment](approleassignment.md)| Получение ролей приложений, которым назначен этот субъект-служба.|
|[Добавление объекта appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Назначение роли приложения субъекту-службе.|
|[Удаление объекта appRoleAssignment](../api/serviceprincipal-delete-approleassignments.md) | Нет | Удаление назначения роли приложения субъекта-службы.|
|[List appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |Коллекция [appRoleAssignment](approleassignment.md)| Создание пользователей, ролей и назначенных ролей приложений для этого субъекта-службы.|
|[Add appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Назначение роли для этого субъекта-службы пользователю, группе или субъекту-службе.|
|[Remove appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | Нет | Удаление назначенной роли этого субъекта-службы у пользователя, группы или субъекта-службы.|
|**Сертификаты и секреты**| | |
|[Добавление пароля](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Добавление стойкого пароля или секрета в servicePrincipal.|
|[Добавление tokenSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md)|[selfSignedCertificate](../resources/selfsignedcertificate.md)| Добавление самозаверяющего сертификата в субъект-службу. В основном используется для настройки приложений единого входа на основе SAML из [коллекции Azure AD](/azure/active-directory/saas-apps/tutorial-list).
|[Удаление пароля](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Удаление пароля или секрета из servicePrincipal.|
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
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Коллекция String|Проверка участия в указанном списке групп.|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|Коллекция String|Проверка участия в указанном списке групп, ролях каталога или объектах административных единиц.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Коллекция String|Список групп, в которых участвует субъект-служба.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Коллекция String|Получение списка групп, административных единиц и ролей каталога, в которых состоит субъект-служба.|
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
|**Единый вход**| | |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Создание набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Получение набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|Нет|Обновление набора учетных данных для пользователя или группы, указанных в основном тексте.|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|Нет|Удаление набора учетных данных для пользователя или группы, указанных в основном тексте.|

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#service-principal-properties).

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
| accountEnabled |Boolean| Значение `true`, если учетная запись субъекта-службы включена. В противном случае используется значение `false`. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| addIns | Коллекция [addIn](addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers/) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.|
|alternativeNames|Коллекция строк| Используется для получения субъектов-служб по подпискам, для идентификации групп ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](/azure/active-directory/managed-identities-azure-resources/overview). Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|appDescription|Строка|Описание, предоставляемое связанным приложением.|
|appDisplayName|String|Отображаемое имя, предоставляемое связанным приложением.|
|appId|String|Уникальный идентификатор для связанного приложения (его свойство **appId**). Поддерживает `$filter` (`eq`, `ne`, `not`, `in`, `startsWith`).|
|applicationTemplateId|Строка|Уникальный идентификатор applicationTemplate, из которого создан объект servicePrincipal. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `NOT`, `startsWith`).|
|appOwnerOrganizationId|Guid|Содержит идентификатор клиента, в котором зарегистрировано приложение. Применимо только для субъектов-служб на основе приложений. Поддерживает `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`).|
|appRoleAssignmentRequired|Boolean|Указывает, нужно ли предоставлять назначение роли пользователям или другим субъектам-службам для этого субъекта-службы, прежде чем пользователи смогут выполнять вход, а приложения — получать маркеры. Значение по умолчанию: `false`. Значение NULL не допускается.<br><br>Поддерживает `$filter` (`eq`, `ne`, `NOT`). |
|appRoles|Коллекция [appRole](approle.md)|Роли, предоставляемые приложением, которое представляет этот субъект-служба. Дополнительные сведения см. в определении свойства **appRoles** для объекта [application](application.md). Значение null не допускается. |
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|Открытый сложный тип, который содержит значение настраиваемого атрибута безопасности, назначенного объекту каталога. Допускается значение NULL.<br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter` (`eq`, `ne`, `not`, `startsWith`).|
| deletedDateTime | DateTimeOffset | Дата и время удаления субъекта-службы. Только для чтения. |
| description | String | Поле с произвольным текстом для предоставления внутренним пользователям описания субъекта-службы. На порталах конечных пользователей, например [MyApps](/azure/active-directory/user-help/my-apps-portal-end-user-access), в этом поле будет отображаться описание приложения. Максимальная длина — 1024 символа. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`) и `$search`.|
| disabledByMicrosoftStatus | Строка | Указывает, отключила ли корпорация Майкрософт зарегистрированное приложение. Возможные значения: `null` (значение по умолчанию), `NotDisabled` и `DisabledDueToViolationOfServicesAgreement` (возможные причины: подозрительные, оскорбительные или вредоносные действия, а также нарушение соглашения об использовании служб Майкрософт).<br><br> Поддерживает `$filter` (`eq`, `ne`, `not`).  |
|displayName|String|Отображаемое имя для субъекта-службы. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям), `$search` и `$orderBy`. |
|errorUrl|Строка|Устарело. Не используйте.|
|homepage|String|Главная или начальная страница приложения.|
| id | Строка | Уникальный идентификатор субъекта-службы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение NULL не допускается. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| info | [informationalUrl](informationalurl.md) | Базовые данные профиля для полученного приложения, такие как URL-адреса маркетинга, поддержки, условий обслуживания и заявления о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в статье [Добавление условий обслуживания и заявления о конфиденциальности для зарегистрированных приложений Azure AD](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le` и `eq` для значений `null`).  |
|keyCredentials|Коллекция [keyCredential](keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение NULL не допускается. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`).            |
|loginUrl|String|Указывает URL-адрес, по которому поставщик услуг перенаправляет пользователя в Azure AD для проверки подлинности. Azure AD использует этот URL-адрес для запуска приложения из Microsoft 365 или из раздела "Мои приложения" в Azure AD. Если оставить пустое значение, Azure AD осуществляет вход на основе IdP для приложений, для которых настроен [единый вход на базе SAML](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). Пользователь запускает приложение из Microsoft 365, из раздела "Мои приложения" в Azure AD или по URL-адресу единого входа Azure AD.|
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html) OpenId Connect, [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|notes|String|Поле с произвольным текстом для записи сведений о субъекте-службе, обычно используемых в рабочих целях. Максимальная длина: 1024 символа.|
|notificationEmailAddresses|Коллекция строк|Указывает список адресов электронной почты, по которым Azure AD отправляет уведомление, когда приближается срок окончания действия активного сертификата. Используется только для сертификатов, с помощью которых подписан маркер SAML, выпущенный для приложений коллекции Azure AD.|
|passwordCredentials|Коллекция [passwordCredential](passwordcredential.md)|Коллекция учетных данных паролей, связанных с субъектом-службой. Значение null не допускается. |
|passwordSingleSignOnSettings|[passwordSingleSignOnSettings](passwordsinglesignonsettings.md)|Коллекция для параметров, связанных с единым входом с паролем. Для чтения свойства используйте параметр `$select=passwordSingleSignOnSettings`. Для [applicationTemplates](applicationTemplate.md) предназначено только для чтения, кроме пользовательских объектов applicationTemplates. |
|preferredSingleSignOnMode|Строка|Указывает режим единого входа, настроенный для этого приложения. Azure AD использует предпочитаемый режим единого входа для запуска этого приложения из Microsoft 365 или из раздела "Мои приложения" Azure AD. Поддерживаемые значения: `password`, `saml`, `notSupported` и `oidc`.|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|Указывает дату окончания срока действия keyCredential, использованного для подписи маркера, помеченного с помощью **preferredTokenSigningKeyThumbprint**.|
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях. |
|publishedPermissionScopes|Коллекция [permissionScope](permissionscope.md)|Делегированные разрешения, предоставляемые приложением. Дополнительные сведения см. в описании свойства **oauth2PermissionScopes** в свойстве **api** объекта [application](application.md). Значение null не допускается. <br/>**Примечание.** Это свойство называется **oauth2PermissionScopes** в версии 1.0.|
|replyUrls|Коллекция String|URL-адреса, по которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, по которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение NULL не допускается. |
|samlMetadataUrl|Строка|URL-адрес, по которому служба предоставляет метаданные SAML для федерации.|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|Коллекция для параметров, связанных с единым входом SAML.|
|ServicePrincipalNames|Коллекция объектов string|Содержит список объектов **identifiersUris**, скопированных из связанного объекта [application](application.md). К гибридным приложениям можно добавить дополнительные значения. С помощью этих значений можно идентифицировать разрешения, предоставленные этим приложением в Azure AD. Пример.<ul><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства, чтобы получать маркер доступа, который представляет собой URI, возвращенный в запросе "aud".</li></ul><br>Для выражений фильтра для свойств с несколькими значениями требуется оператор any. Значение NULL не допускается.<br><br> Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|servicePrincipalType|Строка|Указывает, что представляет субъект-служба: приложение или управляемое удостоверение. Это значение устанавливается внутри Azure AD. Если субъект-служба представляет [приложение](./application.md), указывается значение __Application__. Если субъект-служба представляет [управляемое удостоверение](/azure/active-directory/managed-identities-azure-resources/overview), указывается значение __ManagedIdentity__. Тип __SocialIdp__ предназначен для внутреннего использования. |
| signInAudience | String | Указывает учетные записи Майкрософт, которые поддерживаются для текущего приложения. Только для чтения.<br><br>Поддерживаемые значения:<ul><li>`AzureADMyOrg` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (один клиент).</li><li>`AzureADMultipleOrgs` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (несколько клиентов).</li><li>`AzureADandPersonalMicrosoftAccount` — пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации.</li><li>`PersonalMicrosoftAccount` — пользователи только с личной учетной записью Майкрософт.</li></ul> |
|tags|Коллекция объектов string| Настраиваемые строки, которые можно использовать для классификации и определения субъекта-службы. Значение null не допускается.<br><br>Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|tokenEncryptionKeyId|String|Задает значение открытого ключа keyId из коллекции keyCredentials. Если это свойство настроено, Azure AD выпускает маркеры для этого приложения в зашифрованном виде; шифрование производится с помощью ключа, указанного эти свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Определяет проверенного издателя приложения, которое представляет этот субъект-служба.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|appManagementPolicies|Коллекция [appManagementPolicy](../resources/appManagementPolicy.md)| Параметр appManagementPolicy, примененный к этому субъекту-службе.|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Назначение ролей приложений для приложения или службы, предоставляемых пользователям, группам и другим субъектам-службам. Поддерживает `$expand`.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Назначение роли приложения для другого приложения или службы, предоставляемых субъекту-службе. Поддерживает `$expand`.|
|claimsMappingPolicies|Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)|Типы ресурсов claimsMappingPolicy, назначенные субъекту-службе. Поддерживает `$expand`.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные субъектом-службой. Только для чтения. Допускается значение null.|
|delegatedPermissionClassifications|Коллекция [delegatedPermissionClassification](delegatedpermissionclassification.md)|Классификации для делегированных разрешений, предоставленные приложением, которое представляет эта субъект-служба. Поддерживает `$expand`.|
|endpoints|Коллекция [endpoint](endpoint.md)|Конечные точки, доступные для обнаружения. Службы, такие как Sharepoint, заполняют это свойство конечными точками для конкретного клиента SharePoint, которые другие приложения могут обнаружить и использовать в своей работе.|
|homeRealmDiscoveryPolicies|Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)|Типы ресурсов homeRealmDiscoveryPolicy, назначенные субъекту-службе. Поддерживает `$expand`.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли субъекта-службы. Методы HTTP: GET. Только для чтения. Допускается значение NULL. Поддерживает `$expand`.|
|oauth2PermissionGrants|Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)|Делегированные разрешения, предоставляющие субъекту-службе доступ к API от имени пользователя, выполнившего вход. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, принадлежащие субъекту-службе. Только для чтения. Допускается значение NULL. Поддерживает `$expand`.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие этим объектом servicePrincipal. Владельцы — это группа пользователей, не являющихся администраторами или объектами servicePrincipal, которым разрешено изменять этот объект. Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|tokenIssuancePolicies|Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)|Политики tokenIssuancePoliciy, назначенные этому субъекту-службе. Поддерживает `$expand`.|
|tokenLifetimePolicies|Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)|Типы ресурсов tokenLifetimePolicy, назначенные субъекту-службе. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

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
  "alternativeNames": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appOwnerOrganizationId": "Guid",
  "applicationTemplateId": "String",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "disabledByMicrosoftStatus": "String",
  "displayName": "String",
  "errorUrl": "String",
  "homepage": "String",
  "id": "String (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "loginUrl": "String",
  "logoutUrl": "String",
  "notes": "String",
  "notificationEmailAddresses": ["String"],
  "publishedPermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "passwordSingleSignOnSettings": {"@odata.type": "microsoft.graph.passwordSingleSignOnSettings"},
  "preferredSingleSignOnMode": "String",
  "preferredTokenSigningKeyEndDateTime": "DateTime",
  "preferredTokenSigningKeyThumbprint": "String",
  "replyUrls": ["String"],
  "samlMetadataUrl": "String",
  "samlSingleSignOnSettings": "microsoft.DirectoryServices.SamlSingleSignOnSettings",
  "servicePrincipalNames": ["String"],
  "servicePrincipalType": "String",
  "signInAudience": "String",
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
  "useCustomTokenSigningKey": false,
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