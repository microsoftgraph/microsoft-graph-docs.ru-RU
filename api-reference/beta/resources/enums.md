---
title: Значения перечисления
description: Значения перечисления Microsoft Graph
doc_type: enumPageType
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: a064058b666f7b5709fed96a53b83c6eb3d2c77d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446366"
---
# <a name="enum-values"></a>Значения перечисления

Пространство имен: microsoft.graph

### <a name="decisionitemprincipalresourcemembershiptype-values"></a>Значения decisionItemPrincipalResourceMembershipType 

|Member|
|:---|
|Прямой|
|Косвенные|
|unknownFutureValue|

### <a name="signinfrequencyauthenticationtype-values"></a>Значения signInFrequencyAuthenticationType

|Member|
|:---|
|primaryAndSecondaryAuthentication|
|secondaryAuthentication|
|unknownFutureValue|

### <a name="signinfrequencyinterval-values"></a>Значения signInFrequencyInterval

|Member|
|:---|
|timeBased|
|Everytime|

#### <a name="authenticationprotocol-values"></a>Значения authenticationProtocol

|Member|
|:---|
|wsFed|
|Saml|
|unknownFutureValue|

#### <a name="federatedidpmfabehavior-values"></a>Значения federatedIdpMfaBehavior
|Member|
|:---|
|acceptIfMfaDoneByFederatedIdp|
|enforceMfaByFederatedIdp|
|rejectMfaByFederatedIdp|
|unknownFutureValue|

#### <a name="promptloginbehavior-values"></a>Значения promptLoginBehavior
|Member|
|:---|
|translateToFreshPasswordAuthentication|
|nativeSupport|
|отключено|
|unknownFutureValue|

### <a name="bookingsavailabilitystatus-values"></a>Значения bookingsAvailabilityStatus

|Member|
|:-----|
|доступен|
|Занят|
|slotsAvailable|
|outOfOffice|
|unknownFutureValue|

### <a name="accesspackagecustomextensionhandlerstatus-values"></a>значения accessPackageCustomExtensionHandlerStatus 

|Member|
|:---|
|requestSent|
|requestReceived|
|unknownFutureValue|

### <a name="accesspackagecustomextensionstage-values"></a>Значения accessPackageCustomExtensionStage 

|Member|
|:---|
|assignmentRequestCreated|
|assignmentRequestApproved|
|assignmentRequestGranted|
|assignmentRequestRemoved|
|assignmentFourteenDaysBeforeExpiration|
|assignmentOneDayBeforeExpiration|
|unknownFutureValue|

### <a name="accessreviewhistorystatus-values"></a>Значения accessReviewHistoryStatus

| Member|
|:-----------------|
|done|
|Inprogress|
|error|
|Запрошенный|
|unknownFutureValue|

### <a name="accessreviewhistorydecisionfilter-values"></a>Значения accessReviewHistoryDecisionFilter

| Member|
|:-----------------|
|Утвердить|
|Отрицать|
|notReviewed|
|dontKnow|
|notNotified|
|unknownFutureValue|


### <a name="accessreviewhistorystatus-values"></a>Значения accessReviewHistoryStatus

|Member|
|:---|
|done|
|Inprogress|
|error|
|Запрошенный|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargetconfigurationaccesstype-values"></a>Значения crossTenantAccessPolicyTargetConfigurationAccessType

|Member|
|:---|
|Разрешены|
|Заблокирован|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargettype-values"></a>Значения crossTenantAccessPolicyTargetType

|Member|
|:---|
|пользователь;|
|group|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>значения accessPackageFilterByCurrentUserOptions

|Member|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="usersigninrecommendationscope-values"></a>Значения userSignInRecommendationScope 

|Member|
|:---|
|клиент|
|приложение|

### <a name="incomingtokentype-values"></a>Значения incomingTokenType 

|Member|
|:---|
|Нет|
|primaryRefreshToken|
|saml11|
|saml20|
|unknownFutureValue|
|remoteDesktopToken|

### <a name="protocoltype-values"></a>Значения protocolType 

|Member|
|:---|
|Нет|
|oAuth2|
|ropc|
|wsFederation|
|saml20|
|deviceCode|
|unknownFutureValue|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>значения accessReviewInstanceDecisionItemFilterByCurrentUserOptions 

|Member|
|:---|
|Рецензент|
|unknownFutureValue|

### <a name="accessreviewstagefilterbycurrentuseroptions-values"></a>Значения accessReviewStageFilterByCurrentUserOptions 

|Member|
|:---|
|Рецензент|
|unknownFutureValue|

### <a name="continuousaccessevaluationmode-values"></a>значения continuousAccessEvaluationMode 

|Member|
|:---|
|strictEnforcement|
|отключено|
|unknownFutureValue|

### <a name="multifactorauthconfiguration-values"></a>Значения multiFactorAuthConfiguration

| Элемент             | Значение | Описание |
|:-------------------|:------| :------|
| notRequired        | 0     | Для завершения регистрации устройства пользователю не требуется многофакторная проверка подлинности.|
| обязательно           | 1     | Для завершения регистрации устройства пользователю требуется многофакторная проверка подлинности.|
| unknownFutureValue | 2     | Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="policyscope-values"></a>Значения policyScope

| Элемент             | Значение | Описание |
|:-------------------|:------| :------|
| Нет               | 0     | Политика не применяется ни к пользователям, ни к группам в организации. |
| все                | 1     | Политика применяется ко всем пользователям и группам в организации. Значение по умолчанию. |
| Выбранного           | 2     | Политика применяется к определенным пользователям или группам в организации. |
| unknownFutureValue | 3     | Значение sentinel для развиваемого перечисления. Не следует использовать. |

### <a name="appcredentialrestrictiontype-values"></a>Значения appCredentialRestrictionType

| Member                 |
| :--------------------- |
| passwordAddition       |
| passwordLifetime       |
| symmetricKeyAddition   |
| symmetricKeyLifetime   |
| customPasswordAddition |
| unknownFutureValue     |

### <a name="appkeycredentialrestrictiontype-values"></a>Значения appKeyCredentialRestrictionType

|Member|
|:-----|
|asymmetricKeyLifetime|
|unknownFutureValue|

### <a name="synchronizationsecret-values"></a>Значения synchronizationSecret

|Member|
|:----|
|Нет|
|UserName|
|Password|
|SecretToken|
|AppKey|
|BaseAddress|
|ClientIdentifier|
|ClientSecret|
|SingleSignOnType|
|Песочнице|
|Url|
|Домен|
|ConsumerKey|
|ConsumerSecret|
|TokenKey|
|TokenExpiration|
|Oauth2AccessToken|
|Oauth2AccessTokenCreationTime|
|Oauth2RefreshToken|
|SyncAll|
|Instancename|
|Oauth2ClientId|
|Oauth2ClientSecret|
|CompanyId|
|UpdateKeyOnSoftDelete|
|SynchronizationSchedule|
|SystemOfRecord|
|SandboxName|
|EnforceDomain|
|SyncNotificationSettings|
|SkipOutOfScopeDeletions|
|Oauth2AuthorizationCode|
|Oauth2RedirectUri|
|ApplicationTemplateIdentifier|
|Сервер|
|PerformInboundEntitlementGrants|
|HardDeletesEnabled|
|SyncAgentCompatibilityKey|
|SyncAgentADContainer|
|ValidateDomain|
|TestReferences|

### <a name="filtermode-values"></a>Значения filterMode

|Member|
|:---|
|Включают|
|Исключить|

### <a name="lifecycleeventtype-values"></a>Значения lifecycleEventType

|Member|
|:---|
|Пропустил|
|subscriptionRemoved|
|reauthorizationRequired|

### <a name="changetype-values"></a>Значения changeType

|Member|
|:---|
|создано|
|Обновлено|
|deleted|


### <a name="countrylookupmethodtype-values"></a>Значения countryLookupMethodType

|Member|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="approvalstate-values"></a>Значения approvalState

|Member|
|:---|
|Ожидающие|
|Утвержденных|
|denied|
|Прервана|
|Отменен|

### <a name="rolesummarystatus-values"></a>Значения roleSummaryStatus

|Member|
|:---|
|Хорошо|
|Плохо|

### <a name="datapolicyoperationstatus-values"></a>Значения dataPolicyOperationStatus

|Member|
|:---|
|notStarted|
|Запущена|
|complete|
|Сбой при|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>Значения conditionalAccessClientApp

|Member|
|:---|
|все|
|Обозреватель|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|Других|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>Значения consentRequestFilterByCurrentUserOptions

|Member|
|:---|
|Рецензент|
|unknownFutureValue|

### <a name="attributetype-values"></a>Значения attributeType

|Member|
|:---|
|String|
|Целое число|
|Справочные материалы|
|Binary|
|Логическое|
|DateTime|

### <a name="mutability-values"></a>значения изменяемости

|Member|
|:---|
|Для чтения и записи|
|ReadOnly|
|Неизменяемым|
|WriteOnly|

### <a name="directorydefinitiondiscoverabilities-values"></a>Значения directoryDefinitionDiscoverabilities

|Member|
|:---|
|Нет|
|AttributeNames|
|AttributeDataTypes|
|AttributeReadOnly|
|ReferenceAttributes|
|UnknownFutureValue|

### <a name="connectorgroupregion-values"></a>Значения connectorGroupRegion

|Member|
|:---|
|Nam|
|Eur|
|Aus|
|Азии|
|Ind|
|unknownFutureValue|

### <a name="connectorgrouptype-values"></a>Значения connectorGroupType

|Member|
|:---|
|applicationProxy|

### <a name="onpremisespublishingtype-values"></a>Значения onPremisesPublishingType

|Member|
|:---|
|applicationProxy|
|exchangeOnline|
|authentication|
|Подготовки|
|intunePfx|
|oflineDomainJoin|
|unknownFutureValue|

### <a name="agentstatus-values"></a>Значения agentStatus

|Member|
|:---|
|Активных|
|Неактивные|

### <a name="connectorstatus-values"></a>Значения connectorStatus

|Member|
|:---|
|Активных|
|Неактивные|

### <a name="calltype-values"></a>Значения callType

|Member|
|:---|
|unknown|
|groupCall|
|peerToPeer|
|unknownFutureValue|

### <a name="tone-values"></a>значения звукового сигнала

|Member|
|:---|
|tone0|
|tone1|
|tone2|
|tone3|
|тон4|
|tone5|
|тон6|
|тон7|
|tone8|
|tone9|
|Звездочные|
|Фунт|
|a|
|b|
|c|
|d|
|Вспышки|

### <a name="callstate-values"></a>Значения callState

|Member|
|:---|
|Входящих|
|Создания|
|Звон|
|Установлено|
|Держать|
|Передачи|
|transferAccepted|
|Перенаправление|
|Прекращения|
|Прекращено|

### <a name="routingpolicy-values"></a>Значения routingPolicy

|Member|
|:---|
|Нет|
|noMissedCall|
|disableForwardingExceptPhone|
|disableForwarding|
|preferSkypeForBusiness|
|unknownFutureValue|

### <a name="meetingcapabilities-values"></a>Значения meetingCapabilities

|Member|
|:---|
|questionAndAnswer|
|unknownFutureValue|

### <a name="onlinemeetingrole-values"></a>Значения onlineMeetingRole

|Member|
|:---|
|attendee|
|Ведущий|
|Производитель|
|unknownFutureValue|

### <a name="autoadmitteduserstype-values"></a>Значения autoAdmittedUsersType

|Member|
|:---|
|everyoneInCompany|
|Все|

### <a name="mediastate-values"></a>Значения mediaState

|Member|
|:---|
|Активных|
|Неактивные|
|unknownFutureValue|

### <a name="calldirection-values"></a>Значения callDirection

|Member|
|:---|
|Входящих|
|Исходящих|

### <a name="modality-values"></a>значения модальности

|Member|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="kerberossignonmappingattributetype-values"></a>Значения kerberosSignOnMappingAttributeType

|Member|
|:---|
|userPrincipalName.|
|onPremisesUserPrincipalName|
|userPrincipalUsername|
|onPremisesUserPrincipalUsername|
|onPremisesSAMAccountName|

### <a name="externalauthenticationtype-values"></a>Значения externalAuthenticationType

|Member|
|:---|
|passthru|
|aadPreAuthentication|

### <a name="recipientscopetype-values"></a>Значения recipientScopeType
|Member|
|:---|
|Нет|
|Внутренние|
|Внешних|
|externalPartner|
|externalNonPartner|

### <a name="appliedconditionalaccesspolicyresult-values"></a>Значения appliedConditionalAccessPolicyResult

|Member|
|:---|
|success|
|Сбоя|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|
|reportOnlySuccess|
|reportOnlyFailure|
|reportOnlyNotApplied|
|reportOnlyInterrupted|


### <a name="microsoftauthenticatorauthenticationmode-values"></a>Значения microsoftAuthenticatorAuthenticationMode



|Member|
|:---|
|любой|
|Нажмите|
|deviceBasedPush|


### <a name="authenticationmethodfeature-values"></a>Значения authenticationMethodFeature

|Member|
|:---|
|ssprRegistered|
|ssprEnabled|
|ssprCapable|
|passwordlessCapable|
|mfaCapable|


### <a name="authmethodstype-values"></a>Значения authMethodsType

|Member|
|:---|
|email|
|mobileSMS|
|mobilePhone;|
|officePhone|
|securityQuestion|
|appNotification|
|appNotificationCode|
|appNotificationAndCode|
|appPassword|
|Фидо|
|alternateMobilePhone|
|mobilePhoneAndSMS|
|unknownFutureValue|


### <a name="defaultmfamethodtype-values"></a>Значения defaultMfaMethodType 



|Member|
|:---|
|Нет|
|mobilePhone;|
|alternateMobilePhone|
|officePhone|
|microsoftAuthenticatorPush|
|softwareOneTimePasscode|
|unknownFutureValue|


### <a name="clientcredentialtype-values"></a>Значения clientCredentialType 



|Member|
|:---|
|Нет|
|clientSecret|
|clientAssertion|
|federatedIdentityCredential|
|managedIdentity|
|certificate|
|unknownFutureValue|


### <a name="azureadlicensetype-values"></a>Значения azureADLicenseType

|Member|
|:---|
|Нет|
|Бесплатный|
|Основные|
|PremiumP1|
|PremiumP2|
|unknownFutureValue|

### <a name="conditionalaccessconditions-values"></a>Значения conditionalAccessConditions

|Member|
|:---|
|Нет|
|приложение|
|users|
|devicePlatform|
|расположение;|
|clientType|
|signInRisk|
|userRisk|
|time|
|deviceState|
|Клиента|
|ipAddressSeenByAzureAD|
|ipAddressSeenByResourceProvider|
|unknownFutureValue|
|servicePrincipals|
|servicePrincipalRisk|

### <a name="conditionalaccessstatus-values"></a>Значения conditionalAccessStatus

|Member|
|:---|
|success|
|Сбоя|
|notApplied|
|unknownFutureValue|

### <a name="featuretype-values"></a>Значения featureType

|Member|
|:---|
|Регистрации|
|сброс|
|unknownFutureValue|

### <a name="grouptype-values"></a>Значения groupType

|Member|
|:---|
|unifiedGroups|
|AzureAD|
|unknownFutureValue|

### <a name="includeduserroles-values"></a>Значения includedUserRoles

|Member|
|:---|
|все|
|privilegedAdmin|
|Администратора|
|пользователь;|
|unknownFutureValue|

### <a name="includedusertypes-values"></a>Значения includedUserTypes

|Member|
|:---|
|все|
|член|
|Гостевой|
|unknownFutureValue|

### <a name="initiatortype-values"></a>Значения initiatorType

|Member|
|:---|
|пользователь;|
|приложение|
|system|
|unknownFutureValue|

### <a name="migrationstatus-values"></a>Значения migrationStatus

|Member|
|:---|
|Готов|
|needsReview|
|additionalStepsRequired|
|unknownFutureValue|

### <a name="networktype-values"></a>Значения networkType

|Member|
|:---|
|Интрасети|
|Экстрасети|
|namedNetwork|
|Доверенных|
|unknownFutureValue|

### <a name="operationresult-values"></a>Значения operationResult

|Member|
|:---|
|success|
|Сбоя|
|timeout|
|unknownFutureValue|

### <a name="provisioningresult-values"></a>Значения provisioningResult

|Member|
|:---|
|success|
|Сбоя|
|Пропущен|
|warning|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>Значения provisioningStepType

|Member|
|:---|
|Импорт|
|Области|
|Соответствующие|
|Обработки|
|referenceResolution|
|Экспорт|
|unknownFutureValue|

### <a name="registrationauthmethod-values"></a>Значения registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone;|
|officePhone|
|securityQuestion|
|appNotification|
|AppCode|
|alternateMobilePhone|
|Фидо|
|appPassword|
|unknownFutureValue|

### <a name="registrationstatustype-values"></a>Значения registrationStatusType

|Member|
|:---|
|Зарегистрированных|
|включено|
|Способны|
|mfaRegistered|
|unknownFutureValue|


### <a name="signinidentifiertype-values"></a>Значения signInIdentifierType 

|Member|
|:---|
|userPrincipalName.|
|phoneNumber|
|proxyAddress|
|qrCode|
|onPremisesUserPrincipalName|
|unknownFutureValue|


### <a name="signinusertype-values"></a>Значения signInUserType 

|Member|
|:---|
|член|
|Гостевой|
|unknownFutureValue|

### <a name="requirementprovider-values"></a>Значения requirementProvider 


|Member|
|:---|
|пользователь;|
|Запрос|
|servicePrincipal|
|v1ConditionalAccess|
|multiConditionalAccess|
|tenantSessionRiskPolicy|
|accountCompromisePolicies|
|v1ConditionalAccessDependency|
|v1ConditionalAccessPolicyIdRequested|
|mfaRegistrationRequiredByIdentityProtectionPolicy|
|baselineProtection|
|mfaRegistrationRequiredByBaselineProtection|
|mfaRegistrationRequiredByMultiConditionalAccess|
|enforcedForCspAdmins|
|securityDefaults|
|mfaRegistrationRequiredBySecurityDefaults|
|proofUpCodeRequest|
|crossTenantOutboundRule|
|gpsLocationCondition|
|riskBasedPolicy|
|unknownFutureValue|


### <a name="riskdetail-values"></a>Значения riskDetail

|Member|
|:---|
|Нет|
|Внутренние|
|Внешних|
|externalPartner|
|externalNonPartner|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninCompromised|
|hidden|
|adminConfirmedUserComprommed|
|unknownFutureValue|
|adminConfirmedServicePrincipalComprommed|
|adminDismissedAllRiskForServicePrincipal|


<!-- maintenance comment: Do not delete enum delcaration for riskEventType until all properties of this type are marked as deleted. Dec 28, 2021: Pending eventTypes (in riskUserActivity) and riskType (in riskDetection)-->
### <a name="riskeventtype-values"></a>Значения riskEventType

|Member|
|:---|
|unlikelyTravel|
|anonymizedIPAddress|
|maliciousIPAddress|
|unfamiliarFeatures|
|malwareInfectedIPAddress|
|suspiciousIPAddress|
|leakedCredentials|
|investigationsThreatIntelligence|
|Универсальный|
|adminConfirmedUserComprommed|
|mcasImpossibleTravel|
|mcasSuspiulationInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="usageauthmethod-values"></a>Значения usageAuthMethod

|Member|
|:---|
|email|
|mobileSMS|
|mobileCall|
|officePhone|
|securityQuestion|
|appNotification|
|AppCode|
|alternateMobileCall|
|Фидо|
|appPassword|
|unknownFutureValue|

### <a name="authenticationmethodkeystrength-values"></a>Значения authenticationMethodKeyStrength

|Member|
|:---|
|Нормальной|
|Слабым|
|unknown|

### <a name="authenticationcontextdetail-values"></a>Значения authenticationContextDetail

|Member|
|:---|
|Обязательный|
|previouslyИмя|
|notApplicable|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>значения educationAddedStudentAction

|Member|
|:---|
|Нет|
|assignIfOpen|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>значения educationAddToCalendarOptions
|Member|
|:---|
|Нет|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationassignmentstatus-values"></a>значения educationAssignmentStatus
|Member|
|:---|
|Проект|
|Опубликовано|
|Назначен|
|unknownFutureValue|

### <a name="educationsubmissionstatus-values"></a>значения educationSubmissionStatus
|Member|
|:---|
|Работает|
|Представлены|
|Выпущен|
|Возвращены|
|unknownFutureValue|
|Переназначить|

### <a name="educationfeedbackresourceoutcomestatus-values"></a>Значения educationFeedbackResourceOutcomeStatus
|Member|
|:---|
|notPublished|
|pendingPublish|
|Опубликовано|
|failedPublish|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>Значения externalEmailOtpState

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="expirationrequirement-values"></a>Значения expirationRequirement

|Member|
|:---|
|rememberMultifactorAuthenticationOnTrustedDevices|
|tenantTokenLifetimePolicy|
|audienceTokenLifetimePolicy|
|signInFrequencyPeriodicReauthentication|
|ngcMfa|
|signInFrequencyEveryTime|
|unknownFutureValue|


### <a name="replyrestriction-values"></a>Значения replyRestriction

| Member
|:--------------
| Все
| authorAndModerators
| unknownFutureValue

### <a name="usernewmessagerestriction-values"></a>Значения userNewMessageRestriction

| Member
|:--------------
|Все
|everyoneExceptGuests
|Модераторов
|unknownFutureValue

### <a name="volumetype-values"></a>Значения volumeType

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="allowedaudiences-values"></a>значения allowedAudiences

|Member|
|:---|
|me|
|Семьи|
|contacts|
|groupMembers|
|organization;|
|federatedOrganizations|
|Все|
|unknownFutureValue|

### <a name="attestationlevel-values"></a>Значения attestationLevel

|Member|
|:---|
|аттестовка|
|notAttested|
|unknownFutureValue|

### <a name="emailtype-values"></a>Значения emailType

|Member|
|:---|
|unknown|
|work|
|personal|
|Главной|
|Других|

### <a name="authenticationmethodsigninstate-values"></a>Значения authenticationMethodSignInState

|Member|
|:---|
|notSupported|
|notAllowedByPolicy|
|notEnabled|
|phoneNumberNotUnique|
|Готов|
|notConfigured|
|unknownFutureValue|

### <a name="authenticationphonetype-values"></a>Значения authenticationPhoneType

|Member|
|:---|
|мобильный|
|alternateMobile|
|Офис|
|unknownFutureValue|


### <a name="authenticationmethodtargettype-values"></a>Значения authenticationMethodTargetType

|Member|
|:---|
|пользователь;|
|group|

### <a name="authenticationmethodstate-values"></a>Значения authenticationMethodState

|Member|
|:---|
|включено|
|отключено|

### <a name="fido2restrictionenforcementtype-values"></a>Значения fido2RestrictionEnforcementType

|Member|
|:---|
|Позволяют|
|Блок|
|unknownFutureValue|

### <a name="x509certificateauthenticationmode-values"></a>Значения x509CertificateAuthenticationMode
|Member|
|:---|
|x509CertificateSingleFactor|
|x509CertificateMultiFactor|
|unknownFutureValue|

### <a name="x509certificateruletype-values"></a>Значения x509CertificateRuleType
|Member|
|:---|
|issuerSubject|
|policyOID|
|unknownFutureValue|

### <a name="anniversarytype-values"></a>Значения anniversaryType

|Member|
|:---|
|birthday;|
|Свадебные|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>Значения skillProficiencyLevel

|Member|
|:---|
|Начальной|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|Эксперт|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>Значения languageProficiencyLevel

|Member|
|:---|
|Начальной|
|Разговорный|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>Значения personRelationship

|Member|
|:---|
|manager|
|Коллега|
|directReport|
|dotLineReport|
|Помощник|
|dotLineManager|
|alternateContact|
|Друг|
|Супруга|
|Брат|
|child|
|родитель|
|Спонсор|
|emergencyContact|
|Других|
|unknownFutureValue|

### <a name="attachmenttype-values"></a>Значения attachmentType

| Member
|:--------------
| file
| item
| справочник

### <a name="analyticsactivitytype-values"></a>Значения analyticsActivityType

| Member
|:--------------
| call
| чат
| email
| фокус
| Конференц

### <a name="registrationauthmethod-values"></a>Значения registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone;|
|officePhone|
|securityQuestion|
|appNotification|
|AppCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>Значения entityTypes

|Member|
|:---|
|event|
|сообщение|
|driveItem|
|externalItem|
|site|
|список|
|listItem|
|drive|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>Значения searchAlterationType

| Member |
|:---------------|
|Модификация|
|Предложение|

### <a name="bucketaggregationsortproperty-values"></a>Значения bucketAggregationSortProperty

|Member|
|:---|
|count|
|keyAsString|
|keyAsNumber|

### <a name="contactrelationship-values"></a>Значения объекта contactRelationship

| Элемент             | Значение | Описание                              |
| :----------------- | :---- | :--------------------------------------- |
| родитель             | 0     | Родительский элемент пользователя.                       |
| Относительно           | 1     | Относительный пользователь.                     |
| Помощник               | 2     | Aide пользователя.                         |
| Доктор             | 3     | Пользователь должен быть доктором.                       |
| Опекуна           | 4     | Защитник пользователя.                     |
| child              | 5     | Дочерний элемент пользователя.                        |
| Других              | 6      | Неопределенная связь с пользователем. |
| unknownFutureValue | 7      | Значение маркера для обеспечения совместимости в будущем.   |

### <a name="scheduleentitytheme-values"></a>Значения scheduleEntityTheme

| Member
|:-------------------------
| white
| blue
| green
| purple
| pink
| yellow
| Серый
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>Значения timeOffReasonIconType

|Member|
|:---|
|Нет|
|Автомобилей|
|calendar|
|Запущена|
|Плоскости|
|first В.|
|Доктор|
|notWorking|
|Часы|
|обязанности|
|Глобус|
|Кубок|
|phone|
|Погода|
|Зонтик|
|piggyBank|
|Собака|
|Торт|
|trafficCone|
|Контактный|
|Солнечный|
|unknownFutureValue|

### <a name="timecardstate-values"></a>Значения timeCardState

|Member|
|:---|
|clockedIn|
|onBreak|
|clockedOut|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>Значения scheduleChangeState

| Member
|:----------------------------
|Ожидающие
|Утвержденных
|Отказался
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>Значения scheduleChangeRequestActor

| Member
|:----------------------------
|отправитель;
|получатель;
|manager
|system
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>значения workforceIntegrationEncryptionProtocol

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>значения workforceIntegrationSupportedEntities

|Member|
|:---|
|Нет|
|shift|
|swapRequest|
|userShiftPreferences|
|openShift|
|openShiftRequest|
|offerShiftRequest|
|unknownFutureValue|
|timeCard|
|timeOffReason|
|timeOff|
|timeOffRequest|

### <a name="confirmedby-values"></a>Значения confirmedBy

| Member
|:-----------------
| Нет|
| пользователь;|
| manager|
| unknownFutureValue|

### <a name="timezonestandard-values"></a>Значения timeZoneStandard

| Member
|:-----------------
| windows
| Iana


### <a name="freebusystatus-values"></a>значения freeBusyStatus

| Элемент           | Значение |
| :--------------- | :---- |
| Бесплатный             | 0     |
| Предварительный        | 1     |
| Занят             | 2     |
| Oof              | 3     |
| workingElsewhere | 4     |
| unknown          | –1    |


### <a name="physicaladdresstype-values"></a>Значения physicalAddressType

| Member
|:-------------------------
| unknown
| Дома
| Бизнес
| Других


### <a name="attendeetype-values"></a>Значения attendeeType

| Member
|:-------------------------
| Обязательный
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>Значения externalAudienceScope

| Member
|:-------------------------
| Нет
| contactsOnly
| все


### <a name="automaticrepliesstatus-values"></a>Значения automaticRepliesStatus

| Member
|:-------------------------
| отключено
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>Значения calendarColor

| Элемент      | Значение |
| :---------- | :---- |
| Авто        | –1    |
| lightBlue   | 0     |
| lightGreen  | 1     |
| lightOrange | 2     |
| lightGray   | 3     |
| lightYellow | 4     |
| lightTeal   | 5     |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>Значения educationSynchronizationProfileState

| Элемент             | Значение |
| :----------------- | :---- |
| Удаление           | 2     |
| deletionFailed     | 3     |
| provisioningFailed | 5     |
| Подготовлено        | 6      |
| Подготовки       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>значения educationSynchronizationStatus

| Member             |
| :----------------- |
| Приостановлена             |
| Inprogress         |
| success            |
| error              |
| validationError    |
| Карантин        |
| unknownFutureValue |
| Извлечение         |
| Проверка         |

### <a name="educationexternalsource-values"></a>значения educationExternalSource

| Member
|:-------------------------
| Sis
| Lms
| Вручную
| unknownFutureValue

### <a name="educationgender-values"></a>значения educationGender

| Member
|:-------------------------
| Женский
| Мужской
| Других
| unknownFutureValue


### <a name="eventtype-values"></a>Значения eventType

| Member
|:-------------------------
| singleInstance
| Вхождение
| Исключение
| seriesMaster


### <a name="sensitivity-values"></a>значения конфиденциальности

| Member
|:-------------------------
| Нормальной
| personal
| Частная
| Конфиденциальной


### <a name="importance-values"></a>значения важности

| Member
|:-------------------------
| Низкой
| Нормальной
| Высокой


### <a name="educationuserrole-values"></a>значения educationUserRole
| Member
|:---------------------
| student
| teacher
| Факультет


### <a name="meetingmessagetype-values"></a>Значения meetingMessageType

| Member
|:-----------------
| Нет
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>Значения followupFlagStatus

| Member
|:-------------------------
| notFlagged
| complete
| Помечены


### <a name="inferenceclassificationtype-values"></a>Значения inferenceClassificationType

| Member
|:-----------------
| Сосредоточены
| Других


### <a name="iosnotificationalerttype-values"></a>Значения iosNotificationAlertType

| Member
|:-------------------------
| deviceDefault
| Баннер
| Модального
| Нет

### <a name="deviceenrollmentfailurereason-values"></a>Значения deviceEnrollmentFailureReason

| Member
|:-------------
| unknown
| authentication
| авторизация
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>Значения bodyType
| Member
|:---------
| текст
| HTML


### <a name="locationtype-values"></a>Значения locationType

| Member
|:-------------------------
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| Отель
| Ресторан
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>Значения locationUniqueIdType

| Member
|:-------------------------
| unknown
| locationStore
| Каталог
| Частная
| Bing


### <a name="messageactionflag-values"></a>Значения messageActionFlag

| Member
|:-------------------------
| любой
| call
| doNotForward
| Выполнении
| Fyi
| forward
| noResponseNecessary
| read
| reply
| replyToAll
| Отзыв


### <a name="onenoteuserrole-values"></a>Значения onenoteUserRole

| Элемент      | Значение |
| :---------- | :---- |
| Владелец       | 0     |
| Участник | 1     |
| Читатель      | 2     |
| Нет        | –1    |


### <a name="operationstatus-values"></a>Значения operationStatus

| Member
|:-----------------
|NotStarted
|Работает
|Завершено
|Не выполнено


### <a name="onenotepatchactiontype-values"></a>Значения onenotePatchActionType

| Member
|:-------------------------
| Заменить
| Добавить
| Удалить
| Вставка
| В начало

### <a name="onenotepatchinsertposition-values"></a>Значения onenotePatchInsertPosition

| Member
|:-------------------------
| После
| До


### <a name="phonetype-values"></a>Значения phoneType

| Member
|:-------------------------
| Дома
| Бизнес
| мобильный
| Других
| Помощник
| homeFax
| businessFax
| otherFax
| pager
| Радио


### <a name="plannerpreviewtype-values"></a>Значения plannerPreviewType

| Member
|:-------------------------
| Автоматически
| noPreview
| checklist
| description
| справочник


### <a name="status-values"></a>значения состояния

| Member
|:-----------------
| Активных
| Обновлено
| deleted
| пропущено
| unknownFutureValue


### <a name="weekindex-values"></a>Значения weekIndex

| Member
|:-------------------------
| Первый
| Второй
| Третий
| Четвертый
| Последний


### <a name="dayofweek-values"></a>Значения dayOfWeek

| Member
|:-------------------------
| воскресенье
| понедельник
| вторник
| среда
| четверг
| пятница
| суббота

### <a name="recurrencepatterntype-values"></a>Значения recurrencePatternType

| Member
|:-------------------------
| Ежедневно
| Еженедельно
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>Значения recurrenceRangeType

| Member
|:-------------------------
| endDate
| noEnd
| Пронумерованы


### <a name="onenotesourceservice-values"></a>Значения onenoteSourceService
| Member
|:---------------------
| Unknown
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>Значения responseType

| Member
|:-------------------------
| Нет
| organizer
| tentativelyAccepted
| Принято
| Отказался
| notResponded


### <a name="activitydomain-values"></a>Значения activityDomain

| Member
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>Значения websiteType

| Member
|:-------------------------
| Других
| Дома
| work
| Блог
| profile


### <a name="categorycolor-values"></a>Значения categoryColor

| Элемент   | Значение |
| :------- | :---- |
| Нет     | –1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 2     |
| preset3  | 3     |
| preset4  | 4     |
| preset5  | 5     |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10    |
| preset11 | 11    |
| preset12 | 12     |
| preset13 | 13    |
| preset14 | 14    |
| preset15 | 15    |
| preset16 | 16    |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 20    |
| preset21 | 21    |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>Значения alertFeedback

Возможные значения обратной связи в оповещении, предоставляемом аналитиком.

| Элемент         | Значение | Описание               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | Неизвестно.                  |
| truePositive   | 1     | Оповещение имеет истинно положительный результат.   |
| falsePositive  | 2     | Оповещение имеет ложное срабатывание.  |
| benignPositive | 3     | Оповещение неопасно-положительное. |

### <a name="filehashtype-values"></a>Значения fileHashType

| Элемент              | Значение | Описание                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | Неизвестный тип.                  |
| sha1                | 1     | Тип хэша SHA1.                |
| sha256              | 2     | Тип хэша SHA256.              |
| md5                 | 3     | Тип хэша MD5.                 |
| authenticodeHash256 | 4     | Тип хэша AuthenticodeHash256. |
| lsHash              | 5     | Тип хэша LsHash.              |
| CTPH                | 6      | Тип хэша CTPH.                |
| peSha1              | 7      | Тип хэша PESHA1.              |
| peSha256            | 8      | Тип хэша PESHA256.            |

### <a name="connectiondirection-values"></a>значения connectionDirection

| Элемент   | Значение | Описание          |
| :------- | :---- | :------------------- |
| unknown  | 0     | Неизвестное соединение.  |
| Входящих  | 1     | Входящее подключение.  |
| Исходящих | 2     | Исходящее подключение. |

### <a name="connectionstatus-values"></a>Значения connectionStatus

| Элемент    | Значение | Описание                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | Неизвестное состояние подключения. |
| Попытка | 1     | Попытка подключения.      |
| Удалось | 2     | Подключение выполнено успешно.      |
| Заблокирован   | 3     | Подключение заблокировано.        |
| Сбой при    | 4     | Сбой подключения.         |

### <a name="processintegritylevel-values"></a>Значения processIntegrityLevel

| Элемент    | Значение | Описание                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | Неизвестно.                      |
| Ненадежных | 10    | Уровень целостности ненадежный. |
| Низкой       | 20    | Уровень целостности низкий.       |
| medium    | 30    | Уровень целостности — средний.    |
| Высокой      | 40    | Уровень целостности — Высокий.      |
| system    | 50    | Уровень целостности — System.    |

### <a name="registryhive-values"></a>значения registryHive

Перечисление для кустов реестра, определяемых [Кустами реестра](/windows/desktop/sysinfo/registry-hives).

| Элемент                  | Значение | Описание                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | Неизвестный куст.                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG hive.         |
| Currentuser             | 2     | HKEY_CURRENT_USER hive.           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM hive.      |
| localMachineSamSoftware | 4     | HKEY_LOCAL_MACHINE\Software hive. |
| localMachineSystem      | 5     | HKEY_LOCAL_MACHINE\System hive.   |
| usersDefault            | 6      | \\HKEY_USERS. Куст DEFAULT.        |

### <a name="registryoperation-values"></a>Значения registryOperation

Операция, которая изменила имя и (или) значение раздела реестра.

| Элемент  | Значение | Описание                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | Неизвестный тип значения реестра. |
| create  | 1     | Создайте реестр.             |
| Изменить  | 2     | Изменение реестра.             |
| delete  | 3     | Удаление реестра.             |

### <a name="registryvaluetype-values"></a>Значения registryValueType

Перечисление для типов значений реестра, определенных типами [значений реестра](/windows/desktop/sysinfo/registry-value-types).

| Элемент            | Значение | Описание                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | Неизвестный тип значения реестра.                 |
| двоичный            | 1     | REG_BINARY типа значения реестра.              |
| Dword             | 2     | REG_DWORD типа значения реестра.               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN типа значения реестра. |
| dwordBigEndian    | 4     | REG_DWORD_BIG_ENDIAN типа значения реестра.    |
| expandSz          | 5     | REG_EXPAND_SZ типа значения реестра.           |
| ссылка              | 6      | REG_LINK типа значения реестра.                |
| multiSz           | 7      | REG_MULTI_SZ типа значения реестра.            |
| Нет              | 8      | REG_NONE типа значения реестра.                |
| qword             | 9      | REG_QWORD типа значения реестра.               |
| qwordlittleEndian | 10    | REG_QWORD_LITTLE_ENDIAN типа значения реестра. |
| Sz                | 11    | REG_SZ типа значения реестра.                  |

### <a name="alertseverity-values"></a>Значения alertSeverity

Перечисление серьезности оповещений.

| Элемент        | Значение | Описание                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | Уровень серьезности неизвестен.              |
| Информационных | 1     | Уровень серьезности предназначен только для сведений. |
| Низкой           | 2     | Уровень серьезности низкий.                  |
| medium        | 3     | Уровень серьезности — средний.               |
| Высокой          | 4     | Серьезность высокая.                 |

### <a name="alertstatus-values"></a>Значения alertStatus

Возможные значения состояния жизненного цикла оповещений (стадии).

| Элемент     | Значение | Описание           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | Неизвестное состояние.       |
| newAlert   | 10    | Оповещение является новым.         |
| Inprogress | 20    | Оповещение выполняется. |
| resolved   | 30    | Оповещение разрешается.    |

### <a name="emailrole-values"></a>Значения emailRole

Возможные значения для ролей электронной почты.

| Элемент    | Значение | Описание             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | Неизвестная роль.           |
| sender    | 1     | Отправитель сообщения электронной почты.    |
| получатель; | 2     | Получатель сообщения электронной почты. |

### <a name="logontype-values"></a>Значения logonType

Возможные значения для метода входа пользователя.

| Элемент            | Значение | Описание                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | –1    | Неизвестно.                     |
| Интерактивная       | 0     | Вход является интерактивным.        |
| remoteInteractive | 1     | Вход в систему является удаленным интерактивным. |
| Сети           | 2     | Вход в систему — это сеть.            |
| batch             | 3     | Вход выполняется пакетно.              |
| служба           | 4     | Вход — это служба.            |

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группах) для определения Windows.

| Элемент        | Значение | Описание                     |
| :------------ | :---- | :------------------------------ |
| unknown       | –1    | Неизвестно.                        |
| стандарт      | 0     | Член группы "Стандартные пользователи". |
| Мощность         | 1     | Член группы Power Users.    |
| Администратора | 2     | Член группы "Администраторы". |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>Значения chatMessagePolicyViolationDlpActionType

| Значение |
|:-----------------|
| Нет |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>Значения scopeOperatorMultiValuedComparisonType

|Member|
|:---|
|все|
|любой|

### <a name="risklevel-values"></a>Значения riskLevel

|Member|
|:---|
|Низкой|
|medium|
|Высокой|
|hidden|
|Нет|
|unknownFutureValue|

### <a name="riskstate-values"></a>Значения riskState

|Member|
|:---|
|Нет|
|confirmedSafe|
|исправлено|
|Уволен|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>Значения advancedConfigState

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>Значения referenceAttachmentPermission

|Member|
|:---|
|Других|
|представление|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>Значения referenceAttachmentProvider

|Member|
|:---|
|Других|
|oneDriveBusiness|
|oneDriveConsumer|
|Dropbox|

### <a name="networktype-values"></a>Значения networkType

|Member|
|:---|
|Интрасети|
|Экстрасети|
|namedNetwork|
|Доверенных|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|RestId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>Значения attributeFlowBehavior

|Member|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>Значения attributeFlowType

|Member|
|:---|
|Всегда|
|objectAddOnly|
|multiValueAddOnly|
|RestId|

### <a name="objectflowtypes-values"></a>Значения objectFlowTypes

| Элемент | Значение |
| :----- | :---- |
| Нет   | 0     |
| Добавление    | 1     |
| Update | 2     |
| Delete | 4     |

### <a name="chatmessagetype-values"></a>Значения chatMessageType

|Member|
|:---|
|сообщение|
|chatEvent |
|Ввода |
|unknownFutureValue|
|systemEventMessage|

### <a name="chatmessageimportance-values"></a>Значения chatMessageImportance

|Member|
|:---|
|Нормальной|
|Высокой|
|Срочно|

### <a name="channelmembershiptype-values"></a>Значения channelMembershipType

| Member             |
| :----------------- |
| стандарт           |
| Частная            |
| unknownFutureValue |
| общие             |

### <a name="stagedfeaturename-values"></a>Значения stagedFeatureName

| Member                    | Описание                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | Сквозная проверка подлинности    |
| seamlessSso               | Простой единый вход       |
| passwordHashSync          | Синхронизация хэша паролей |
| emailAsAlternateId        | Адрес электронной почты в качестве альтернативного идентификатора      |
| unknownFutureValue        | Элемент sentinel             |

### <a name="tokenissuertype-values"></a>Значения tokenIssuerType

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|
|AzureADBackupAuth|
|ADFederationServicesMFAAdapter|
|NPSExtension|


### <a name="riskdetectiontimingtype-values"></a>Значения riskDetectionTimingType

|Member|
|:---|
|notDefined|
|Realtime|
|nearRealtime|
|Автономных|
|unknownFutureValue|

### <a name="activitytype-values"></a>Значения activityType

|Member|
|:---|
|Signin|
|пользователь;|
|unknownFutureValue|
|servicePrincipal|

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>Значения chatMessagePolicyViolationUserActionType

| Member   | Значение int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 | Значение по умолчанию. Это значение в сообщении, если пользователь не выполняет действие с сообщением, заблокированным защитой от потери данных. |
| Override | 1 | Отправитель переопределил решение и отправил сообщение.|
| ReportFalsePositive | 2 | Отправитель сообщил администраторам о ложном срабатывании сообщения.|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>Значения chatMessagePolicyViolationVerdictDetailsType

| Member   | Значение int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 |  Пользователю не разрешено переопределять сообщение. Пользователю не разрешено сообщать о сообщении как ложноположительном, если подсказка политики не указана. Во всех остальных сценариях пользователь может сообщить о сообщении как о ложном срабатывании.|
| AllowFalsePositiveOverride | 1 |  Пользователю не разрешено явно переопределять блок, если он не объедиен с флагами `AllowOverrideWithoutJustification` `AllowOverrideWithJustification` . Сообщение о ложном срабатывании нарушения автоматически переопределяет блок и отправляет сообщение. |
| AllowOverrideWithoutJustification | 2 | Пользователю разрешено переопределять блок и отправлять сообщение. Текст обоснования не требуется. Монопольно.`AllowOverrideWithJustification` |
| AllowOverrideWithJustification | 4 |  Пользователю разрешено переопределять блок и отправлять сообщение. Требуется текст обоснования. Монопольно.`AllowOverrideWithoutJustification`|

### <a name="entitytype-values"></a>Значения entityType

| Member       |
|:--------------|
|event|
|сообщение|
|driveItem|
|externalFile|
|externalItem|

### <a name="onlinemeetingprovidertype-values"></a>Значения onlineMeetingProviderType

|Member|
|:---|
|unknown|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>Значения delegateMeetingMessageDeliveryOptions

|Member|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>Значения calendarRoleType

|Member|
|:---|
|Нет|
|freeBusyRead|
|limitedRead|
|read|
|write|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|Пользовательские|

### <a name="contentformat-values"></a>Значения contentFormat

| Элемент  | Значение | Описание                          |
| :------ | :---- | :----------------------------------- |
| default | 0     | Содержимое — это файл или тип, отличный от электронной почты. |
| email   | 1     | Содержимое — это сообщение электронной почты.                 |

### <a name="contentstate-values"></a>Значения contentState

| Элемент | Значение | Описание                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| Остальные   | 0     | Неактивные данные; Например, файл в общей папке.                                 |
| Движения | 1     | Данные в движении. Файл, перехваченный сетевым устройством при передаче.         |
| Использовать    | 2     | Данные используются. Файл открыт в клиентском приложении, например Microsoft Office. |

### <a name="assignmentmethod-values"></a>Значения assignmentMethod

| Элемент     | Значение | Описание                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| стандарт   | 0     | Метка задается службой или условием политики.                                                                              |
| Привилегированных | 1     | Метка была явно задана пользователем.                                                                                          |
| Авто       | 2     | Разрешает переопределение любой существующей метки. Обоснование, необходимое для понижения уровня. Приводит к методу `standard` присваивания в метаданных. |

### <a name="actionsource-values"></a>Значения actionSource

| Элемент        | Значение | Описание                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| Вручную        | 0     | Пользователь вручную выберет метку.                          |
| Автоматически     | 1     | Метка была выбрана в результате выполнения условий политики.       |
| Рекомендуемый   | 2     | Выбранная для применения рекомендуемой метки.                    |
| policyDefault | 3     | Пользователь не выполняет никаких действий, и была применена метка по умолчанию политики. |
| Обязательным     | 4     | Пользователь выбрал метку после принудительного выбора.         |

### <a name="contentalignment-values"></a>Значения contentAlignment

| Элемент | Значение | Описание                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | Выравнивание пометки содержимого по левому краю.  |
| Правильно  | 1     | Выравнивание пометки содержимого по правому краю. |
| Центр | 2     | Пометка содержимого по центру.             |

### <a name="watermarklayout-values"></a>Значения watermarkLayout

| Элемент     | Значение | Описание                 |
| :--------- | :---- | :-------------------------- |
| Горизонтальной | 0     | Используйте горизонтальную подложку. |
| Диагональ   | 1     | Используйте диагональную подложку.   |

### <a name="conditionalaccesspolicystate-values"></a>Значения conditionalAccessPolicyState

|Member|
|:---|
|включено|
|отключено|
|enabledForReportingButNotEnforced|

### <a name="conditionalaccessgrantcontrol-values"></a>Значения conditionalAccessGrantControl

| Member       |
|:--------------|
|Блок|
|Мид|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|
|passwordChange|
|unknownFutureValue|

### <a name="conditionalaccessrule-values"></a>Значения conditionalAccessRule 

|Member|
|:---|
|allApps|
|firstPartyApps|
|office365|
|appId|
|Acr|
|appFilter|
|Allusers|
|Гостевой|
|groupId|
|roleId|
|userId|
|allDevicePlatforms|
|devicePlatform|
|allLocations|
|insideCorpnet|
|allTrustedLocations|
|locationId|
|allDevices|
|deviceFilter|
|deviceState|
|unknownFutureValue|
|deviceFilterIncludeRuleNotMatched|
|allDeviceStates|

### <a name="signinaccesstype-values"></a>Значения signInAccessType 

|Member|
|:---|
|Нет|
|b2bCollaboration|
|b2bDirectConnect|
|microsoftSupport|
|Serviceprovider|
|unknownFutureValue|

### <a name="signinfrequencytype-values"></a>Значения signinFrequencyType

| Member       |
|:--------------|
|days|
|Часов|

### <a name="persistentbrowsersessionmode-values"></a>Значения persistentBrowserSessionMode

| Member       |
|:--------------|
|Всегда|
|Нвер|

### <a name="cloudappsecuritysessioncontroltype-values"></a>Значения cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="conditionalaccessdeviceplatform-values"></a>Значения conditionalAccessDevicePlatform

| Member       |
|:--------------|
|Android|
|iOS|
|windows|
|WindowsPhone|
|macOS|
|все|
|unknownFutureValue|

### <a name="priority-values"></a>значения приоритета

|Элемент|Значение|
|:---|:---|
|Нет|0|
|High (Высокий)|1|
|Низкая|2|

### <a name="threatassessmentcontenttype-values"></a>Значения threatAssessmentContentType

| Элемент | Значение | Описание             |
|:-------|:------|:------------------------|
| mail;   | 1     | Почтовая угроза.            |
| url    | 2     | Угроза URL-адреса.             |
| file   | 3     | Угроза файла вложения. |

### <a name="threatexpectedassessment-values"></a>Значения threatExpectedAssessment

| Элемент  | Значение | Описание                       |
|:--------|:------|:----------------------------------|
| Блок   | 1     | Угроза должна быть заблокирована.     |
| Разблокировать | 2     | Угрозу не следует блокировать. |

### <a name="threatcategory-values"></a>Значения threatCategory

| Элемент             | Значение | Описание        |
|:-------------------|:------|:-------------------|
| уверенности               | 1     | Угроза нежелательной почты.       |
| степенью           | 2     | Фишинговая угроза.   |
| malware            | 3     | Угроза вредоносных программ.    |
| unknownFutureValue | 4     | Элемент sentinel. |

### <a name="threatassessmentstatus-values"></a>Значения threatAssessmentStatus

| Элемент    | Значение | Описание                              |
|:----------|:------|:-----------------------------------------|
| Ожидающие   | 1     | Оценка угроз все еще выполняется. |
| Завершена | 2     | Оценка угроз завершена.         |

### <a name="threatassessmentrequestsource-values"></a>Значения threatAssessmentRequestSource

| Элемент        | Значение | Описание              |
|:--------------|:------|:-------------------------|
| Неопределенный     | 0     | Пока не известно.            |
| пользователь;          | 1     | Отправка пользователя.         |
| Администратора | 2     | Отправка администратора клиента. |

### <a name="threatassessmentresulttype-values"></a>Значения threatAssessmentResultType

| Элемент             | Значение | Описание                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | Результат проверки политики, только для оценки `mail` . |
| Повторное сканирование             | 2     | Результат повторного сканирования.                                   |
| unknownFutureValue | 3     | Элемент sentinel.                                   |

### <a name="maildestinationroutingreason-values"></a>Значения mailDestinationRoutingReason

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| Нет                  | 0     | Пока не известно.                       |
| mailFlowRule          | 1     | Правило транспорта Exchange.            |
| safeSender            | 2     | Список надежных отправителей.                   |
| blockedSender         | 3     | Список заблокированных отправителей.                |
| advancedSpamFiltering | 4     | Расширенный параметр фильтрации нежелательной почты.     |
| domainAllowList       | 5     | Список разрешений домена отправителя.           |
| domainBlockList       | 6      | Список блоков домена отправителя.           |
| notInAddressBook      | 7      | Исключить отправителя не в адресной книге. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправителя.   |
| autoPurgeToInbox      | 9      | Перемещение сообщения TimeTravel в папку "Входящие".   |
| autoPurgeToJunk       | 10    | Перемещение сообщения TimeTravel в нежелательное.    |
| autoPurgeToDeleted    | 11    | Сообщение о перемещении TimeTravel в удаленное. |
| Исходящих              | 12     | Исходящая почта.                      |
| notJunk               | 13    | Разрешить из-за нежелательной почты.              |
| Нежелательной                  | 14    | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15    | Элемент sentinel.                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>Значения threatAssessmentRequestPivotProperty

| Элемент                       | Значение | Описание                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | Агрегировать запрос на оценку угроз по `threatCategory`.               |
| mailDestinationRoutingReason | 2     | Агрегировать запрос на оценку угроз по `mailDestinationRoutingReason`. |

### <a name="userflowtype-values"></a>Значения userFlowType

|Member
|:----------------------
| Регистрации
| Signin
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| unknownFutureValue

### <a name="openidconnectresponsemode-values"></a>Значения openIdConnectResponseMode

| Member
|:----------------------
| form_post
| Запрос
| unknownFutureValue

### <a name="wellknownlistname-values"></a>Значения wellknownListName

| Member
|:----------------------
| Нет
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>Значения taskStatus

| Member
|:----------------------
| notStarted
| Inprogress
| Завершена
| waitingOnOthers
| Отложенные

### <a name="columntypes-values"></a>Значения columnTypes

|Member|Описание|
|:-------|:------
|Примечание| многострочный текст. |
|текст | однострочный текст. |
|Выбор | столбец выбора |
|multichoice | столбец multichoice. |
|число | столбец number. |
|Валюты | столбец валюты. |
|dateTime | Столбец dateTime. |
|Поиска | столбец подстановки. |
|логический | Столбец "Да" или "Нет". |
|пользователь; | столбец пользователя или группы. |
|url | гиперссылка или столбец рисунка. |
|Рассчитывается | вычисляемый столбец. |
|расположение; | столбец location. |
|географическое положение | столбец географического расположения. |
|term | столбец управляемых метаданных. |
|многотерминантная | столбец управляемых метаданных, который принимает несколько значений. |
|Миниатюру | Столбец изображения. |
|approvalStatus | Столбец состояния утверждения контента. |
|unknownFutureValue | unknownFuturevalue |

### <a name="connectedorganizationstate-values"></a>Значения connectedOrganizationState

| Элемент                | Значение | Описание                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Настроен            | 0     | Подключенные организации с этим значением состояния включаются в политики назначения с типом области запрашиваемого объекта `AllConfiguredConnectedOrganizationSubjects`.                                                          |
| Предлагаемые              | 1     | Подключенные организации, автоматически созданные системой, имеют это значение состояния. Они не включены в политики назначения с типом области запроса `AllConfiguredConnectedOrganizationSubjects`.   |
| unknownFutureValue    | 2     | Элемент sentinel.                                                                                                                                                                                                 |

### <a name="identityuserflowattributedatatype-values"></a>Значения identityUserFlowAttributeDataType

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| string                | 1     | строковый тип данных                    |
| логический               | 2     | тип данных Boolean                   |
| int64                 | 3     | Тип данных Int                       |
| Stringcollection      | 4     | Тип данных коллекции строк         |
|dateTime|5||
| unknownFutureValue    | 6      | Элемент sentinel.                  |

### <a name="identityuserflowattributetype-values"></a>Значения identityUserFlowAttributeType

| Элемент                | Значение | Описание                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| Builtin               | 1     | Этот тип атрибута потока пользователя обозначает, что он был создан системой |
| Пользовательские                | 2     | Этот тип атрибута потока пользователя указывает, что он был создан пользователем.   |
|обязательно|3||
| unknownFutureValue    | 4     | Элемент sentinel.                                                 |

### <a name="permissionclassificationtype-values"></a>Значения permissionClassificationType

| Member
|:-------
| Низкой

### <a name="permissiontype-values"></a>Значения permissionType

| Member
|:-------------------------
| приложение
| Делегированные
| delegatedUserConsentable

### <a name="identityuserflowattributeinputtype-values"></a>Значения identityUserFlowAttributeInputType

| Member                |
|:----------------------|
| Textbox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>Значения teamworkActivityTopicSource

| Member
|:---
| entityUrl
| текст

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>Значения cloudPcProvisioningPolicyImageType

|Member|
|:---|
|Пользовательские|
|Галерея|

### <a name="chattype-values"></a>Значения chatType

| Элемент             | Значение | Описание               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Указывает, что чат является чатом 1:1. Для этого типа чата задан фиксированный размер, член не может быть удален или добавлен.                  |
|group               | 1     | Указывает, что чат является групповым чатом. Для этого типа чата можно изменить размер реестра (не менее 2 человек). Элементы можно удалить или добавить позже.   |
|Конференц             | 2     | Указывает, что чат является чатом собрания, который создается как побочный эффект создания OnlineMeeting.  |
|unknownFutureValue  | 3     | Значение Sentinel, указывающее будущие значения. |

### <a name="singlesignonmode-values"></a>Значения singleSignOnMode

|Member|
|:---|
|Нет|
|onPremisesKerberos|
|aadHeaderBased|
|pingHeaderBased|

### <a name="plannercontainertype-values"></a>Значения plannerContainerType

|Member|
|:---|
|group|
|unknownFutureValue|
|состав|

### <a name="plannerplancontexttype-values"></a>Значения plannerPlanContextType

|Member|
|:---|
|teamsTab|
|sharePointPage|
|meetingNotes|
|Других|
|unknownFutureValue|

### <a name="plannercontextstate-values"></a>Значения plannerContextState

|Member             |
|:------------------|
|Активных             |
|delinked           |
|unknownFutureValue |  


### <a name="policyscope-values"></a>Значения policyScope

|Member|
|:---|
|Нет|
|все|
|Выбранного|

### <a name="teamsappinstallationscope-values"></a>Значения teamsAppInstallationScope

|Элемент    |Значение    |Описание |
|:---------|:--------|:----------- |
|team      |0        |Указывает, что приложение Teams может быть установлено в команде и имеет право на доступ к данным этой команды.|
|groupChat |1        |Указывает, что приложение Teams может быть установлено в групповом чате и имеет право на доступ к данным этого чата группы.|
|personal  |2        |Указывает, что приложение Teams может быть установлено в личной области пользователя и имеет право на доступ к данным этого пользователя.|

### <a name="roleassignmentschedulerequestfilterbycurrentuseroptions-values"></a>Значения roleAssignmentScheduleRequestFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="roleassignmentschedulefilterbycurrentuseroptions-values"></a>Значения roleAssignmentScheduleFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|unknownFutureValue|

### <a name="roleassignmentscheduleinstancefilterbycurrentuseroptions-values"></a>Значения roleAssignmentScheduleInstanceFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|unknownFutureValue|

### <a name="roleeligibilityschedulerequestfilterbycurrentuseroptions-values"></a>Значения roleEligibilityScheduleRequestFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="roleeligibilityschedulefilterbycurrentuseroptions-values"></a>Значения roleEligibilityScheduleFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|unknownFutureValue|

### <a name="roleeligibilityscheduleinstancefilterbycurrentuseroptions-values"></a>Значения roleEligibilityScheduleInstanceFilterByCurrentUserOptions

|Member|
|:---|
|Основной|
|unknownFutureValue|

### <a name="cloudpcauditactivityoperationtype-values"></a>Значения cloudPcAuditActivityOperationType

|Member|
|:---|
|create|
|delete|
|Патч|
|Других|

### <a name="cloudpcauditactivityresult-values"></a>Значения cloudPcAuditActivityResult

|Member|
|:---|
|success|
|clientError|
|Сбоя|
|timeout|
|Других|

### <a name="cloudpcauditactortype-values"></a>Значения cloudPcAuditActorType

|Member|
|:---|
|itPro|
|приложение|
|Партнер|
|unknown|

### <a name="cloudpcauditcategory-values"></a>Значения cloudPcAuditCategory

|Member|
|:---|
|CloudPC|
|Других|

### <a name="posttype-values"></a>Значения postType

|Member|
|:---|
|Регулярные|
|Быстрый|
|Стратегических|
|unknownFutureValue|

### <a name="servicehealthclassificationtype-values"></a>Значения serviceHealthClassificationType

|Member|
|:---|
|Консультативный|
|Инцидента|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>Значения serviceHealthOrigin

|Member|
|:---|
|Microsoft|
|thirdParty|
|Клиентов|
|unknownFutureValue|

### <a name="servicehealthstatus-values"></a>Значения serviceHealthStatus

|Member|
|:---|
|serviceOperational|
|изучении|
|restoringService|
|verifyingService|
|serviceRestored|
|postIncidentReviewPublished|
|serviceDegradation|
|serviceInterruption|
|extendedRecovery|
|falsePositive|
|investigationSuspended|
|resolved|
|mitigatedExternal|
|Смягчить|
|resolvedExternal|
|Подтвердил|
|Сообщили|
|unknownFutureValue|

### <a name="serviceupdatecategory-values"></a>Значения serviceUpdateCategory

|Member|
|:---|
|preventOrFixIssue|
|planForChange|
|stayInformed|
|unknownFutureValue|

### <a name="serviceupdateseverity-values"></a>Значения serviceUpdateSeverity

|Member|
|:---|
|Нормальной|
|Высокой|
|Критических|
|unknownFutureValue|

### <a name="teamworktagtype-values"></a>Значения teamworkTagType

|Элемент| Значение | Описание               |
|:---|:---- | :------------------------ |
|стандарт| 0     |Тип по умолчанию для тега. Тегами уровня "Стандартный" в команде могут управлять участники с разрешениями.|

### <a name="teamworkapplicationidentitytype-values"></a>Значения teamworkApplicationIdentityType

|Member|
|:---|
|aadApplication|
|бот|
|tenantBot|
|office365Connector|
|outgoingWebhook|
|unknownFutureValue|

### <a name="teamworkconversationidentitytype-values"></a>Значения teamworkConversationIdentityType

|Member|
|:---|
|team|
|channel|
|чат|
|unknownFutureValue|

### <a name="teamworkuseridentitytype-values"></a>Значения teamworkUserIdentityType

|Member|
|:---|
|aadUser|
|onPremiseAadUser|
|anonymousGuest|
|federatedUser|
|personalMicrosoftAccountUser|
|skypeUser|
|phoneUser|
|unknownFutureValue|
|emailUser|

### <a name="callrecordingstatus-values"></a>Значения callRecordingStatus

|Member|
|:---|
|success|
|Сбоя|
|Первоначального|
|chunkFinished|
|unknownFutureValue|

### <a name="payloaddeliveryplatform-values"></a>Значения payloadDeliveryPlatform

|Member|
|:---|
|unknown|
|Sms|
|email|
|Команды|
|unknownFutureValue|

### <a name="trainingstatus-values"></a>значения trainingStatus

|Member|
|:---|
|unknown|
|Назначен|
|Inprogress|
|Завершена|
|Просроченные|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>Значения teamworkCallEventType

|Member|
|:---|
|call|
|Конференц|
|screenShare|
|unknownFutureValue|

### <a name="binaryoperator-values"></a>Значения binaryOperator 

|Member|
|:---|
|или|
|и|

### <a name="subjectrightsrequeststage-values"></a>Значения subjectRightsRequestStage 

|Member|
|:---|
|contentRetrieval|
|contentReview| 
|generateReport| 
|contentDeletion|
|CaseResolved|
|unknownFutureValue|

### <a name="subjectrightsrequeststagestatus-values"></a>Значения subjectRightsRequestStageStatus 

|Member|
|:---|
|notStarted|
|Текущего|
|Завершена|
|Сбой при|
|unknownFutureValue|

### <a name="subjectrightsrequeststatus-values"></a>Значения subjectRightsRequestStatus 

|Member|
|:---|
|Активных|
|Закрыт|
|unknownFutureValue|

### <a name="subjectrightsrequesttype-values"></a>Значения subjectRightsRequestType 

|Member|
|:---|
|Экспорт|
|delete|
|Доступа|
|tagForAction|
|unknownFutureValue|

### <a name="datasubjecttype-values"></a>Значения dataSubjectType 

|Member|
|:---|
|Клиентов|
|currentEmployee|
|formerEmployee|
|prospectiveEmployee|
|student|
|teacher|
|Факультет|
|Других|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>Значения answerInputType

|Элемент|Значение|Описание|
|:---|:---|:---|
|text|0|Текст.|
|Radiobutton|1|Radiobutton.|
|unknownFutureValue|2|UnknownFutureValue.|

### <a name="taskstatus_v2-values"></a>taskStatus_v2 значения

|Member|
|:---|
|notStarted|
|Inprogress|
|Завершена|
|unknownFutureValue|


### <a name="wellknownlistname_v2-values"></a>wellKnownListName_v2 значения

|Member|
|:---|
|Нет|
|defaultList|
|flaggedEmail|
|unknownFutureValue|

### <a name="bookingpricetype-values"></a>Значения bookingPriceType

|Member|
|:---|
|Неопределенный|
|fixedPrice|
|startingAt|
|Почасовой|
|Бесплатный|
|priceVaries|
|Каллуса|
|Notset|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>Значения bookingStaffRole 

|Member|
|:---|
|Гостевой|
|Администратора|
|Просмотра|
|externalGuest|
|unknownFutureValue|
|Планировщик|
|член|

### <a name="bookingreminderrecipients-values"></a>Значения bookingReminderRecipients 

|Member|
|:---|
|allAttendees|
|Персонал|
|Клиентов|
|unknownFutureValue|

### <a name="teamworkconnectionstatus-values"></a>Значения teamworkConnectionStatus

| Member |
|:--------|
|unknown|
|Подключен|
|Отключен|
|unknownFutureValue|

### <a name="teamworkdeviceactivitystate-values"></a>Значения teamworkDeviceActivityState

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|unknown|0|Неизвестное состояние.|
|Занят|1|Устройство занято.|
|Простоя|2|Устройство простаивает.|
|Недоступен|3|Устройство недоступно.|
|unknownFutureValue|4|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="teamworkdeviceoperationtype-values"></a>Значения teamworkDeviceOperationType

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|deviceRestart|0|Перезапустите устройство.|
|configUpdate|1|Обновите конфигурацию устройства.|
|deviceDiagnostics|2|Получение журналов устройств.|
|softwareUpdate|3|Обновление программного обеспечения на устройстве.|
|deviceManagementAgentConfigUpdate|4|Обновите конфигурацию агента устройства.|
|remoteLogin|5|Удаленное имя входа устройства.|
|remoteLogout|6 |Удаленный вход устройства.|
|unknownFutureValue|7 |Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="teamworksoftwarefreshness-values"></a>Значения teamworkSoftwareFreshness

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|unknown|0|Неизвестное значение.|
|Последнее|1|Указывает, запускает ли компонент устройства последнюю версию программного обеспечения.|
|updateAvailable|2|Указывает, что обновление программного обеспечения доступно для компонента устройства.|
|unknownFutureValue|3|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="teamworksoftwaretype-values"></a>Значения teamworkSoftwareType

| Member |
|:---------------|
|adminAgent|
|operatingSystem|
|teamsClient|
|Прошивки|
|partnerAgent|
|companyPortal|
|unknownFutureValue|

### <a name="teamworksupportedclient-values"></a>Значения teamworkSupportedClient

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|unknown|0|Неизвестное значение.|
|skypeDefaultAndTeams|1|Поддерживает и . `Skype` , и `Teams`. Значение по умолчанию: `Skype`.|
|teamsDefaultAndSkype|2|Поддерживает и . `Skype` , и `Teams`. Значение по умолчанию: `Teams`.|
|SkypeOnly|3|Поддерживает только .`Skype`|
|teamsOnly|4|Поддерживает только .`Teams`|
|unknownFutureValue|5|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="longrunningoperationstatus-values"></a>Значения longRunningOperationStatus

| Member|
|:-----------------|
|notStarted|
|Запущена|
|Удалось|
|Сбой при|
|unknownFutureValue|

### <a name="delegatedadminaccessassignmentstatus-values"></a>Значения delegatedAdminAccessAssignmentStatus 

|Member|
|:---|
|Ожидающие|
|Активных|
|Удаление|
|deleted|
|error|
|unknownFutureValue|

### <a name="delegatedadminaccesscontainertype-values"></a>Значения delegatedAdminAccessContainerType 

|Member|
|:---|
|securityGroup|
|unknownFutureValue|

### <a name="delegatedadminrelationshipoperationtype-values"></a>Значения delegatedAdminRelationshipOperationType 

|Member|
|:---|
|delegatedAdminAccessAssignmentUpdate|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequestaction-values"></a>Значения delegatedAdminRelationshipRequestAction 

|Member|
|:---|
|lockForApproval|
|Прекратить|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequeststatus-values"></a>Значения delegatedAdminRelationshipRequestStatus 

|Member|
|:---|
|создано|
|Ожидающие|
|Удалось|
|Сбой при|
|unknownFutureValue|

### <a name="delegatedadminrelationshipstatus-values"></a>Значения delegatedAdminRelationshipStatus 

|Member|
|:---|
|Активация|
|Активных|
|approvalPending|
|Утвержденных|
|создано|
|Истек|
|Истекает|
|Прекращено|
|Прекращения|
|terminationRequested|
|unknownFutureValue|
