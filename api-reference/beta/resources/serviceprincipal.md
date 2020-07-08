---
title: Тип ресурса servicePrincipal
description: Представляет экземпляр приложения в каталоге. Наследуется от directoryObject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: b24cf57f4b286c0751e1d0570bd869d2b45ca8f9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080655"
---
# <a name="serviceprincipal-resource-type"></a>Тип ресурса servicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр приложения в каталоге. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/serviceprincipal-delta.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление servicePrincipals](../api/serviceprincipal-list.md) | Коллекция [servicePrincipal](serviceprincipal.md) | Получение списка объектов servicePrincipal. |
|[Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Создает новый объект servicePrincipal. |
|[Получение объекта servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Чтение свойств и связей объекта servicePrincipal.|
|[Обновление servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Обновление объекта servicePrincipal. |
|[Удаление servicePrincipal](../api/serviceprincipal-delete.md) | Нет. |Удаление объекта servicePrincipal.|
|[Перечисление createdObjects](../api/serviceprincipal-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов createdObject.|
|[Перечисление ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов ownedObject.|
|[delta](../api/serviceprincipal-delta.md)|Коллекция servicePrincipal| Получение добавочных изменений для субъектов-служб. |
|**Назначения ролей приложений**| | |
|[Перечисление appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |Коллекция [appRoleAssignment](approleassignment.md)| Получение ролей приложений, которым назначен данный участник службы.|
|[Добавление Аппролеассигнмент](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Назначьте роль приложения этому субъекту службы.|
|[Удаление Аппролеассигнмент](../api/serviceprincipal-delete-approleassignments.md) | Нет | Удаление назначения роли приложения для этого участника службы.|
|[Список Аппролеассигнедто](../api/serviceprincipal-list-approleassignedto.md) |Коллекция [appRoleAssignment](approleassignment.md)| Получение пользователей, групп и субъектов служб, которым назначены роли приложения для этого участника службы.|
|[Добавление Аппролеассигнедто](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Назначьте роль приложения для этого субъекта службы пользователю, группе или субъекту службы.|
|[Удаление Аппролеассигнедто](../api/serviceprincipal-delete-approleassignedto.md) | Нет | Удаление назначения роли приложения для этого участника службы от пользователя, группы или субъекта службы.|
|**Сертификаты и секреты**| | |
|[Добавление пароля](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Добавьте надежный пароль для servicePrincipal.|
|[Удаление пароля](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Удаление пароля из servicePrincipal.|
|[Клавиша прибавления](../api/serviceprincipal-addkey.md)|[кэйкредентиал](keycredential.md)|Добавление ключевых учетных данных в servicePrincipal.|
|[Удалить ключ](../api/serviceprincipal-removekey.md)|Нет|Удаление ключевых учетных данных из servicePrincipal.|
|**Предоставление делегированных разрешений**| | |
|[Перечисление oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)| Получение делегированного разрешения предоставляет авторизацию этого субъекта-службы для доступа к API от имени пользователя, выполнившего вход в систему.|
|**Членство**.| | |
|[Перечисление memberOf](../api/serviceprincipal-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп, непосредственным участником которых является субъект-служба, из свойства навигации memberOf.|
|[Перечисление транзитивных свойств memberOf](../api/serviceprincipal-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Перечисление групп, в которых участвует субъект-служба. Эта операция является транзитивной и включает группы, в которых состоит субъект-служба. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Коллекция String|Проверка участия в указанном списке групп.|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|Коллекция String|Проверка участия в указанном списке группы, роли каталога или объектах административных единиц.|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Коллекция String|Список групп, в которых участвует субъект-служба.|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Коллекция String|Список групп и ролей каталога, в которых участвует субъект-служба.|
|**Owners**| | |
|[Перечисление владельцев](../api/serviceprincipal-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Добавление владельца](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Создание владельца путем добавления в коллекцию владельцев.|
|[Удаление владельца](../api/serviceprincipal-delete-owners.md) |Нет| Удаление владельца из serviceprincipal.|
|**Политики**| | |
|[Назначение типа ресурса claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Назначение типа ресурса claimsMappingPolicy объекту.|
|[Перечисление типов ресурсов claimsMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Получение всех типов ресурсов claimsMappingPolicy, назначенных объекту.|
|[Удаление типа ресурса claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)| Удаление объекта Клаимсмаппингполици из этого объекта.|
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

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.|
| addIns | Коллекция [addIn](addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.|
|алтернативенамес|Коллекция String| Используется для получения субъектов служб по подписке, идентификации группы ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).|
|appDisplayName|String|Отображаемое имя, предоставляемое связанным приложением.|
|appId|String|Уникальный идентификатор для связанного приложения (его свойство **appId**).|
|аппликатионтемплатеид|String|Уникальный идентификатор Аппликатионтемплате, из которого было создано servicePrincipal. Только для чтения.|
|апповнерорганизатионид|String|Содержит идентификатор клиента, в котором зарегистрировано приложение. Это относится только к субъектам-службам, которые поддерживаются приложениями.|
|appRoleAssignmentRequired|Boolean|Указывает, должны ли пользователи или другие субъекты служб предоставлять назначение роли приложения для этого участника службы, прежде чем пользователи смогут входить в систему или получать маркеры. Значение по умолчанию — **false**. Значение null не допускается. |
|appRoles|Коллекция [appRole](approle.md)|Роли, предоставляемые приложением, которое представляет этот участник службы. Дополнительные сведения см. в определении свойства **appRoles** для объекта [application](application.md). Значение null не допускается. |
| deletedDateTime | DateTimeOffset | Дата и время удаления участника службы. Только для чтения. |
|displayName|Строка|Отображаемое имя для субъекта-службы.|
|errorUrl|String|Устаревшие. Не следует использовать.|
|homepage|String|Домашняя или целевая страница приложения.|
| id | String | Уникальный идентификатор для субъекта-службы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
| info | [informationalUrl](informationalurl.md) | Основные сведения о профиле приобретенного приложения, такие как сведения о маркетинговом приложении, поддержке, условия обслуживания и URL-адреса заявления о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в статье [Добавление условий обслуживания и заявления о конфиденциальности для зарегистрированных приложений Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
|keyCredentials|Коллекция [keyCredential](keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|логинурл|String|Указывает URL-адрес, по которому поставщик услуг перенаправляет пользователя в Azure AD для проверки подлинности. Azure AD использует URL-адрес для запуска приложения из Microsoft 365 или Azure AD мои приложения. Если это поле не заполнено, Azure AD выполняет IdP вход для приложений, настроенных с [единым входом на основе SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). Пользователь запускает приложение из Microsoft 365, "Мои приложения Azure AD" или URL-адрес единого входа Azure AD.|
|logoutUrl|String| Указывает URL-адрес, который будет использоваться службой авторизации Майкрософт для выхода пользователя из системы, использующей протоколы OpenId подключения [переднего канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или SAML Logout.|
|notificationEmailAddresses|Коллекция String|Указывает список адресов электронной почты, на которые служба Azure AD отправляет уведомление, если срок действия активного сертификата приближается к дате окончания срока действия. Это относится только к сертификатам, которые используются для подписи маркера SAML, выпущенного для приложений коллекции Azure AD.|
|passwordCredentials|Коллекция [passwordCredential](passwordcredential.md)|Коллекция учетных данных паролей, связанных с субъектом-службой. Значение null не допускается. |
|преферредсинглесигнонмоде|string|Задает режим единого входа, настроенный для этого приложения. Azure AD использует предпочтительный режим единого входа для запуска приложения из Microsoft 365 или Azure AD мои приложения. Поддерживаемые значения: Password, SAML, External и оидк.|
|преферредтокенсигнингкэйенддатетиме|DateTimeOffset|Задает дату истечения срока действия Кэйкредентиал, которая используется для подписи маркеров, помеченной **преферредтокенсигнингкэйсумбпринт**.|
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях. |
|публишедпермиссионскопес|Коллекция [permissionScope](permissionscope.md)|Делегированные разрешения, предоставляемые приложением. Дополнительные сведения см. в свойстве **oauth2PermissionScopes** для свойства **API** сущности [приложения](application.md) . Значение null не допускается.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|samlMetadataUrl|String|URL-адрес, по которому служба предоставляет метаданные SAML для Федерации.|
|самлсинглесигнонсеттингс|[самлсинглесигнонсеттингс](samlsinglesignonsettings.md)|Коллекция параметров, связанных с единым входом SAML.|
|ServicePrincipalNames|Коллекция String|Содержит список **идентифиерсурис**, скопированных из связанного [приложения](application.md). В гибридные приложения можно добавлять дополнительные значения. Эти значения можно использовать для определения разрешений, предоставляемых приложением в Azure AD. For example,<ul><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства для получения маркера доступа, который представляет собой URI, возвращенный в утверждении "ауд".</li></ul><br>Для выражений фильтра в случае многозначных свойств требуется оператор any. Значение null не допускается.|
|сервицепринЦипалтипе|String|Указывает, представляет ли субъект службы приложение или управляемое удостоверение. Это задается службой Azure AD внутренним образом. Для субъекта-службы, представляющего [приложение](./application.md) , задано значение " __приложение__". Для субъекта-службы, представляющего [управляемый идентификатор](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) , он задается как __манажедидентити__.|
|signInAudience|String| Указывает, какие учетные записи Майкрософт поддерживаются для соответствующего приложения. Только для чтения.|
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для категоризации и идентификации участника службы. Значение null не допускается. |
|tokenEncryptionKeyId|String|Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке в Azure AD маркеры проблем для этого приложения шифруются с помощью ключа, указанного этим свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Субъекты (пользователи, группы и субъекты-службы), которые назначены для субъекта-службы. Только для чтения.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Приложения, которым назначен этот субъект-служба. Только для чтения. Допускается значение null.|
|claimsMappingPolicies|Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)|Типы ресурсов claimsMappingPolicy, назначенные субъекту-службе.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные субъектом-службой. Только для чтения. Может иметь значение null.|
|endpoints|Коллекция [endpoint](endpoint.md)|Конечные точки, доступные для обнаружения. Такие службы, как SharePoint, заполняют это свойство определенными конечными точками SharePoint для клиента, которые другие приложения могут обнаружить и использовать в своих впечатлениях.|
|homeRealmDiscoveryPolicies|Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)|Типы ресурсов homeRealmDiscoveryPolicy, назначенные субъекту-службе.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Роли, в которых участвует субъект-служба. Методы HTTP: GET. Только для чтения. Допускается значение null.|
|oauth2PermissionGrants|Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)|Делегированное разрешение предоставляет авторизацию этого субъекта-службы для доступа к API от имени пользователя, выполнившего вход в систему. Только для чтения. Может иметь значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, принадлежащие субъекту-службе. Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, являющиеся владельцами этого servicePrincipal. Владельцы являются набором пользователей, не являющихся администраторами, или СервицепринЦипалс, которым разрешено изменять этот объект. Только для чтения. Может иметь значение null.|
|tokenIssuancePolicies|[tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция|ТокениссуанцеполиЦиес, назначенный этому участнику службы.|
|tokenLifetimePolicies|Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)|Типы ресурсов tokenLifetimePolicy, назначенные субъекту-службе.|

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
  "alternativeNames": "string",
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "applicationTemplateId": "string",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "loginUrl": "string",
  "logoutUrl": "string",
  "notificationEmailAddresses": ["string"],
  "publishedPermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredSingleSignOnMode": "string",
  "preferredTokenSigningKeyEndDateTime": "DateTime",
  "preferredTokenSigningKeyThumbprint": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "samlSingleSignOnSettings": "microsoft.DirectoryServices.SamlSingleSignOnSettings",
  "servicePrincipalNames": ["string"],
  "servicePrincipalType": "string",
  "signInAudience": "String",
  "tags": ["string"],
  "tokenEncryptionKeyId": "String",
  "useCustomTokenSigningKey": false
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
