---
title: Тип ресурса application
description: Представляет приложение.
ms.localizationpriority: high
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 399040493f8401574a1094f8d97b528c7f3f6354
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555221"
---
# <a name="application-resource-type"></a>Тип ресурса application

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение. Любое приложение, передающее проверку подлинности в Azure Active Directory (Azure AD), должно быть зарегистрировано в каталоге. Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. Дополнительную информацию см. в статье [Основные сведения о регистрации приложения в Azure AD](/azure/active-directory/develop/authentication-vs-authorization#basics-of-registering-an-application-in-azure-ad). Наследуется от [directoryObject](directoryobject.md).

Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

> [!Note]
> В настоящее время разрабатываются изменения типа ресурса application. Дополнительные сведения см. в статье [Известные проблемы с Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление приложений](../api/application-list.md) | Коллекция [application](application.md) | Получение списка приложений в организации. |
|[Создание приложения](../api/application-post-applications.md) | [application](application.md) | Создает (регистрирует) новое приложение.|
|[Получение приложения](../api/application-get.md) | [application](application.md) |Считывание свойств и связей объекта application.|
|[Обновление приложения](../api/application-update.md) | Нет |Обновление объекта application. |
|[Удаление приложения](../api/application-delete.md) | Нет |Удаление объекта application. |
|[Список удаленных приложений](../api/directory-deleteditems-list.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка недавно удаленных приложений. |
| [Перечисление удаленных приложений, принадлежащих пользователю](../api/directory-deleteditems-user-owned.md) | Коллекция [directoryObject](directoryobject.md) | Получение приложений, принадлежащих пользователю, которые удалены в клиенте за последние 30 дней. |
|[Получение удаленного приложения](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Получение свойств недавно удаленного приложения. |
|[Окончательное удаление приложения](../api/directory-deleteditems-delete.md) | Нет | Окончательное удаление приложения. |
|[Восстановление удаленного приложения](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Восстановление недавно удаленного приложения. |
|[delta](../api/application-delta.md)|Коллекция [application](application.md)| Получение добавочных изменений для приложений. |
|[Создание звонка](../api/application-post-calls.md)|[call](call.md)|Создание звонка путем добавления в коллекцию calls.|
|[Создание собрания по сети](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Создание собрания по сети путем добавления в коллекцию onlineMeetings.|
|**Сертификаты и секреты**| | |
|[Добавление пароля](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|Добавление надежного пароля или секрета в приложение.|
|[Удаление пароля](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|Удаление пароля или секрета из приложения.|
|[Добавление ключа](../api/application-addkey.md)|[keyCredential](keycredential.md)|Добавление учетных данных ключа в приложение.|
|[Удаление ключа](../api/application-removekey.md)|Нет|Удаление учетных данных ключа из приложения.|
|**Расширения**| | |
| [Список объектов extensionProperties](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Создание объекта extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Получение объекта extensionProperty](../api/extensionproperty-delete.md) | Нет | Удаление свойства расширения объекта application. |
| [Удаление объекта extensionProperty](../api/extensionproperty-delete.md) | Нет | Удаление свойства расширения объекта application. |
|**Учетные данные федеративных удостоверений**| | |
| [Список federatedIdentityCredential](../api/application-list-federatedidentitycredentials.md) | Коллекция [federatedIdentityCredential](../resources/federatedidentitycredential.md) | Получение списка учетных данных федеративных удостоверений для объекта application. |
| [Создание federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md) | [federatedIdentityCredential](../resources/federatedidentitycredential.md) | Создание учетных данных федеративных удостоверений для объекта application. |
| [Получение federatedIdentityCredential](../api/federatedidentitycredential-get.md) | [federatedIdentityCredential](../resources/federatedidentitycredential.md) | Получение свойств учетных данных федеративных удостоверений. |
| [Обновление federatedIdentityCredential](../api/federatedidentitycredential-update.md) | Нет | Обновление учетных данных федеративных удостоверений объекта application. |
| [Удаление federatedIdentityCredential](../api/federatedidentitycredential-delete.md) | Нет | Удаление учетных данных федеративных удостоверений из объекта application. |
|**Владельцы**| | |
|[Список владельцев](../api/application-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Добавление владельца](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Добавление владельца путем помещения в коллекцию владельцев.|
|[Удаление владельца](../api/application-delete-owners.md) |Нет| Удаление владельца приложения.|
|**Политики**| | |
|[Назначить tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Присвойте tokenIssuancePolicy этому объекту.|
|[Перечислить tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Назначьте все tokenIssuancePolicies этому объекту.|
|[Убрать tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Удалите tokenIssuancePolicy из этого объекта.|
|[Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Назначение типа ресурса tokenLifetimePolicy объекту.|
|[Перечисление типов ресурсов tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Получение всех типов ресурсов tokenLifetimePolicies, назначенных объекту.|
|[Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Удаление типа ресурса tokenLifetimePolicy из объекта.|
|**Проверенный издатель**| | |
|[Установка проверенного издателя](../api/application-setverifiedpublisher.md)| Нет | Установка проверенного издателя приложения.|
|[Удаление проверенного издателя](../api/application-unsetverifiedpublisher.md)| Нет | Удаление проверенного издателя приложения.|

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#application-properties).

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| addIns | Коллекция [addIn](addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers) для его функции "FileHandler". Это позволит таким службам, как Office 365, вызывать приложение в контексте документов, над которыми работает пользователь. |
| api | [apiApplication](apiapplication.md) | Задает параметры приложения, реализующего веб-API. |
| appId | String | Уникальный идентификатор приложения, назначенный с помощью Azure AD. Значение NULL не допускается. Только для чтения. |
|applicationTemplateId | Строка | Уникальный идентификатор applicationTemplate. Поддерживает `$filter` (`eq`, `not`, `ne`).|
| appRoles | Коллекция [appRole](approle.md) | Совокупность ролей, назначенных приложению. С помощью команды [назначения ролей приложений](approleassignment.md) эти роли можно назначать пользователям, группам или субъектам-службам, связанным с другими приложениями. Значение null не допускается. |
|certification|[certification](certification.md)|Указывает состояние сертификации приложения.|
| createdDateTime | DateTimeOffset | Дата и время регистрации приложения. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.<br><br> Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in` и `eq` для значений `null`) и `$orderBy`. |
|defaultRedirectUri|String|URI перенаправления по умолчанию. Если этот параметр указан и отсутствует явный URI перенаправления в запросе на вход для потоков SAML и OIDC, Azure AD отправляет маркер этому URI перенаправления. Azure AD также отправляет маркер этому стандартному URI при едином входе, инициированном IdP SAML. Значение должно соответствовать одному из настроенных URI перенаправления для приложения.|
| deletedDateTime | DateTimeOffset | Дата и время удаления приложения. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
| description | Строка | Произвольное текстовое поле для описания объекта приложения конечным пользователям. Максимальная длина — 1024 символа. <br><br>Возвращается по умолчанию. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`) и `$search`. |
| disabledByMicrosoftStatus | Строка | Указывает, отключила ли корпорация Майкрософт зарегистрированное приложение. Возможные значения: `null` (значение по умолчанию), `NotDisabled` и `DisabledDueToViolationOfServicesAgreement` (возможные причины: подозрительные, оскорбительные или вредоносные действия, а также нарушение соглашения об использовании служб Майкрософт).<br><br> Поддерживает `$filter` (`eq`, `ne`, `not`). |
| displayName | String | Отображаемое имя приложения. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`. |
| groupMembershipClaims | String | Настраивает утверждение `groups`, выданное в маркере пользователя или маркере доступа OAuth 2.0, ожидаемом приложением. Чтобы задать этот атрибут, используйте одно из следующих строковых значений: `None`, `SecurityGroup` (для групп безопасности и ролей Azure AD), `All` (предоставит все группы безопасности, группы рассылки и роли каталога Azure AD, участником которых является выполнивший вход пользователь). |
| id | String | Уникальный идентификатор объекта приложения. Это свойство называется **идентификатором объекта** на портале Azure. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| identifierUris | Коллекция String | Это значение, также известное как URI идентификатора приложения, задается, когда приложение используется в качестве приложения-ресурса. IdentifierUris выступает в качестве префикса для областей, на которые вы будете ссылаться в коде API, он должен быть уникальным на глобальном уровне. Можно использовать предоставленное по умолчанию значение, которое находится в форме `api://<application-client-id>`, или указать более читаемый URI, например `https://contoso.com/api`. Дополнительные сведения о допустимых шаблонах identifierUris и рекомендуемых методах см. в статье [Рекомендации по безопасной регистрации приложений Azure AD](/azure/active-directory/develop/security-best-practices-for-app-registration#appid-uri-configuration). Значение null не допускается. <br><br>Поддерживает `$filter` (`eq`, `ne`, `ge`, `le`, `startsWith`). |
| info | [informationalUrl](informationalurl.md) | Базовые данные профиля для приложения, такие как URL-адреса маркетинга, поддержки, условий обслуживания и заявления о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в статье [Добавление условий обслуживания и заявления о конфиденциальности для зарегистрированных приложений Azure AD](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le` и `eq` для значений `null`). |
| isDeviceOnlyAuthSupported | Boolean | Указывает, поддерживает ли приложение проверку подлинности устройства без пользователя. Значение по умолчанию: `false`.  |
| isFallbackPublicClient | Boolean | Указывает резервный тип приложения как общедоступный клиент, например установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию — `false`. Это означает, что резервный тип приложения является конфиденциальным клиентом, таким как веб-приложение. В некоторых ситуациях Azure AD не может определить тип клиентского приложения. Например, при потоке [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3), когда приложение настроено без указания URI перенаправления. В таких случаях Azure AD интерпретирует тип приложения на основе значения этого свойства.|
| keyCredentials | Коллекция [keyCredential](keycredential.md) | Коллекция ключевых учетных данных, связанных с приложением. Значение NULL не допускается. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`).|
| logo | Stream | Основной логотип для приложения. Значение NULL не допускается. |
| notes | String | Заметки, важные для управления приложением. |
| oauth2RequiredPostResponse | Boolean | Указывает, позволяет ли Azure AD в рамках запросов маркеров OAuth 2.0 запросы POST в отличие от запросов GET. Значение по умолчанию — `false`. В таком случае позволяются только запросы GET. |
| onPremisesPublishing |[onPremisesPublishing](onpremisespublishing.md)| Представляет набор свойств, необходимых для [настройки прокси-сервера приложений](/graph/application-proxy-configure-api) для этого приложения. Настройка этих свойств позволяет опубликовать локальное приложение для безопасного удаленного доступа. |
| optionalClaims | [optionalClaims](optionalclaims.md) | Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать утверждения, отправляемые в приложения службой маркеров безопасности (Майкрософт). Дополнительные сведения см. в статье [Инструкции: предоставление необязательных утверждений для приложения](/azure/active-directory/develop/active-directory-optional-claims).|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |Указывает параметры родительского контроля для приложения. |
| passwordCredentials | Коллекция [passwordCredential](passwordcredential.md)|Коллекция ключевых учетных данных, связанных с приложением. Значение NULL не допускается.|
| publicClient | [publicClientApplication](publicclientapplication.md) | Указывает параметры для установленных клиентов, например классических или мобильных устройств. |
| publisherDomain | String | Проверенный домен издателя для приложения. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `ge`, `le`, `startsWith`).|
| requiredResourceAccess |Коллекция [requiredResourceAccess](requiredresourceaccess.md)| Указывает ресурсы, к которым приложению необходимо получить доступ. В этом свойстве также указывается набор делегированных разрешений и ролей приложения, необходимых для каждого из этих ресурсов. Эта настройка доступа к необходимым ресурсам определяет порядок предоставления согласия. Можно настроить не более 50 служб ресурсов (API). С середины октября 2021 г. общее количество необходимых разрешений не должно превышать 400. Значение null не допускается. <br><br>Поддерживает `$filter` (`eq`, `not`, `ge`, `le`).|
| samlMetadataUrl | Строка | URL-адрес, по которому служба предоставляет метаданные SAML для федерации. Это свойство допустимо только для приложений с одним клиентом. Допускается значение null. |
| serviceManagementReference | Строка | Ссылки на контактные данные приложения или службы из базы данных управления службами или активами. Возможность обнуления. |
| signInAudience | String | Указывает, учетные записи Майкрософт, которые поддерживаются для текущего приложения. Возможные значения: `AzureADMyOrg`, `AzureADMultipleOrgs`, `AzureADandPersonalMicrosoftAccount` (используется по умолчанию) и `PersonalMicrosoftAccount`. Дополнительные сведения см. в [таблице ниже](#signinaudience-values). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`).|
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Указывает параметры для одностраничного приложения, в том числе URL-адреса выхода и URI перенаправления для кодов авторизации и маркеров доступа. |
| tags |Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается.<br><br>Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
| tokenEncryptionKeyId |Guid|Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке Azure AD шифрует все созданные маркеры с помощью ключа, на который указывает это свойство. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Указывает проверенного издателя приложения. Дополнительные сведения о том, как проверка издателя помогает поддерживать безопасность приложений, надежность и соответствие требованиям, см. в разделе [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).|
| uniqueName | Строка | Уникальный идентификатор, который можно назначить приложению в качестве альтернативного идентификатора. Неизменяемый. Только для чтения. |
| web |[webApplication](webapplication.md)| Указывает параметры для веб-приложения. |
| windows |[windowsApplication](windowsapplication.md)| Указывает параметры приложений для устройств под управлением Microsoft Windows, опубликованных в Microsoft Store или магазине игр Xbox.|

### <a name="signinaudience-values"></a>Значения signInAudience

| Значение | Описание |
|:---------------|:--------|
|AzureADMyOrg|Пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (один клиент).|
|AzureADMultipleOrgs|Пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (несколько клиентов).|
|AzureADandPersonalMicrosoftAccount|Пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации. Для проверки подлинности пользователей с помощью пользовательских потоков Azure AD B2C используйте `AzureADandPersonalMicrosoftAccount`. Это значение позволяет использовать самый широкий набор удостоверений пользователей, включая локальные учетные записи и удостоверения пользователей из Microsoft, Facebook, Google, Twitter или любого поставщика OpenID Connect. Это значение по умолчанию для свойства **signInAudience**.|
|PersonalMicrosoftAccount|Пользователи только с личной учетной записью Майкрософт.|

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|appManagementPolicies|Коллекция [appManagementPolicy](../resources/appManagementPolicy.md)| Параметр appManagementPolicy, примененный к этому приложению.|
|calls           |Коллекция [call](call.md)                  |Только для чтения. Допускается значение null.|
|connectorGroup|[connectorGroup](connectorgroup.md)| Параметр connectorGroup, используемый приложением с прокси приложения Azure AD. Допускается значение NULL.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Только для чтения.|
|extensionProperties|Коллекция [extensionProperty](extensionproperty.md)| Только для чтения. Допускается значение null. Поддерживает `$expand` и `$filter` (`eq` при подсчете пустых коллекций).|
|federatedIdentityCredentials|Коллекция [federatedIdentityCredential](federatedidentitycredential.md) |Федеративные удостоверения для приложений. Поддерживает `$expand` и `$filter` (`eq` при подсчете пустых коллекций).|
|onlineMeetings  |Коллекция [onlineMeeting](onlinemeeting.md)|Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие приложением. Только для чтения. Допускается значение NULL. Поддерживает `$expand`.|
|tokenLifetimePolicies|Коллекция [tokenLifetimePolicy](tokenLifetimePolicy.md)|Типы ресурсов tokenLifetimePolicy, назначенные приложению. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "applicationTemplateId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "certification": {"@odata.type": "microsoft.graph.certification"},
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "disabledByMicrosoftStatus": "String",
  "displayName": "String",
  "groupMembershipClaims": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isDeviceOnlyAuthSupported": false,
  "isFallbackPublicClient": false,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "notes": "String",
  "oauth2RequiredPostResponse": false,
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "serviceManagementReference": "String",
  "signInAudience": "String",
  "spa": {"@odata.type": "microsoft.graph.spaApplication"},
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
  "uniqueName": "String",
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"},
  "web": {"@odata.type": "microsoft.graph.webApplication"},
  "windows": {"@odata.type": "microsoft.graph.windowsApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
