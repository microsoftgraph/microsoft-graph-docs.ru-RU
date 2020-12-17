---
title: Различия свойств между Azure AD Graph и Microsoft Graph
description: Описывает различия свойств между ресурсами (сущностями) Azure AD Graph и Microsoft Graph, чтобы помочь в переносе приложений соответствующим образом.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 38d151fa5c6510f3b8279646db7ebe0c37c4926a
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705949"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия свойств между Azure AD Graph и Microsoft Graph

Эта статья является частью *шага 1. Обзор различий API* в [процессе переноса приложений.](migrate-azure-ad-graph-planning-checklist.md)

В общем случае лучший способ сравнить API Azure AD Graph с Microsoft Graph — сравнить общие метаданные для каждой службы, особенно описания ресурсов:

- [Метаданные Azure AD Graph](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Метаданные бета-версии Microsoft Graph](https://graph.microsoft.com/beta/$metadata)
- [Метаданные Microsoft Graph 1.0](https://graph.microsoft.comv/1.0/$metadata)

Здесь выделяются различия свойств между ресурсами. Если свойство не отображается в этом списке, оно уже доступно в версии [1.0](/graph/api/overview?view=graph-rest-1.0) Microsoft Graph с точно таким же именем, как в Azure AD Graph.

Так как пользователи и группы используются так часто, эти ресурсы отображаются первыми.  Другие ресурсы отображаются в алфавитном порядке.

## <a name="user-property-differences"></a>Различия в свойствах пользователей

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br>свойство|Примечания|
|---|---|---|
| **deletedTimestamp**| beta &nbsp; - &nbsp; **deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **faxNumber** <br> v1.0 &nbsp; - &nbsp; **faxNumber** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | &nbsp; - &nbsp; _Бета-версия недоступна_ <br> V1.0 &nbsp; - &nbsp; _Недоступна_ | API защиты [идентификации](/graph/api/resources/identityprotection-root?view=graph-rest-beta) Microsoft Graph предоставляет более сложные функции. |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | &nbsp; - &nbsp; **бета-версия mobilePhone** <br> v1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | &nbsp; - &nbsp; _Бета-версия недоступна_ <br> V1.0 &nbsp; - &nbsp; _Недоступна_ | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство, описывающие все ошибки, связанные с подготовкаю AD Connect |
| **refreshTokensValidFromDateTime** | beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v1.0 &nbsp; - &nbsp; **signinSessionsValidFromDateTime** | |
| **signinNames** | beta &nbsp; - &nbsp; **identities/signInType** <br> удостоверения &nbsp; - v1.0/signInType; &nbsp;  | Это свойство теперь является частью ресурса [objectIdentity.](/graph/api/resources/objectIdentity?view=graph-rest-1.0)|
| **telephoneNumber** | &nbsp; - &nbsp; **бета-версии бизнес-телефонов** <br> v1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | &nbsp; - &nbsp; **бета-версия фотографии,** фотографии <br> v1.0 &nbsp; - &nbsp; **photo**, photos | Фотография эскиза Azure AD недоступна в Microsoft Graph.  Вместо этого [используйте API](/graph/api/resources/profilephoto?view=graph-rest-1.0) фотографий. |
| **userIdentities** | &nbsp; - &nbsp; **бета-версии удостоверений** <br> Удостоверения v1.0 &nbsp; - &nbsp;  | Дополнительные [сведения см. в](/graph/api/resources/objectIdentity?view=graph-rest-1.0) типе ресурса objectIdentity.|
| **userState** | beta &nbsp; - &nbsp; **externalUserState** <br> v1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>Различия свойств группы

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime**<br>v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **provisioningErrors** | &nbsp; - &nbsp; _Бета-версия недоступна_ <br> V1.0 &nbsp; - &nbsp; _Недоступна_ | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство, описывающие все ошибки, связанные с подготовкаю AD Connect |

## <a name="application-property-differences"></a>Различия свойств приложения

| Azure AD Graph <br>Свойство (v1.6) | Microsoft Graph<br> свойство                                                                                                                          | Примечания                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | beta &nbsp; - &nbsp; **api/acceptMappedClaims** <br> API &nbsp; - v1.0/acceptMappedClaims &nbsp;                                                        | acceptMappedClaims теперь является частью нового ресурса api.                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | beta &nbsp; - &nbsp; **signInAudience** <br> v1.0 &nbsp; - &nbsp; **signInAudience**                                                                      |                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство является неподготовленным.                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp; - &nbsp; **web/homePageUrl** <br> v1.0 &nbsp; - &nbsp; **web/homePageUrl**                                                                     | домашняя страницу теперь является частью нового веб-ресурса.                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | Сведения о &nbsp; - &nbsp; **бета-версии** <br> Сведения о v1.0 &nbsp; - &nbsp;                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | beta &nbsp; - &nbsp; **api/knownClientApplications** <br> API &nbsp; - v1.0/knownClientApplications &nbsp;                                                | KnownClientApplications теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp; - &nbsp; **web/logoutUrl** <br> v1.0 &nbsp; - &nbsp; **web/logoutUrl**                                                                         | logoutUrl теперь является частью веб-ресурса.                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp; - &nbsp; **info/logoUrl** <br> v1.0 &nbsp; - &nbsp; **info/logoUrl**                                                                           | logoUrl теперь является частью нового информационного ресурса.                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | Логотип &nbsp; - &nbsp; **бета-версии** <br> Логотип v1.0 &nbsp; - &nbsp;                                                                                             |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**         | Переименован и теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance** | Переименован и теперь является частью нового ресурса implicitGrantSettings.                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство является неподготовленным.                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | beta &nbsp; - &nbsp; **api/oauth2PermissionScopes**<br> &nbsp; - &nbsp; **api/oauth2PermissionScopes** v1.0                                                  | Переименован и теперь является частью нового ресурса API.                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp; - &nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp; - &nbsp; **isFallbackPublicClient**                                                      | Теперь это свойство имеет новое значение, которое содержит общедоступные &nbsp; - &nbsp; параметры клиента, такие как redirectUris. Определение того, является ли приложение общедоступным или конфиденциальным клиентом, теперь делается автоматически, при этом свойство isFallbackPublicClient обработчик одного специального случая, которое не может быть определено автоматически. |
| **recordConsentConditions**        | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _недоступна_                                                                              | Это свойство является неподготовленным.                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | beta &nbsp; - &nbsp; **web/redirectUris**, **publicClient/redirectUris**<br> v1.0 &nbsp; - &nbsp; **web/redirectUris**, **publicClient/redirectUris**        | Как и переименование, redirectUris теперь является частью новых веб-ресурсов и ресурсов publicClient. Это позволяет разработчикам использовать определенные IS для своих веб-клиентов и общедоступных клиентов (например, установленное приложение на настольном устройстве).                                                                                           |
| **samlMetadataUrl**                | &nbsp; - &nbsp; _Бета-версия пока недоступна_  <br> V1.0 &nbsp; - &nbsp; _Пока не доступен_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | &nbsp; - &nbsp; _Бета-версия недоступна_  <br> V1.0 &nbsp; - &nbsp; _Недоступна_                                                                          | Это свойство является неподготовленным, но планируется для servicePrincipal.                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>Отличия AppRoleAssignment

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **creationTimestamp** | beta &nbsp; - &nbsp; **creationTimestamp** <br> v1.0 &nbsp; - &nbsp; **createdDateTime** | |
| **id** | beta &nbsp; - &nbsp; **appRoleId** <br> v1.0 &nbsp; - &nbsp; **appRoleId** | |

## <a name="contact-property-differences"></a>Различия свойств контакта

Ресурс контакта Azure AD Graph переименован в orgContact в Microsoft Graph.  Ниже различия между свойствами.

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **city** | &nbsp; - &nbsp; **бета-адреса (город)** <br> Адреса 1.0 &nbsp; - &nbsp; **(город)**  | Свойство city является частью коллекции ресурсов addresses. |
| **country** | beta &nbsp; - &nbsp; **addresses** &nbsp; **(countryOrRegion)**<br> адреса v1.0 &nbsp; - &nbsp;  &nbsp; **(countryOrRegion)**  | Свойство countryOrRegion является частью коллекции ресурсов addresses. |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | &nbsp; - &nbsp; **бета-версии** &nbsp; **телефонов (businessFax)** <br> Телефоны v1.0 &nbsp; - &nbsp;  &nbsp; **(businessFax)** | Теперь входит в коллекцию телефонов, которая поддерживает мобильные устройства, бизнес и businessFax. |
| **physicalDeliveryOfficeName** | beta &nbsp; - &nbsp; **officeLocation** <br> v1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | beta &nbsp; - &nbsp; **addresses** &nbsp; **(postalCode)**<br> адреса v1.0 &nbsp; - &nbsp;  &nbsp; **(postalCode)** | Свойство postalCode является частью коллекции ресурсов addresses. |
| **provisioningErrors** | &nbsp; - &nbsp; бета-версия недоступна <br> V1.0 &nbsp; - &nbsp; недоступна | Это свойство и его сведения неподготовлены.  Однако в **onPremisesProvisioningErrors** можно найти новое свойство, описывающие все ошибки, связанные с подготовкаю AD Connect. В настоящее время эта версия доступна только в бета-версии. |
| **sipProxyAddress** |  beta &nbsp; - &nbsp; **imAddresses**<br> 1.0 &nbsp; - &nbsp; **imAddresses**  | |
| **state** | &nbsp; - &nbsp; **бета-адреса** &nbsp; **(состояние)**<br> Адреса v1.0 &nbsp; - &nbsp;  &nbsp; **(состояние)**  | Свойство state является частью коллекции ресурсов addresses. |
| **streetAddress** | beta &nbsp; - &nbsp; **addresses** &nbsp; **(street)**<br> адреса 1.0 &nbsp; - &nbsp;  &nbsp; **(street)**  | Свойство street является частью коллекции ресурсов addresses. |
| **telephoneNumber** | &nbsp; - &nbsp; **бета-версии** &nbsp; **телефонов (бизнес)** <br> Телефоны v1.0 &nbsp; - &nbsp;  &nbsp; **(бизнес)** | Теперь входит в коллекцию телефонов, которая поддерживает мобильные устройства, бизнес и businessFax. |
| **thumbnailPhoto** | &nbsp; - &nbsp; _Бета-версия &nbsp; пока &nbsp; недоступна_&nbsp;<br> V1.0 &nbsp; - &nbsp; _Пока не доступен_ | |

## <a name="contract-property-differences"></a>Различия в свойствах контракта

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **customerContextId** | beta &nbsp; - &nbsp; **customerId** <br> v1.0 &nbsp; - &nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>Различия свойств устройства

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **approximateLastLogonTimestamp** | beta &nbsp; - &nbsp; **approximateLastSignInDateTime** <br> v1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | beta &nbsp; - &nbsp; **complianceExpirationDateTime** <br> v1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  beta &nbsp; - &nbsp; **deviceVersion** <br> v1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | beta &nbsp; - &nbsp; **operatingSystem** <br> v1.0 &nbsp; - &nbsp; **operatingSystem** |  |
| **deviceOSVersion** | beta &nbsp; - &nbsp; **operatingSystemVersion** <br> v1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta &nbsp; - &nbsp; **physicalIds** <br> physicalIds v1.0 &nbsp; - &nbsp;  |  |
| **deviceTrustType** | beta &nbsp; - &nbsp; **trustType** <br> v1.0 &nbsp; - &nbsp; **trustType** |  |
| **dirSyncEnabled** |  beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>Различия свойств DirectoryObjectReference

Ресурс directoryObjectReference Azure AD Graph переименован в directoryObjectPartnerReference в Microsoft Graph.  Ниже различия между свойствами.

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **externalContextId** | beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>Различия свойств домена

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **name** | &nbsp; - &nbsp; **бета-версия** <br> v1.0 &nbsp; - &nbsp; **id** | В Microsoft Graph уникальный идентификатор (идентификатор) содержит доменное имя; свойство `name` не существует. |
| **forceDeleteState** |  состояние &nbsp; - &nbsp; **бета-версии** <br> Состояние 1.0 &nbsp; - &nbsp;  | В Azure AD Graph существуют отдельные свойства forceDelete и состояния домена.  В Microsoft Graph все состояния домена обрабатываются свойством state. |
| **isDefaultForCloudRedirections** | &nbsp; - &nbsp; _Бета-версия &nbsp; пока &nbsp; недоступна_&nbsp;<br> V1.0 &nbsp; - &nbsp; _Пока не доступен_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>Отличия свойств OAuth2PermissionsGrant

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **expiryTime** | beta &nbsp; - &nbsp; **expiryTime** <br> Удалена v1.0 &nbsp; - &nbsp;  | Это свойство не используется и удаляется в Microsoft Graph 1.0. |
| **startTime** | beta &nbsp; - &nbsp; **startTime** <br> Удалена v1.0 &nbsp; - &nbsp;   | Это свойство не используется и удаляется в Microsoft Graph 1.0. |

## <a name="policy-property-differences"></a>Различия свойств политики

В Microsoft Graph существуют именованные типы политик (например, tokenIssuancePolicy или tokenLifetimePolicy), а не универсальный тип ресурса политики. Дополнительные сведения доступны в [обзоре политики.](/graph/api/resources/policy-overview?view=graph-rest-1.0)

## <a name="serviceendpoint-property-differences"></a>Различия в свойствах ServiceEndpoint

Ресурс ServiceEndpoint Azure AD Graph переименован в конечную точку в Microsoft Graph.

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **serviceId** | beta &nbsp; - &nbsp; **providerId**<br> v1.0 &nbsp; - &nbsp; **providerId** | |
| **serviceName** | beta &nbsp; - &nbsp; **providerName**<br> v1.0 &nbsp; - &nbsp; **providerName** | |
| **resourceId** | beta &nbsp; - &nbsp; **providerResourceId**<br> v1.0 &nbsp; - &nbsp; **providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>Различия свойств ServicePrincipal

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **appOwnerTenantId** | beta &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | Переименовано. |
| **informationalUrls**| Сведения о &nbsp; - &nbsp; **бета-версии** <br> Сведения о v1.0 &nbsp; - &nbsp;  | |
| **oauth2Permissions** | beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | Переименовано. |
| **preferredTokenSigningKeyEndDateTime** | &nbsp; - &nbsp; _Бета-версия пока недоступна_ <br> V1.0 &nbsp; -  _Пока не доступен_ | |
| **signInAudience** | &nbsp; - &nbsp; _Бета-версия пока недоступна_ <br> V1.0 &nbsp; -  _Пока не доступен_ | |
| **serviceEndpoints** | &nbsp; - &nbsp; **Конечная точка бета-версии** <br> Конечная точка &nbsp; - &nbsp;  v1.0 | Переименовано. |

## <a name="tenantdetails-property-differences"></a>Различия свойств TenantDetails

Ресурс TenantDetails Azure AD Graph переименован в организацию в Microsoft Graph.  Ниже различия между свойствами.

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **companyLastDirSyncTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | &nbsp; - &nbsp; _Бета-версия недоступна_ <br> V1.0 &nbsp; - &nbsp; _Недоступна_ | Это свойство и его сведения неподготовлены.|
| **telephoneNumber** | &nbsp; - &nbsp; **бета-версии бизнес-телефонов** <br> v1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Различия свойств TrustedCasForPasswordlessAuth

Ресурс Azure AD Graph TrustedCasForPasswordlessAuth переименован в [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)и доступен только в конечной точке бета-версии Microsoft Graph. Различия между свойствами не существуют; Однако существуют различия в типе ресурса **certificateAuthority,** используемом **свойством certificateAuthorities.**

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

Сертификат CertificateAuthorityInformation Azure AD Graph переименован в **certificateAuthority** в Microsoft Graph. Ниже различия между свойствами.

|Azure AD Graph <br>Свойство (v1.6) |Microsoft Graph<br> свойство|Примечания|
|---|---|---|
| **authorityType** | beta &nbsp; - &nbsp; **isRootAuthority**<br> v1.0 &nbsp; - &nbsp; **isRootAuthority** | Тип этого свойства также изменился на boolean. Ранее этому свойству приходилось устанавливать "RootAuthority" или "IntermediateAuthority". Установка для нового свойства **true** эквивалентна свойству RootAuthority. |
| **crlDistributionPoint** | beta &nbsp; - &nbsp; **certificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | &nbsp; - &nbsp; **бета-сертификат** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | beta &nbsp; - &nbsp; **issuer**<br> Issuer v1.0 &nbsp; - &nbsp;  | |
| **trustedIssuerSki** | beta &nbsp; - &nbsp; **issuerSki**<br> IssuerSki 1.0 &nbsp; - &nbsp;  | |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях методов](migrate-azure-ad-graph-method-differences.md) между Azure AD Graph и Microsoft Graph.
- Еще раз [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.

