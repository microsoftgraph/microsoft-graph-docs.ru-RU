---
title: Различия свойств между Azure AD Graph Microsoft Graph
description: Описывает различия свойств между ресурсами Azure AD Graph (сущностями) и microsoft Graph, чтобы помочь соответствующим образом перенести приложения.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fece47dfea3afd007ce148c2a13294b6a89e790d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077658"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия свойств между Azure AD Graph Microsoft Graph

Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

В общем, лучший способ сравнить API Azure Active Directory (Azure AD Graph) с Microsoft Graph — сравнить лежащие метаданные для каждой службы, особенно описания ресурсов:

- [Метаданные Azure AD Graph](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Метаданные Graph Microsoft](https://graph.microsoft.com/beta/$metadata)
- [Метаданные microsoft Graph v1.0](https://graph.microsoft.com/v1.0/$metadata)

Здесь выделяются различия свойств между ресурсами. Если свойство не отображается в этом списке, оно уже доступно в [версии v1.0](/graph/api/overview) Microsoft Graph, с точно таким же именем, как в Azure AD Graph.

Так как пользователи и группы используются так часто, эти ресурсы отображаются в первую очередь.  Другие ресурсы отображаются в алфавитном порядке.

## <a name="user-property-differences"></a>Различия свойств пользователя

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br>свойство|Комментарии|
|---|---|---|
| **deletedTimestamp**| &nbsp; - &nbsp; **бета-версия deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | &nbsp; - &nbsp; **бета-версия onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **faxNumber** <br> v1.0 &nbsp; - &nbsp; **факсНумбер** | |
| **immutableId** | &nbsp; - &nbsp; **бета-версия onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _Недоступны_ | API защиты Graph [майкрософт](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) предоставляет более сложные функции. |
| **lastDirSyncDateTime** | &nbsp; - &nbsp; **бета-версия наPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | &nbsp; - &nbsp; **бета-версия mobilePhone** <br> v1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _Недоступны_ | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство, описывающие все ошибки, связанные с Подключение AD. |
| **refreshTokensValidFromDateTime** | beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v1.0 &nbsp; - &nbsp; **signinSessionsValidFromDateTime** | |
| **signinNames** | &nbsp; - &nbsp; **бета-идентификаторы/signInType** <br> v1.0 &nbsp; - &nbsp; **удостоверений/signInType** | Это свойство теперь является частью [ресурса objectIdentity.](/graph/api/resources/objectIdentity)|
| **telephoneNumber** | &nbsp; - &nbsp; **бета-версии businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | &nbsp; - &nbsp; **бета-фотография**, фотографии <br> v1.0 &nbsp; - &nbsp; **фото**, фотографии | Фотография эскиза Azure AD недоступна в Microsoft Graph.  Вместо этого [используйте API](/graph/api/resources/profilephoto) фотографий. |
| **userIdentities** | идентификаторы &nbsp; - &nbsp; **бета-версии** <br> удостоверения v1.0 &nbsp; - &nbsp;  | Дополнительные сведения см. в типе ресурса [objectIdentity.](/graph/api/resources/objectIdentity)|
| **userState** | beta &nbsp; - &nbsp; **externalUserState** <br> v1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Различия свойств группы

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **dirSyncEnabled** | &nbsp; - &nbsp; **бета-версия onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | &nbsp; - &nbsp; **бета-версия onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | &nbsp; - &nbsp; **бета-версия наPremisesLastSyncDateTime**<br>v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **provisioningErrors** | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _Недоступны_ | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство, описывающие все ошибки, связанные с Подключение AD. |

## <a name="application-property-differences"></a>Различия свойств приложений

| Azure AD Graph <br>(v1.6) свойство | Microsoft Graph<br> свойство                                                                                                                          | Комментарии                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | &nbsp; - &nbsp; **бета-api/acceptMappedClaims** <br> v1.0 &nbsp; - &nbsp; **api/acceptMappedClaims**                                                       | acceptMappedClaims теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | &nbsp; - &nbsp; **бета-версия signInAudience** <br> v1.0 &nbsp; - &nbsp; **signInAudience**                                                                      | Значение по умолчанию для доступныхToOtherTenants (имеется в виду) в то время как для `false` `AzureADMyOrg` signInAudience `AzureADandPersonalMicrosoftAccount` является .                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство обесценилось.                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | &nbsp; - &nbsp; **бета-версия веб/homePageUrl** <br> v1.0 &nbsp; - &nbsp; **web/homePageUrl**                                                                     | Теперь главная страницу является частью нового веб-ресурса.                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | сведения о &nbsp; - &nbsp; **бета-версии** <br> сведения о v1.0 &nbsp; - &nbsp;                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | &nbsp; - &nbsp; **бета-api/knownClientApplications** <br> v1.0 &nbsp; - &nbsp; **api/knownClientApplications**                                               | knownClientApplications теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | &nbsp; - &nbsp; **бета-версия веб/logoutUrl** <br> v1.0 &nbsp; - &nbsp; **web/logoutUrl**                                                                         | logoutUrl теперь является частью веб-ресурса.                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | &nbsp; - &nbsp; **бета-информация/logoUrl** <br> v1.0 &nbsp; - &nbsp; **info/logoUrl**                                                                           | logoUrl теперь является частью нового информационного ресурса.                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | логотип &nbsp; - &nbsp; **бета-версии** <br> логотип v1.0 &nbsp; - &nbsp;                                                                                             |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | &nbsp; - &nbsp; **бета-версия веб/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**         | Переименован, а теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | &nbsp; - &nbsp; **бета-версия веб/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance** | Переименован, а теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство обесценилось.                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | &nbsp; - &nbsp; **бета-api/oauth2PermissionScopes**<br> v1.0 &nbsp; - &nbsp; **api/oauth2PermissionScopes**                                                  | Переименовано и теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                                |
| **publicClient**                   | &nbsp; - &nbsp; **бета-версия —FallbackPublicClient** <br> v1.0 &nbsp; - &nbsp; **isFallbackPublicClient**                                                      | Теперь это свойство имеет новое значение, содержающее общедоступные &nbsp; - &nbsp; параметры клиента, такие как redirectUris. Определение того, является ли приложение общедоступным или конфиденциальным клиентом, теперь делается автоматически, с свойством isFallbackPublicClient, которое не может быть определено автоматически. |
| **recordConsentConditions**        | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство обесценилось.                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | &nbsp; - &nbsp; **бета-версия веб/redirectUris**, **publicClient/redirectUris**<br> v1.0 &nbsp; - &nbsp; **web/redirectUris**, **publicClient/redirectUris**        | Как и переименование, redirectUris теперь является частью новых веб-и общедоступных ресурсовClient. Это позволяет разработчикам использовать определенные URL-адреса для своих веб-клиентов и общедоступных клиентов (например, установленного приложения на настольном устройстве).                                                                                           |
| **samlMetadataUrl**                | &nbsp; - &nbsp; _бета-версия еще недоступна_  <br> v1.0 &nbsp; - &nbsp; _Еще не доступен_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | &nbsp; - &nbsp; _бета-версия недоступна_  <br> v1.0 &nbsp; - &nbsp; _Недоступны_                                                                          | Это свойство не является амортизации, но планируется для servicePrincipal.                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>Различия appRoleAssignment

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **creationTimestamp** | &nbsp; - &nbsp; **бета-созданиеTimestamp** <br> v1.0 &nbsp; - &nbsp; **createdDateTime** | |
| **id** | &nbsp; - &nbsp; **бета-приложениеRoleId** <br> v1.0 &nbsp; - &nbsp; **appRoleId** | |

## <a name="contact-property-differences"></a>Различия свойств контактов

Ресурс Azure AD Graph Contact переименован в orgContact в Microsoft Graph.  Вот различия свойств:

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **город** | &nbsp; - &nbsp; **бета-адреса (город)** <br> v1.0 &nbsp; - &nbsp; **адреса (город)**  | Свойство city является частью коллекции ресурсов адресов. |
| **country** | &nbsp; - &nbsp; **бета-адреса** &nbsp; **(countryOrRegion)**<br> v1.0 &nbsp; - &nbsp; **адреса** &nbsp; **(countryOrRegion)**  | Свойство countryOrRegion является частью коллекции ресурсов адресов. |
| **dirSyncEnabled** | &nbsp; - &nbsp; **бета-версия onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | &nbsp; - &nbsp; **бета-телефоны** &nbsp; **(businessFax)** <br> v1.0 &nbsp; - &nbsp; **телефоны** &nbsp; **(businessFax)** | Теперь часть коллекции телефонов, которая поддерживает мобильные, бизнес и businessFax. |
| **physicalDeliveryOfficeName** | beta &nbsp; - &nbsp; **officeLocation** <br> v1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | &nbsp; - &nbsp; **бета-адреса** &nbsp; **(postalCode)**<br> v1.0 &nbsp; - &nbsp; **адреса** &nbsp; **(почтовый индекс)** | Свойство postalCode является частью коллекции ресурсов адресов. |
| **provisioningErrors** | &nbsp; - &nbsp; бета-версия недоступна <br> v1.0 &nbsp; - &nbsp; недоступна | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство с описанием Подключение связанных ошибок проготовки. В настоящее время это доступно только в бета-версии. |
| **sipProxyAddress** |  beta &nbsp; - &nbsp; **imAddresses**<br> v1.0 &nbsp; - &nbsp; **imAddresses**  | |
| **state** | &nbsp; - &nbsp; **бета-адреса** &nbsp; **(состояние)**<br> v1.0 &nbsp; - &nbsp; **адреса** &nbsp; **(состояние)**  | Свойство состояния является частью коллекции ресурсов адресов. |
| **streetAddress** | &nbsp; - &nbsp; **бета-адреса** &nbsp; **(улица)**<br> v1.0 &nbsp; - &nbsp; **адреса** &nbsp; **(улица)**  | Свойство street является частью коллекции ресурсов адресов. |
| **telephoneNumber** | &nbsp; - &nbsp; **бета-телефоны** &nbsp; **(бизнес)** <br> v1.0 &nbsp; - &nbsp; **телефоны** &nbsp; **(бизнес)** | Теперь часть коллекции телефонов, которая поддерживает мобильные, бизнес и businessFax. |
| **thumbnailPhoto** | &nbsp; - &nbsp; _бета-версия &nbsp; еще &nbsp; недоступна_&nbsp;<br> v1.0 &nbsp; - &nbsp; _Еще не доступен_ | |

## <a name="contract-property-differences"></a>Различия свойств контрактов

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **customerContextId** | beta &nbsp; - &nbsp; **customerId** <br> v1.0 &nbsp; - &nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>Различия свойств устройства

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **approximateLastLogonTimestamp** | &nbsp; - &nbsp; **бета-версия приблизительнымLastSignInDateTime** <br> v1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | &nbsp; - &nbsp; **бета-соответствиеExpirationDateTime** <br> v1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  &nbsp; - &nbsp; **бета-версия deviceVersion** <br> v1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | &nbsp; - &nbsp; **бета-операционная Система** <br> v1.0 &nbsp; - &nbsp; **operatingSystem** |  |
| **deviceOSVersion** | &nbsp; - &nbsp; **бета-операционнаяSystemVersion** <br> v1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta &nbsp; - &nbsp; **physicalIds** <br> v1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | &nbsp; - &nbsp; **бета-версия trustType** <br> v1.0 &nbsp; - &nbsp; **trustType** |  |
| **dirSyncEnabled** |  &nbsp; - &nbsp; **бета-версия onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  &nbsp; - &nbsp; **бета-версия наPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>Различия свойств DirectoryObjectReference

Ресурс Azure AD Graph directoryObjectReference переименован в directoryObjectPartnerReference в Microsoft Graph.  Вот различия свойств:

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **externalContextId** | beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Различия свойств домена

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **name** | &nbsp; - &nbsp; **бета-версия** <br> v1.0 &nbsp; - &nbsp; **id** | В microsoft Graph, уникальный идентификатор (id) содержит доменное имя; свойство `name` не существует. |
| **forceDeleteState** |  состояние &nbsp; - &nbsp; **бета-версии** <br> состояние v1.0 &nbsp; - &nbsp;  | В Azure AD Graph существуют отдельные свойства forceDelete и состояния домена.  В microsoft Graph все состояния домена обрабатываются свойством состояния. |
| **isDefaultForCloudRedirections** | &nbsp; - &nbsp; _бета-версия &nbsp; еще &nbsp; недоступна_&nbsp;<br> v1.0 &nbsp; - &nbsp; _Еще не доступен_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Различия свойств OAuth2PermissionsGrant

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **expiryTime** | beta &nbsp; - &nbsp; **expiryTime** <br> v1.0 &nbsp; - &nbsp; _Удален_ | Это свойство не используется и удаляется в Microsoft Graph v1.0. |
| **startTime** | &nbsp; - &nbsp; **бета-версия startTime** <br> v1.0 &nbsp; - &nbsp; _Удален_  | Это свойство не используется и удаляется в Microsoft Graph v1.0. |

## <a name="policy-property-differences"></a>Различия свойств политики

В microsoft Graph существуют типы политик (например tokenIssuancePolicy или tokenLifetimePolicy), а не тип общих ресурсов политики. Дополнительные сведения доступны в [обзоре политики.](/graph/api/resources/policy-overview)

## <a name="serviceendpoint-property-differences"></a>Различия свойств ServiceEndpoint

Ресурс Azure AD Graph ServiceEndpoint переименован в конечную точку в Microsoft Graph.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **serviceId** | beta &nbsp; - &nbsp; **providerId**<br> v1.0 &nbsp; - &nbsp; **providerId** | |
| **serviceName** | beta &nbsp; - &nbsp; **providerName**<br> v1.0 &nbsp; - &nbsp; **providerName** | |
| **resourceId** | &nbsp; - &nbsp; **бета-провайдерResourceId**<br> v1.0 &nbsp; - &nbsp; **providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>Различия свойств ServicePrincipal

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **appOwnerTenantId** | бета &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | Переименовано. |
| **informationalUrls**| сведения о &nbsp; - &nbsp; **бета-версии** <br> сведения о v1.0 &nbsp; - &nbsp;  | |
| **oauth2Permissions** | beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | Переименовано. |
| **preferredTokenSigningKeyEndDateTime** | &nbsp; - &nbsp; _бета-версия еще недоступна_ <br> v1.0 &nbsp; -  _Еще не доступен_ | |
| **signInAudience** | &nbsp; - &nbsp; _бета-версия еще недоступна_ <br> v1.0 &nbsp; -  _Еще не доступен_ | |
| **serviceEndpoints** | &nbsp; - &nbsp; **Конечная точка бета-версии** <br> конечная точка v1.0 &nbsp; - &nbsp;  | Переименовано. |

## <a name="tenantdetails-property-differences"></a>TenantDetails property differences

Ресурс Azure AD Graph TenantDetails переименован в организацию в Microsoft Graph.  Вот различия свойств:

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **companyLastDirSyncTime** | &nbsp; - &nbsp; **бета-версия наPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | &nbsp; - &nbsp; **бета-версия onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _Недоступны_ | Это свойство и его сведения неподготовлены.|
| **telephoneNumber** | &nbsp; - &nbsp; **бета-версии businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Различия свойств TrustedCasForPasswordlessAuth

Ресурс Azure AD Graph TrustedCasForPasswordlessAuth переименован в [certificateBasedAuthConfiguration.](/graph/api/resources/certificatebasedauthconfiguration) Не существует различий в свойствах; однако существуют различия в типе ресурса **certificateAuthority,** используемом **свойством certificateAuthorities.**

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

Azure AD Graph CertificateAuthorityInformation переименована в **certificateAuthority** в Microsoft Graph. Ниже приводится различие свойств.

|Azure AD Graph <br>(v1.6) свойство |Microsoft Graph<br> свойство|Комментарии|
|---|---|---|
| **authorityType** | &nbsp; - &nbsp; **бета-версия isRootAuthority**<br> v1.0 &nbsp; - &nbsp; **isRootAuthority** | Тип этого свойства также изменился в Boolean. Ранее это свойство должно было быть задавалось как "RootAuthority" или "IntermediateAuthority". Настройка true нового **свойства** эквивалентна "RootAuthority". |
| **crlDistributionPoint** | &nbsp; - &nbsp; **бета-сертификатRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | &nbsp; - &nbsp; **бета-сертификат** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | &nbsp; - &nbsp; **бета-эмитент**<br> эмитент v1.0 &nbsp; - &nbsp;  | |
| **trustedIssuerSki** | beta &nbsp; - &nbsp; **issuerSki**<br> v1.0 &nbsp; - &nbsp; **issuerSki** | |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях методов](migrate-azure-ad-graph-method-differences.md) между Azure AD Graph Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.

