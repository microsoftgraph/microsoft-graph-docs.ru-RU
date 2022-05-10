---
title: Различия свойств между Azure AD Graph и Microsoft Graph
description: Описание различий в свойствах между Azure AD Graph (сущностями) и microsoft Graph, чтобы помочь перенести приложения соответствующим образом.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 2d5df9eede57ff0987bfced91d34c11d4d5142f1
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296243"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия свойств между Azure AD Graph и Microsoft Graph

Эта статья является *частью шага 1. Ознакомьтесь с различиями API* в [процессе переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Как правило, лучший способ сравнить Azure Active Directory (Azure AD) API Graph с Microsoft Graph — сравнить базовые метаданные для каждой службы, особенно описания ресурсов:

- [Azure AD Graph метаданных](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Метаданные Graph microsoft Graph бета-версии](https://graph.microsoft.com/beta/$metadata)
- [Метаданные Microsoft Graph версии 1.0](https://graph.microsoft.com/v1.0/$metadata)

В этой статье рассматриваются различия в свойствах между ресурсами. Если свойство не отображается в этом списке, оно уже доступно в версии [1.0](/graph/api/overview) Microsoft Graph с тем же именем, что и в Azure AD Graph.

Так как [ресурсы пользователей](#user-property-differences) и групп используются так часто, они перечислены первыми.[](#group-property-differences) Другие ресурсы перечислены в алфавитном порядке.

## <a name="user-property-differences"></a>Различия в свойствах пользователей

Ресурс Azure AD Graph **пользователя** наследуется от **DirectoryObject**; он был переименован в пользователя в Microsoft Graph и  наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br>свойство|Комментарии|
|---|---|---|
| **deletedTimestamp**| beta  &nbsp;-&nbsp; **deletedDateTime** <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> **onPremisesSyncEnabled** версии 1.0 &nbsp;-&nbsp; | |
| **facsimileTelephoneNumber** | beta  &nbsp;-&nbsp; **faxNumber** <br> Номер факса версии 1.0 &nbsp;-&nbsp; | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> **onPremisesImmutableId** версии 1.0 &nbsp;-&nbsp;  | |
| **isCompromised** | бета-версия  &nbsp;-&nbsp; _недоступна_ <br> Версия 1.0 &nbsp;-&nbsp; _недоступна_ | API [защиты Graph](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) удостоверений Майкрософт предоставляет более сложные функции. |
| **lastDirSyncDateTime** | beta &nbsp;-&nbsp;**onPremisesLastSyncDateTime** <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | бета-версия  &nbsp;-&nbsp; **mobilePhone** <br> MobilePhone версии 1.0 &nbsp;-&nbsp; | |
| **passwordProfile/enforceChangePasswordPolicy** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** | |
| **passwordProfile/forceChangePasswordNextLogin** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** | |
| **provisioningErrors** | бета-версия &nbsp;-&nbsp; _недоступна_ <br> Версия 1.0 &nbsp;-&nbsp; _недоступна_ | Это свойство и его сведения являются нерекомендуемыми.  Однако новое свойство, описывающее все ошибки подготовки Подключение AD, можно найти в **onPremisesProvisioningErrors**. |
| **refreshTokensValidFromDateTime** | **betasigninSessionsValidFromDateTime**&nbsp;-&nbsp;<br>**v1.0signinSessionsValidFromDateTime**&nbsp;-&nbsp; | |
| **signinNames** | beta &nbsp;-&nbsp; **identities/signInType** <br> Удостоверения версии 1.0 &nbsp;-&nbsp; **/signInType** | Это свойство теперь является частью [ресурса objectIdentity](/graph/api/resources/objectIdentity) .|
| **telephoneNumber** | бета-версии  &nbsp;-&nbsp; **businessPhone** <br> **Бизнес-устройства версии** 1.0 &nbsp;-&nbsp; | |
| **thumbnailPhoto** | **бета-версия**&nbsp;-&nbsp; фотографии, фотографии <br> фотография версии 1.0 &nbsp;-&nbsp; **,** фотографии | Фотография Azure AD эскиза недоступна в Microsoft Graph.  Вместо этого [используйте API](/graph/api/resources/profilephoto) фотографий. |
| **userIdentities** | бета-версии &nbsp;-&nbsp; **удостоверений** <br> Удостоверения версии 1.0 &nbsp;-&nbsp; | Дополнительные сведения см. в описании типа ресурса [objectIdentity](/graph/api/resources/objectIdentity) .|
| **userState** | beta  &nbsp;-&nbsp; **externalUserState** <br> v1.0 &nbsp;-&nbsp; **externalUserState** | |
| **userStateChangedOn** | **betaexternalUserStateChangeDateTime**&nbsp;-&nbsp;<br>**v1.0externalUserStateChangeDateTime**&nbsp;-&nbsp; | |

## <a name="group-property-differences"></a>Различия в свойствах группы

Ресурс Azure AD Graph **группы** наследуется от **DirectoryObject**; он был переименован в группу в Microsoft Graph  и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> **onPremisesSyncEnabled** версии 1.0 &nbsp;-&nbsp; | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> **onPremisesImmutableId** версии 1.0 &nbsp;-&nbsp; | |
| **lastDirSyncDateTime** | **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp;<br>**v1.0onPremisesLastSyncDateTime**&nbsp;-&nbsp; | |
| **provisioningErrors** | бета-версия &nbsp;-&nbsp; _недоступна_ <br> Версия 1.0 &nbsp;-&nbsp; _недоступна_ | Это свойство и его сведения являются нерекомендуемыми.  Однако новое свойство, описывающее все ошибки подготовки Подключение AD, можно найти в **onPremisesProvisioningErrors**. |

## <a name="application-property-differences"></a>Различия в свойствах приложения

Ресурс Azure AD Graph **наследуется** от **DirectoryObject**; он был переименован в приложение в Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.


| Azure AD Graph <br>(v1.6) свойство | Microsoft Graph<br> свойство                                                                                                                          | Комментарии                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | бета-API &nbsp;-&nbsp;**/acceptMappedClaims** <br> API версии 1.0 &nbsp;-&nbsp; **/acceptMappedClaims**                                                       | AcceptMappedClaims теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | бета-версия &nbsp;-&nbsp; **signInAudience** <br> **SignInAudience** версии 1.0 &nbsp;-&nbsp;                                                                      | Значение по умолчанию для availableToOtherTenants равно `false` (то есть`AzureADMyOrg`) в то время как для signInAudience — .`AzureADandPersonalMicrosoftAccount`                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | бета-версия &nbsp;-&nbsp;_недоступна_ <br> Версия 1.0 &nbsp;-&nbsp;  _недоступна_                                                                            | Это свойство является устаревшим.                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp;-&nbsp;**web/homePageUrl** <br> Web/**homePageUrl** версии 1.0 &nbsp;-&nbsp;                                                                     | домашняя страница теперь является частью нового веб-ресурса.                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | Бета-версия &nbsp;-&nbsp;**сведений** <br> Сведения о версии 1.0 &nbsp;-&nbsp;                                                                                           |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | betaapi&nbsp;-&nbsp;**/knownClientApplications** <br> API версии 1.0 &nbsp;-&nbsp;**/knownClientApplications**                                               | KnownClientApplications теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp;-&nbsp;**web/logoutUrl** <br> Web **/logoutUrl** версии 1.0 &nbsp;-&nbsp;                                                                         | LogoutUrl теперь является частью веб-ресурса.                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | бета-версия &nbsp;-&nbsp;**info/logoUrl** <br> Сведения и **логотип версии** 1.0 &nbsp;-&nbsp;                                                                           | LogoUrl теперь является частью нового информационного ресурса.                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | Логотип **бета-версии** &nbsp;-&nbsp; <br> Логотип версии 1.0 &nbsp;-&nbsp;                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | betaweb&nbsp;-&nbsp;**/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**         | Переименован и теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | betaweb&nbsp;-&nbsp;**/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableAccessTokenIssuance** | Переименован и теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | бета-версия &nbsp;-&nbsp;_недоступна_ <br> Версия 1.0 &nbsp;-&nbsp;  _недоступна_                                                                            | Это свойство является устаревшим.                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | betaapi&nbsp;-&nbsp;**/oauth2PermissionScopes**<br> API версии 1.0 &nbsp;-&nbsp;**/oauth2PermissionScopes**                                                  | Переименован и теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp;-&nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp;-&nbsp; **isFallbackPublicClient**                                                      | Теперь это свойство имеет новое значение &nbsp;-&nbsp; , которое содержит общедоступные параметры клиента, такие как redirectUris. Определение того, является ли приложение общедоступным или конфиденциальным клиентом, теперь выполняется автоматически с помощью свойства isFallbackPublicClient, обрабатывающее один особый случай, который не может быть определен автоматически. |
| **recordConsentConditions**        | бета-версия &nbsp;-&nbsp;_недоступна_ <br> Версия 1.0 &nbsp;-&nbsp;  _недоступна_                                                                            | Это свойство является устаревшим.                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | betaweb&nbsp;-&nbsp;**/redirectUris**, **publicClient/redirectUris**<br> v1.0 &nbsp;-&nbsp;**web/redirectUris**, **publicClient/redirectUris**        | Как и переименование, redirectUris теперь является частью новых веб-ресурсов и ресурсов publicClient. Это позволяет разработчикам использовать определенные универсальные коды ресурса (URI) для своих веб-клиентов и общедоступных клиентов (например, установленное приложение на настольном устройстве).                                                                                           |
| **samlMetadataUrl**                | бета-версия  &nbsp;-&nbsp; _еще не доступна_  <br> Версия 1.0 &nbsp;-&nbsp; _пока недоступна_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | бета-версия  &nbsp;-&nbsp; _недоступна_  <br> Версия 1.0 &nbsp;-&nbsp; _недоступна_                                                                          | Это свойство является устаревшим, но планируется для servicePrincipal.                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>Различия AppRoleAssignment

Ресурс Azure AD Graph **AppRoleAssignment** наследуется от **DirectoryObject**; он был переименован в **appRoleAssignment** в Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.


|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **creationTimestamp** | beta &nbsp;-&nbsp;**creationTimestamp** <br> Версия 1.0 &nbsp;-&nbsp;**createdDateTime** | |
| **id** | beta &nbsp;-&nbsp;**appRoleId** <br> **AppRoleId** версии 1.0 &nbsp;-&nbsp; | |

## <a name="contact-property-differences"></a>Различия в свойствах контактов

Ресурс Azure AD Graph **Contact** наследуется от **DirectoryObject**; он был переименован в **orgContact** в Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **Города** | **betaaddresse**&nbsp;-&nbsp;/city <br> Адреса и город версии 1.0 &nbsp;-&nbsp;  | Свойство **city** является частью коллекции **ресурсов адресов** . |
| **country** | betaaddresses&nbsp;-&nbsp;**/countryOrRegion**<br> v1.0addresses&nbsp;-&nbsp;**/countryOrRegion**  | Свойство **countryOrRegion** входит в **коллекцию ресурсов адресов** . |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> **onPremisesSyncEnabled** версии 1.0 &nbsp;-&nbsp;   | |
| **facsimileTelephoneNumber** | betaphones&nbsp;-&nbsp;**/businessFax** <br> Телефоны и **businessFax версии** 1.0 &nbsp;-&nbsp; | Теперь входит в **коллекцию телефонов** , которая поддерживает различные типы телефонов. |
| **physicalDeliveryOfficeName** | beta &nbsp;-&nbsp;**officeLocation** <br> **OfficeLocation** версии 1.0 &nbsp;-&nbsp; | |
| **postalCode** | betaaddresses&nbsp;-&nbsp;**/postalCode**<br> Адреса и **почтовый индекс** версии 1.0 &nbsp;-&nbsp; | Свойство **postalCode** является частью коллекции **ресурсов адресов** . |
| **provisioningErrors** | бета-версия &nbsp;-&nbsp; недоступна <br> Версия 1.0 &nbsp;-&nbsp; недоступна | Это свойство и его сведения являются нерекомендуемыми.  Однако новое свойство, описывающее все ошибки подготовки Подключение AD, можно найти в **onPremisesProvisioningErrors**. В настоящее время это доступно только в `beta`. |
| **sipProxyAddress** |  beta &nbsp;-&nbsp;**imAddresses**<br> **ImAddresses** версии 1.0 &nbsp;-&nbsp;  | |
| **state** | бета-адреса &nbsp;-&nbsp;**и состояние**<br> Адреса и состояние версии 1.0 &nbsp;-&nbsp;  | Свойство **state** является частью коллекции **ресурсов адресов** . |
| **streetAddress** | бета-адреса &nbsp;-&nbsp;**/улицы**<br> Адреса и улицы версии 1.0 &nbsp;-&nbsp;  | Свойство **street** является частью коллекции **ресурсов адресов** . |
| **telephoneNumber** | betaphones&nbsp;-&nbsp;**/business** <br> Телефоны и бизнес версии 1.0 &nbsp;-&nbsp; | Теперь входит в **коллекцию телефонов** , которая поддерживает различные типы телефонов. |
| **thumbnailPhoto** | beta &nbsp;-&nbsp;_Notyetavailable&nbsp;&nbsp;_&nbsp;<br> Версия 1.0 &nbsp;-&nbsp; _пока недоступна_ | |

## <a name="contract-property-differences"></a>Различия в свойствах контракта

Ресурс Azure AD Graph **контракта** наследуется от **DirectoryObject**; он был переименован в контракт в Microsoft Graph и  наследуется от **directoryObject**. Ниже приведены различия в свойствах.


|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **customerContextId** | beta &nbsp;-&nbsp;**customerId** <br> Идентификатор клиента версии 1.0 &nbsp;-&nbsp;  |  |

## <a name="device-property-differences"></a>Различия в свойствах устройств

Ресурс Azure AD Graph **устройства** наследуется от **DirectoryObject**; он был переименован в устройство в Microsoft Graph и  наследуется от **directoryObject**. Ниже приведены различия в свойствах.


|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **approximateLastLogonTimestamp** | **betaapproximateLastSignInDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | **betacomplianceExpirationDateTime**&nbsp;-&nbsp; <br> Версия 1.0 &nbsp;-&nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  **betadeviceVersion**&nbsp;-&nbsp; <br> Версия 1.0 &nbsp;-&nbsp; **deviceVersion** |  |
| **deviceOSType** | **betaoperatingSystem**&nbsp;-&nbsp; <br> Операционная система версии 1.0 &nbsp;-&nbsp; |  |
| **deviceOSVersion** | **betaoperatingSystemVersion**&nbsp;-&nbsp; <br> Версия 1.0 &nbsp;-&nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | **betaphysicalIds**&nbsp;-&nbsp; <br> Физические идентификаторы версии 1.0 &nbsp;-&nbsp; |  |
| **deviceTrustType** | **betatrustType**&nbsp;-&nbsp; <br> Тип доверия версии 1.0 &nbsp;-&nbsp; |  |
| **dirSyncEnabled** |  **betaonPremisesSyncEnabled**&nbsp;-&nbsp; <br> **onPremisesSyncEnabled** версии 1.0 &nbsp;-&nbsp; |  |
| **lastDirSyncTime** |  **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobject-property-differences"></a>Различия свойств DirectoryObject

Ресурс Azure AD Graph **DirectoryObject** переименован в **directoryObject** в Microsoft Graph. Изменения его свойств также будут видны в других ресурсах, которые наследуются **от DirectoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **deletionTimestamp** | **betadeletedDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | Хотя **deletionTimestamp был** типом DateTime, **deletedDateTime** является типом DateTimeOffset.  |
| **Objectid** | betaid&nbsp;-&nbsp; <br> Идентификатор версии 1.0 &nbsp;-&nbsp; | Свойство **id** в Microsoft Graph наследуется [от ресурса сущности](/graph/api/resources/entity). |
| **objectType** | Доступно *betaNot*&nbsp;-&nbsp; <br> Версия 1.0 &nbsp;-&nbsp; *недоступна* | Это свойство не используется в microsoft Graph. Вместо этого Microsoft Graph возвращает свойство **@odata.type**, но только для API, которые могут возвращать объекты разных типов или производных типов. Например, API [членов](/graph/api/group-list-members) группы списка может возвращать участников, которые являются пользователями [,](/graph/api/resources/user) группами [,](/graph/api/resources/group) субъектами-службами [,](/graph/api/resources/serviceprincipal) контактами [организации](/graph/api/resources/orgcontact) или [устройствами](/graph/api/resources/device). Для пользователей используется **@odata.type**`#microsoft.graph.user`. |

## <a name="directoryobjectreference-property-differences"></a>Различия свойств DirectoryObjectReference

Ресурс Azure AD Graph **DirectoryObjectReference** наследуется от **DirectoryObject**; он был переименован в **directoryObjectPartnerReference** в Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **externalContextId** | **betaexternalPartnerTenantId**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Различия в свойствах домена

Ресурс Azure AD Graph **домена** переименован в **домен в Microsoft** Graph. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **name** | betaid&nbsp;-&nbsp; <br> Идентификатор версии 1.0 &nbsp;-&nbsp; | В Microsoft Graph уникальный идентификатор (идентификатор) содержит доменное имя; `name` свойство не существует. |
| **forceDeleteState** |  **betastate**&nbsp;-&nbsp; <br> Состояние версии 1.0 &nbsp;-&nbsp; | В Azure AD Graph существуют отдельные свойства forceDelete и состояния домена.  В microsoft Graph все состояния домена обрабатываются свойством состояния. |
| **isDefaultForCloudRedirections** | _betaNotyetavailable&nbsp;&nbsp;_&nbsp;-&nbsp;&nbsp;<br> Версия 1.0 &nbsp;-&nbsp; _пока недоступна_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Различия в свойствах OAuth2PermissionsGrant

Ресурс Azure AD Graph **OAuth2PermissionsGrant** переименован в **oAuth2PermissionsGrant** в Microsoft Graph. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **истечение срока действия** | **betaexpiryTime**&nbsp;-&nbsp; <br> _v1.0Removed_&nbsp;-&nbsp; | Это свойство не используется и удаляется в Microsoft Graph версии 1.0. |
| **Starttime** | **betastartTime**&nbsp;-&nbsp; <br> _v1.0Removed_&nbsp;-&nbsp;  | Это свойство не используется и удаляется в Microsoft Graph версии 1.0. |

## <a name="policy-property-differences"></a>Различия свойств политики

В Microsoft Graph существуют именованные типы политик (например **, tokenIssuancePolicy** или **tokenLifetimePolicy**), а не тип ресурса универсальной политики. Дополнительные сведения см. в [обзоре политики](/graph/api/resources/policy-overview).

## <a name="serviceendpoint-property-differences"></a>Различия в свойствах ServiceEndpoint

Ресурс Azure AD Graph **ServiceEndpoint** наследуется от **DirectoryObject**; он был переименован в конечную точку в  Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **serviceId** | **betaproviderId**&nbsp;-&nbsp;<br> Идентификатор поставщика версии 1.0 &nbsp;-&nbsp; | |
| **serviceName** | **betaproviderName**&nbsp;-&nbsp;<br> Имя поставщика версии 1.0 &nbsp;-&nbsp; | |
| **resourceId** | **betaproviderResourceId**&nbsp;-&nbsp;<br> V1.0 &nbsp;-&nbsp;**providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>Различия в свойствах ServicePrincipal

Ресурс Azure AD Graph **ServicePrincipal** наследуется от **DirectoryObject**; он был переименован в **servicePrincipal** в Microsoft Graph и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **appOwnerTenantId** | **betaappOwnerOrganizationId**&nbsp;-&nbsp; <br> **AppOwnerOrganizationId** версии 1.0 &nbsp;-&nbsp; | Переименован. |
| **informationalUrls**| Бета-версия &nbsp;-&nbsp;**сведений** <br> Сведения о версии 1.0 &nbsp;-&nbsp; | |
| **oauth2Permissions** | beta  &nbsp;-&nbsp;**publishedPermissionScopes** <br> v1.0  &nbsp;-&nbsp;**oauth2PermissionScopes** | Переименован. |
| **preferredTokenSigningKeyEndDateTime** | _Бета-заметка_&nbsp;-&nbsp; пока доступна <br> Версия 1.0 &nbsp;- _пока недоступна_ | |
| **signInAudience** | _Бета-заметка_&nbsp;-&nbsp; пока доступна <br> Версия 1.0 &nbsp;- _пока недоступна_ | |
| **serviceEndpoints** | **betaendpoint**&nbsp;-&nbsp; <br> Конечная точка версии 1.0 &nbsp;-&nbsp; | Переименован. |

## <a name="tenantdetails-property-differences"></a>Различия свойств TenantDetails

Ресурс Azure AD Graph **TenantDetail** наследуется от **DirectoryObject**; он был переименован в организацию в Microsoft Graph  и наследуется от **directoryObject**. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **companyLastDirSyncTime** | **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp; <br> **v1.0onPremisesLastSyncDateTime**&nbsp;-&nbsp; |  |
| **dirSyncEnabled** | **betaonPremisesSyncEnabled**&nbsp;-&nbsp; <br> **onPremisesSyncEnabled** версии 1.0 &nbsp;-&nbsp; |  |
| **provisioningErrors** | Доступно _betaNot_&nbsp;-&nbsp; <br> Версия 1.0 _. Доступно_&nbsp;-&nbsp; | Это свойство и его сведения являются нерекомендуемыми.|
| **telephoneNumber** | **betabusinessPhones**&nbsp;-&nbsp; <br> **V1.0businessPhones**&nbsp;-&nbsp; |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Различия в свойствах TrustedCasForPasswordlessAuth

Ресурс Azure AD Graph **TrustedCasForPasswordlessAuth** переименован в [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration). Различия между свойствами отсутствуют. Однако существуют различия в типе ресурса **certificateAuthority** , используемом **свойством certificateAuthorities** .

### <a name="certificateauthorityinformation-property-differences"></a>Различия свойств CertificateAuthorityInformation

Объект Azure AD Graph **CertificateAuthorityInformation** переименован в **certificateAuthority** в Microsoft Graph. Ниже приведены различия в свойствах.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **authorityType** | **betaisRootAuthority**&nbsp;-&nbsp;<br> **IsRootAuthority** версии 1.0 &nbsp;-&nbsp; | Тип этого свойства также изменился на логический. Ранее для этого свойства необходимо было задать значение RootAuthority или IntermediateAuthority. Присвоение новому **свойству значения true** эквивалентно значению RootAuthority. |
| **crlDistributionPoint** | **betacertificateRevocationListUrl**&nbsp;-&nbsp; <br> **v1.0certificateRevocationListUrl**&nbsp;-&nbsp; | |
| **deltaCrlDistributionPoint** | **betadeltaCertificateRevocationListUrl**&nbsp;-&nbsp; <br> **v1.0deltaCertificateRevocationListUrl**&nbsp;-&nbsp; | |
| **trustedCertificate** | **betacertificate**&nbsp;-&nbsp; <br> **v1.0deltaCertificateRevocationListUrl**&nbsp;-&nbsp; | |
| **trustedIssuer** | **betaissuer**&nbsp;-&nbsp;<br> Версия **1.0issuer**&nbsp;-&nbsp; | |
| **trustedIssuerSki** | **betaissuerSki**&nbsp;-&nbsp;<br> **IssuerSki** версии 1.0 &nbsp;-&nbsp; | |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях методов](migrate-azure-ad-graph-method-differences.md) между Azure AD Graph и Microsoft Graph.
- Проверьте [контрольный список](migrate-azure-ad-graph-planning-checklist.md) еще раз.

