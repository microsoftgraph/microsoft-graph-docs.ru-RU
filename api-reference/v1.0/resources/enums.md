---
title: Значения перечисления
description: Значения перечисления Microsoft Graph.
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: 43a22ad7bdd5ba93e70016105078c9c3e9e626a7
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855646"
---
# <a name="enum-values"></a>Значения перечисления

Пространство имен: microsoft.graph

### <a name="bookingsavailabilitystatus-values"></a>Значения bookingsAvailabilityStatus
|Member|
|:---|
|доступен|
|Занят|
|slotsAvailable|
|outOfOffice|
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
|user|
|group|

### <a name="federatedidpmfabehavior-values"></a>Значения federatedIdpMfaBehavior
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

### <a name="expirationpatterntype-values"></a>Значения expirationPatternType 

|Member|
|:---|
|notSpecified|
|noExpiration|
|afterDateTime|
|afterDuration|

### <a name="recurrencepatterntype-values"></a>Значения recurrencePatternType 

|Member|
|:---|
|Ежедневно|
|Еженедельно|
|absoluteMonthly|
|relativeMonthly|
|absoluteYearly|
|relativeYearly|

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

### <a name="roleassignmentschedulerequestfilterbycurrentuseroptions-values"></a>Значения roleAssignmentScheduleRequestFilterByCurrentUserOptions 

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

### <a name="roleeligibilityschedulerequestfilterbycurrentuseroptions-values"></a>Значения roleEligibilityScheduleRequestFilterByCurrentUserOptions 

|Member|
|:---|
|Основной|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="unifiedrolemanagementpolicyruletargetoperations-values"></a>Значения unifiedRoleManagementPolicyRuleTargetOperations 

|Member|
|:---|
|все|
|Активировать|
|Отключить|
|Назначить|
|Обновление|
|Удалить|
|Расширить|
|renew|
|unknownFutureValue|

### <a name="unifiedroleschedulerequestactions-values"></a>Значения unifiedRoleScheduleRequestActions 

|Member|
|:---|
|adminAssign|
|adminUpdate|
|adminRemove|
|selfActivate|
|selfDeactivate|
|adminExtend|
|adminRenew|
|selfExtend|
|selfRenew|
|unknownFutureValue|

### <a name="approvalfilterbycurrentuseroptions-values"></a>Значения approvalFilterByCurrentUserOptions 

|Member|
|:---|
|target|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="accessreviewexpirationbehavior-values"></a>Значения accessReviewExpirationBehavior

|Member|
|:---|
|keepAccess|
|removeAccess|
|acceptAccessRecommendation|
|unknownFutureValue|

### <a name="allowedtargetscope-values"></a>Значения allowedTargetScope

|Member|
|:---|
|notSpecified|
|specificDirectoryUsers|
|specificConnectedOrganizationUsers|
|specificDirectoryServicePrincipals|
|allMemberUsers|
|allDirectoryUsers|
|allDirectoryServicePrincipals|
|allConfiguredConnectedOrganizationUsers|
|allExternalUsers|
|unknownFutureValue|

### <a name="approvalfilterbycurrentuseroptions-values"></a>Значения approvalFilterByCurrentUserOptions 

|Member|
|:---|
|target|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="accesspackageassignmentfilterbycurrentuseroptions-values"></a>значения accessPackageAssignmentFilterByCurrentUserOptions

|Member|
|:---|
|target|
|createdBy|
|unknownFutureValue|

### <a name="accesspackageassignmentrequestfilterbycurrentuseroptions-values"></a>значения accessPackageAssignmentRequestFilterByCurrentUserOptions

|Member|
|:---|
|target|
|createdBy|
|Утверждающий|
|unknownFutureValue|

### <a name="accesspackageassignmentstate-values"></a>Значения accessPackageAssignmentState

|Member|
|:---|
|Доставки|
|partiallyDelivered|
|Доставлены|
|Истек|
|deliveryFailed|
|unknownFutureValue|

### <a name="accesspackagecatalogstate-values"></a>значения accessPackageCatalogState

|Member|
|:---|
|Неопубликованные|
|Опубликовано|
|unknownFutureValue|

### <a name="accesspackagecatalogtype-values"></a>Значения accessPackageCatalogType

|Member|
|:---|
|userManaged|
|serviceDefault|
|serviceManaged|
|unknownFutureValue|

### <a name="accesspackageexternaluserlifecycleaction-values"></a>Значения accessPackageExternalUserLifecycleAction

|Member|
|:---|
|none|
|blockSignIn|
|blockSignInAndDelete|
|unknownFutureValue|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>значения accessPackageFilterByCurrentUserOptions

|Member|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="accesspackagerequeststate-values"></a>Значения accessPackageRequestState

|Member|
|:---|
|Представлены|
|pendingApproval|
|Доставки|
|Доставлены|
|deliveryFailed|
|denied|
|scheduled|
|Отменен|
|partiallyDelivered|
|unknownFutureValue|

### <a name="accesspackagerequesttype-values"></a>Значения accessPackageRequestType

|Member|
|:---|
|notSpecified|
|userAdd|
|userUpdate|
|userRemove|
|adminAdd|
|adminUpdate|
|adminRemove|
|systemAdd|
|systemUpdate|
|systemRemove|
|onBehalfAdd|
|unknownFutureValue|

### <a name="accesspackagesubjecttype-values"></a>Значения accessPackageSubjectType

|Member|
|:---|
|notSpecified|
|user|
|servicePrincipal|
|unknownFutureValue|

### <a name="connectedorganizationstate-values"></a>Значения connectedOrganizationState

|Member|
|:---|
|Настроен|
|Предлагаемые|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>значения accessReviewInstanceDecisionItemFilterByCurrentUserOptions 

|Member|
|:---|
|Рецензент|
|unknownFutureValue|

### <a name="volumetype-values"></a>Значения volumeType

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

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
|clientIpAddress|
|authenticatorAppGps|

### <a name="countrylookupmethodtype-values"></a>Значения countryLookupMethodType

|Member|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>Значения consentRequestFilterByCurrentUserOptions 

|Member|
|:---|
|Рецензент|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>Значения externalEmailOtpState

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>значения educationAddedStudentAction

|Member|
|:---|
|none|
|assignIfOpen|
|unknownFutureValue|

### <a name="fido2restrictionenforcementtype-values"></a>Значения fido2RestrictionEnforcementType

|Member|
|:---|
|Позволяют|
|Блок|

### <a name="attestationlevel-values"></a>Значения attestationLevel

|Member|
|:---|
|аттестовка|
|notAttested|

### <a name="authenticationmethodtargettype-values"></a>Значения authenticationMethodTargetType

|Member|
|:---|
|user|
|group;|

### <a name="authenticationmethodstate-values"></a>Значения authenticationMethodState

|Member|
|:---|
|включено|
|отключено|

### <a name="microsoftauthenticatorauthenticationmode-values"></a>Значения microsoftAuthenticatorAuthenticationMode

|Member|
|:---|
|любой|
|Нажмите|
|deviceBasedPush|

### <a name="keystrength-values"></a>Значения keyStrength

|Member|
|:---|
|Нормальной|
|Слабым|
|unknown|

### <a name="authenticationmethodkeystrength-values"></a>Значения authenticationMethodKeyStrength

|Member|
|:---|
|Нормальной|
|Слабым|
|unknown|

### <a name="allowinvitesfrom-values"></a>Значения allowInvitesFrom

|Member|
|:---|
|none|
|adminsAndGuestInviters|
|adminsGuestInvitersAndAllMembers|
|Все|
|unknownFutureValue|

### <a name="datapolicyoperationstatus-values"></a>Значения dataPolicyOperationStatus

|Member|
|:---|
|notStarted|
|Запущена|
|complete|
|Сбой при|
|unknownFutureValue|

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
|unknownFutureValue|

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

### <a name="conditionalaccessclientapp-values"></a>Значения conditionalAccessClientApp

|Member|
|:---|
|все|
|Обозреватель|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|Других|
|unknownFutureValue|

### <a name="conditionalaccesspolicystate-values"></a>Значения conditionalAccessPolicyState

|Member|
|:---|
|включено|
|отключено|
|enabledForReportingButNotEnforced|

#### <a name="deviceprofiletype-values"></a>Значения deviceProfileType
|Member|
|:---|
|RegisteredDevice|
|SecureVM|
|Принтер|
|Shared|
|Iot|

### <a name="appliedconditionalaccesspolicyresult-values"></a>Значения appliedConditionalAccessPolicyResult 

|Member|
|:---|
|success|
|Сбоя|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|

### <a name="grouptype-values"></a>Значения groupType 

|Member|
|:---|
|unifiedGroups|
|AzureAD|
|unknownFutureValue|

### <a name="conditionalaccessstatus-values"></a>Значения conditionalAccessStatus

|Member|
|:---|
|success|
|Сбоя|
|notApplied|
|unknownFutureValue|

### <a name="operationresult-values"></a>Значения operationResult

|Member|
|:---|
|success|
|Сбоя|
|timeout|
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

### <a name="mediastate-values"></a>Значения mediaState

|Member|
|:---|
|Активных|
|Неактивные|
|unknownFutureValue|

### <a name="basicstatus-values"></a>Значения basicStatus

|Member|
|:---|
|Активных|
|Неактивные|

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

### <a name="calltype-values"></a>Значения callType

|Member|
|:---|
|unknown|
|groupCall|
|peerToPeer|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>значения educationAddToCalendarOptions
|Member|
|:---|
|none|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationsubmissionstatus-values"></a>значения educationSubmissionStatus
|Member|
|:---|
|Работает|
|Представлены|
|Выпущен|
|Возвращены|
|unknownFutureValue|
|Переназначить|

### <a name="onlinemeetingrole-values"></a>Значения onlineMeetingRole

|Member|
|:---|
|attendee|
|Ведущий|
|unknownFutureValue|

### <a name="modality-values"></a>значения модальности 

|Member|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="calldirection-values"></a>Значения callDirection

|Member|
|:---|
|Входящих|
|Исходящих|

### <a name="signinaudience-values"></a>Значения signInAudience

|Member|
|:---|
|AzureADMyOrg|
|AzureADMultipleOrgs|
|AzureADandPersonalMicrosoftAccount|
|PersonalMicrosoftAccount|

### <a name="groupmembershipclaims-values"></a>Значения groupMembershipClaims

|Member|
|:---|
|Нет|
|SecurityGroup|
|Все|

### <a name="recipientscopetype-values"></a>Значения recipientScopeType

|Member|
|:---|
|none|
|Внутренние|
|Внешних|
|externalPartner|
|externalNonPartner|

### <a name="activitytype-values"></a>Значения activityType

|Member|
|:---|
|Signin|
|user|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>Значения riskDetectionTimingType

|Member|
|:---|
|notDefined|
|Realtime|
|nearRealtime|
|Автономных|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>Значения tokenIssuerType

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="attachmenttype-values"></a>Значения attachmentType

| Member
|:--------------
| file
| item
| справочник

### <a name="contactrelationship-values"></a>Значения объекта contactRelationship

|Элемент|Значение|Описание|
|:---|:---|:---|
|родитель|0|Родительский элемент пользователя.|
|Относительно|1| Относительный пользователь.|
|Помощник|2| Aide пользователя.|
|Доктор|3| Пользователь должен быть доктором.|
|Опекуна|4| Защитник пользователя.|
|child|5| Дочерний элемент пользователя.|
|Других|6| Неопределенная связь с пользователем.|
|unknownFutureValue|7 | Значение маркера для обеспечения совместимости в будущем.|

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
|none|
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

### <a name="workforceintegrationencryptionprotocol-values"></a>значения workforceIntegrationEncryptionProtocol

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>значения workforceIntegrationSupportedEntities

|Member|
|:---|
|none|
|shift|
|swapRequest|
|userShiftPreferences|
|openShift|
|openShiftRequest|
|offerShiftRequest|
|unknownFutureValue|

### <a name="timezonestandard-values"></a>Значения timeZoneStandard

| Member
|:-----------------
| windows
| Iana


### <a name="freebusystatus-values"></a>значения freeBusyStatus

| Элемент            |Значение
|:------------------|:-------
| Бесплатный              | 0
| Предварительный         | 1
| Занят              | 2
| Oof               | 3
| workingElsewhere  | 4
| unknown           | –1


### <a name="attendeetype-values"></a>Значения attendeeType

| Member
|:-------------------------
| Обязательный
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>Значения externalAudienceScope

| Member
|:-------------------------
| none
| contactsOnly
| все


### <a name="automaticrepliesstatus-values"></a>Значения automaticRepliesStatus

| Member
|:-------------------------
| отключено
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>Значения calendarColor

| Элемент     | Значение
|:-----------|:----------
| Авто       | –1
| lightBlue  | 0
| lightGreen | 1
| lightOrange| 2
| lightGray  | 3
| lightYellow| 4
| lightTeal  | 5
| lightPink  | 6
| lightBrown | 7 
| lightRed   | 8 
| maxColor   | 9 

### <a name="educationexternalsource-values"></a>значения educationExternalSource

| Member             |
| :----------------- |
| Sis                |
| Вручную             |
| unknownFutureValue |

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

| Member             |
| :----------------- |
| student            |
| teacher            |
| none               |
| unknownFutureValue |

### <a name="meetingmessagetype-values"></a>Значения meetingMessageType

| Member
|:-----------------
| none
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
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
| none

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

| Элемент      | Значение
|:------------|:------------
| Владелец       | 0
| Участник | 1
| Читатель      | 2
| Нет        | –1


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


### <a name="plannercontainertype-values"></a>Значения plannerContainerType

|Member|
|:---|
|group|
|unknownFutureValue|
|состав|


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
| Неизвестно
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>Значения responseType

| Member
|:-------------------------
| none
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

| Элемент   |Значение
|:---------|:--------
| none     | –1
| preset0  | 0
| preset1  | 1
| preset2  | 2
| preset3  | 3
| preset4  | 4
| preset5  | 5
| preset6  | 6
| preset7  | 7 
| preset8  | 8 
| preset9  | 9 
| preset10 | 10
| preset11 | 11
| preset12 | 12 
| preset13 | 13
| preset14 | 14
| preset15 | 15
| preset16 | 16
| preset17 | 17 
| preset18 | 18 
| preset19 | 19
| preset20 | 20
| preset21 | 21
| preset22 | 22
| preset23 | 23
| preset24 | 24

### <a name="alertfeedback-values"></a>Значения alertFeedback

Возможные значения обратной связи в оповещении, предоставляемом аналитиком.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|truePositive|1|Оповещение имеет истинно положительный результат.|
|falsePositive|2| Оповещение имеет ложное срабатывание.|
|benignPositive|3| Оповещение неопасно-положительное.|

### <a name="filehashtype-values"></a>Значения fileHashType

Перечисление для типов хэша файлов.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип.|
|sha1|1|Тип хэша SHA1.|
|sha256|2| Тип хэша SHA256.|
|md5|3| Тип хэша MD5.|
|authenticodeHash256|4| Тип хэша AuthenticodeHash256.|
|lsHash|5| Тип хэша LsHash.|
|CTPH|6| Тип хэша CTPH.|
|peSha1|7 | Тип хэша PESHA1.|
|peSha256|8 | Тип хэша PESHA256.|

### <a name="connectiondirection-values"></a>значения connectionDirection

Перечисление для направления сетевого подключения (входящего и исходящего).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное соединение.|
|Входящих|1|Входящее подключение.|
|Исходящих|2| Исходящее подключение.|

### <a name="connectionstatus-values"></a>Значения connectionStatus

Перечисление состояния подключений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное состояние подключения.|
|Попытка|1|Попытка подключения.|
|Удалось|2| Подключение выполнено успешно.|
|Заблокирован|3| Подключение заблокировано.|
|Сбой при|4| Сбой подключения.|

### <a name="processintegritylevel-values"></a>Значения processIntegrityLevel

Возможные значения уровня целостности процесса.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|Ненадежных|10|Уровень целостности ненадежный.|
|Низкой|20| Уровень целостности низкий.|
|medium|30| Уровень целостности — средний.|
|Высокой|40| Уровень целостности — Высокий.|
|system|50| Уровень целостности — System.|

### <a name="registryhive-values"></a>значения registryHive

Перечисление для кустов реестра, определяемых [/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный куст.|
|currentConfig|1|HKEY_CURRENT_CONFIG hive.|
|Currentuser|2| HKEY_CURRENT_USER hive.|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM hive.|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software hive.|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System hive.|
|usersDefault|6| \\HKEY_USERS. Куст DEFAULT.|

### <a name="registryoperation-values"></a>Значения registryOperation

Операция, которая изменила имя и (или) значение раздела реестра.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|create|1|Создайте реестр.|
|Изменить|2|Изменение реестра.|
|delete|3|Удаление реестра.|

### <a name="registryvaluetype-values"></a>Значения registryValueType

Перечисление для типов значений реестра, определяемых [типами /windows/desktop/sysinfo/registry-value-types](/windows/desktop/sysinfo/registry-value-types).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|двоичный|1|REG_BINARY типа значения реестра.|
|Dword|2| REG_DWORD типа значения реестра.|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN типа значения реестра.|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN типа значения реестра.|
|expandSz|5| REG_EXPAND_SZ типа значения реестра.|
|ссылка|6| REG_LINK типа значения реестра.|
|multiSz|7 | REG_MULTI_SZ типа значения реестра.|
|none|8 | REG_NONE типа значения реестра.|
|qword|9 | REG_QWORD типа значения реестра.|
|qwordlittleEndian|10| REG_QWORD_LITTLE_ENDIAN типа значения реестра.|
|Sz|11| REG_SZ типа значения реестра.|

### <a name="alertseverity-values"></a>Значения alertSeverity

Перечисление серьезности оповещений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Уровень серьезности неизвестен.|
|Информационных|1|Уровень серьезности предназначен только для сведений.|
|Низкой|2| Уровень серьезности низкий.|
|medium|3| Уровень серьезности — средний.|
|Высокой|4| Серьезность высокая.|

### <a name="alertstatus-values"></a>Значения alertStatus

Возможные значения состояния жизненного цикла оповещений (стадии).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное состояние.|
|newAlert|10| Оповещение является новым.|
|Inprogress|20|Оповещение выполняется.|
|resolved|30|Оповещение разрешается.|

### <a name="emailrole-values"></a>Значения emailRole
Возможные значения для ролей электронной почты.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестная роль.|
|sender|1|Отправитель сообщения электронной почты.|
|получатель;|2|Получатель сообщения электронной почты.|

### <a name="logontype-values"></a>Значения logonType

Возможные значения для метода входа пользователя.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|Интерактивная|0|Вход является интерактивным.|
|remoteInteractive|1| Вход в систему является удаленным интерактивным.|
|Сети|2| Вход в систему — это сеть.|
|batch|3| Вход выполняется пакетно.|
|служба|4| Вход — это служба.|

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группах) для определения Windows.

|Member|Member|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|стандарт|0|Член группы "Стандартные пользователи".|
|Мощность|1| Член группы Power Users.|
|Администратора|2| Член группы "Администраторы".|

### <a name="riskdetail-values"></a>Значения riskDetail

|Member|
|:---|
|none|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninCompromised|
|adminConfirmedUserComprommed|
|hidden|
|unknownFutureValue|

### <a name="riskeventtypes-values"></a>Значения riskEventTypes

| Member
|:-------------------------
| unlikelyTravel
| anonymizedIPAddress
| maliciousIPAddress
| unfamiliarFeatures
| malwareInfectedIPAddress
| suspiciousIPAddress
| leakedCredentials
| investigationsThreatIntelligence
| Универсальный
| unknownFutureValue

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

### <a name="risklevel-values"></a>Значения riskLevel

| Member
|:-------------------------
| none
| Низкой
| medium
| Высокой
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>Значения riskState

| Member
|:-------------------------
| none
| confirmedSafe
| исправлено
| Уволен
| atRisk
| confirmedCompromised
| unknownFutureValue

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|RestId|
|restImmutableEntryId|

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
|none|
|freeBusyRead|
|limitedRead|
|read|
|write|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|Пользовательские|

### <a name="threatassessmentcontenttype-values"></a>Значения threatAssessmentContentType

| Элемент | Значение | Описание             |
|:-------|:------|:------------------------|
| почта;   | 1     | Почтовая угроза.            |
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
| user          | 1     | Отправка пользователя.         |
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
| none                  | 0     | Пока не известно.                       |
| mailFlowRule          | 1     | Правило транспорта Exchange.            |
| safeSender            | 2     | Список надежных отправителей.                   |
| blockedSender         | 3     | Список заблокированных отправителей.                |
| advancedSpamFiltering | 4     | Расширенный параметр фильтрации нежелательной почты.     |
| domainAllowList       | 5     | Список разрешений домена отправителя.           |
| domainBlockList       | 6     | Список блоков домена отправителя.           |
| notInAddressBook      | 7      | Исключить отправителя не в адресной книге. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправителя.   |
| autoPurgeToInbox      | 9      | Перемещение сообщения TimeTravel в папку "Входящие".   |
| autoPurgeToJunk       | 10    | Перемещение сообщения TimeTravel в нежелательное.    |
| autoPurgeToDeleted    | 11    | Сообщение о перемещении TimeTravel в удаленное. |
| Исходящих              | 12     | Исходящая почта.                      |
| notJunk               | 13    | Разрешить из-за нежелательной почты.              |
| Нежелательной                  | 14    | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15    | Элемент sentinel.                  |

### <a name="chatmessagetype-values"></a>Значения chatMessageType

| Значение |
|:-----------------|
| message |
| chatEvent |
| Ввода |
| unknownFutureValue |
| systemEventMessage |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>Значения chatMessagePolicyViolationDlpActionType

| Значение |
|:-----------------|
| none |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

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

### <a name="channelmembershiptype-values"></a>Значения channelMembershipType

| Элемент             | Значение |Описание|
| :----------------- | :---- |:-----------|
| стандарт           | 0     |Канал наследует список участников родительской команды.|
| Частная            | 1     |Канал может содержать участников, которые являются подмножеством всех участников родительской команды.|
| unknownFutureValue | 2     |      |
### <a name="wellknownlistname-values"></a>Значения wellknownListName
| Member
|:----------------------
| none
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
|Примечание| Многострочный текст. |
|текст | Однострочный текст. |
|Выбор | Колонка выбора |
|multichoice | Столбец multichoice. |
|число | Числовая гистограмма. |
|Валюты | Столбец валюты. |
|dateTime | Столбец DateTime. |
|Поиска | Столбец подстановки. |
|логический | Столбец "Да" или "Нет". |
|user | Столбец пользователя или группы. |
|url | Гиперссылка или столбец рисунка. |
|Рассчитывается | Вычисляемый столбец. |
|расположение | Столбец расположения. |
|географическое положение | Столбец географического расположения. |
|term | Столбец управляемых метаданных. |
|многотерминантная | Столбец управляемых метаданных, который принимает несколько значений. |
|Миниатюру | Столбец изображения. |
|approvalStatus | Столбец состояния утверждения контента. |
|unknownFutureValue | UnknownFuturevalue |

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

### <a name="printcolormode-values"></a>Значения printColorMode 

|Member|
|:---|
|blackAndWhite|
|Оттенках серого|
|color|
|Авто|
|unknownFutureValue|

### <a name="printduplexmode-values"></a>Значения printDuplexMode 

|Member|
|:---|
|FlipOnLongEdge|
|FlipOnShortEdge|
|oneSided|
|unknownFutureValue|

### <a name="printerfeedorientation-values"></a>Значения printerFeedOrientation 

|Member|
|:---|
|longEdgeFirst|
|shortEdgeFirst|
|unknownFutureValue|

### <a name="printfinishing-values"></a>значения printFinishing 

|Member|
|:---|
|none|
|Основных|
|Удар|
|Крышка|
|Привязки|
|saddleStitch|
|совмещаемая|
|stapleTopLeft;|
|stapleBottomLeft;|
|stapleTopRight|
|основные боттомыRight|
|совмещатьLeftEdge|
|совмещаемая таблица|
|висячее|
|stitchBottomEdge|
|stapleDualLeft;|
|stapleDualTop;|
|stapleDualRight;|
|stapleDualBottom;|
|unknownFutureValue|

### <a name="printmultipagelayout-values"></a>Значения printMultipageLayout 

|Member|
|:---|
|clockwiseFromTopLeft|
|counterclockwiseFromTopLeft|
|counterclockwiseFromTopRight|
|clockwiseFromTopRight|
|counterclockwiseFromBottomLeft|
|clockwiseFromBottomLeft|
|counterclockwiseFromBottomRight|
|clockwiseFromBottomRight|
|unknownFutureValue|

### <a name="printorientation-values"></a>Значения printOrientation 

|Member|
|:---|
|Портрет|
|Пейзаж|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>Значения printQuality 

|Member|
|:---|
|Низкой|
|medium|
|Высокой|
|unknownFutureValue|

### <a name="printscaling-values"></a>значения printScaling 

|Member|
|:---|
|Авто|
|shrinkToFit|
|fill|
|Подходят|
|none|
|unknownFutureValue|

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

### <a name="identityuserflowattributedatatype-values"></a>Значения identityUserFlowAttributeDataType

| Member                |
|:----------------------|
| Строка                |
| логический               |
| int64                 |
| Stringcollection      |
| dateTime              |
| unknownFutureValue    |

### <a name="identityuserflowattributetype-values"></a>Значения identityUserFlowAttributeType

| Member                |
|:----------------------|
| Builtin               |
| Пользовательские                |
| обязательно              |
| unknownFutureValue    |

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

| Member    |
| :-------- |
| entityUrl |
| текст      |


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

### <a name="provisioningstatuserrorcategory-values"></a>Значения provisioningStatusErrorCategory 

|Member|
|:---|
|Сбоя|
|nonServiceFailure|
|success|
|unknownFutureValue|

### <a name="provisioningaction-values"></a>Значения provisioningAction 

|Member|
|:---|
|Других|
|create|
|delete|
|отключение|
|Обновление|
|stagedDelete|
|unknownFutureValue|


### <a name="initiatortype-values"></a>Значения initiatorType 

|Member|
|:---|
|user|
|приложение|
|system|
|unknownFutureValue|

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
|Канал|
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

### <a name="posttype-values"></a>Значения postType 

|Member|
|:---|
|Регулярные|
|Быстрый|
|Стратегических|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>Значения searchAlterationType

| Member |
|:---------------|
|Модификация|
|Предложение|

### <a name="servicehealthclassificationtype-values"></a>Значения serviceHealthClassificationType 

|Member|
|:---|
|Консультативный|
|Инцидента|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>Значения serviceHealthOrigin 

|Member|
|:---|
|microsoft|
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

### <a name="advancedconfigstate-values"></a>Значения advancedConfigState 

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="callrecordingstatus-values"></a>Значения callRecordingStatus 

|Member|
|:---|
|success|
|Сбоя|
|Первоначального|
|chunkFinished|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>Значения teamworkCallEventType 

|Member|
|:---|
|call|
|Конференц|
|screenShare|
|unknownFutureValue|

### <a name="bookingreminderrecipients-values"></a>Значения bookingReminderRecipients 

|Member|
|:---|
|allAttendees|
|Персонал|
|Клиентов|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>Значения bookingStaffRole 

|Member|
|:---|
|Гостевой|
|Администратора|
|Просмотра|
|externalGuest|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>Значения answerInputType 

|Member|
|:---|
|текст|
|Radiobutton|
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

### <a name="authenticationprotocol-values"></a>Значения authenticationProtocol 

|Member|
|:---|
|wsFed|
|Saml|

### <a name="longrunningoperationstatus-values"></a>Значения longRunningOperationStatus

| Member|
|:-----------------|
|notStarted|
|Запущена|
|Удалось|
|Сбой при|
|unknownFutureValue|
