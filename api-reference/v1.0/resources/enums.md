---
title: Значения Enum
description: Значения Graph майкрософт.
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: a85865ca6eba3aad8899cd48cdb65ca56e28e1c9
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608053"
---
# <a name="enum-values"></a>Значения Enum

Пространство имен: microsoft.graph

### <a name="accessreviewexpirationbehavior-values"></a>accessReviewExpirationBehavior значения

|Member|
|:---|
|keepAccess|
|removeAccess|
|acceptAccessRecommendation|
|unknownFutureValue|

### <a name="allowedtargetscope-values"></a>значения allowedTargetScope

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

### <a name="approvalfilterbycurrentuseroptions-values"></a>значения approvalFilterByCurrentUserOptions 

|Member|
|:---|
|target|
|createdBy|
|одобрение|
|unknownFutureValue|

### <a name="accesspackageassignmentfilterbycurrentuseroptions-values"></a>accessPackageAssignmentFilterByCurrentUserOptions

|Member|
|:---|
|target|
|createdBy|
|unknownFutureValue|

### <a name="accesspackageassignmentrequestfilterbycurrentuseroptions-values"></a>accessPackageAssignmentRequestFilterByCurrentUserOptions

|Member|
|:---|
|target|
|createdBy|
|одобрение|
|unknownFutureValue|

### <a name="accesspackageassignmentstate-values"></a>значения accessPackageAssignmentState

|Member|
|:---|
|доставка|
|partiallyDelivered|
|доставлено|
|истек срок действия|
|deliveryFailed|
|unknownFutureValue|

### <a name="accesspackagecatalogstate-values"></a>значения accessPackageCatalogState

|Member|
|:---|
|неопубликованный|
|опубликовано|
|unknownFutureValue|

### <a name="accesspackagecatalogtype-values"></a>значения accessPackageCatalogType

|Member|
|:---|
|userManaged|
|serviceDefault|
|serviceManaged|
|unknownFutureValue|

### <a name="accesspackageexternaluserlifecycleaction-values"></a>значения accessPackageExternalUserLifecycleAction

|Member|
|:---|
|Нет|
|blockSignIn|
|blockSignInAndDelete|
|unknownFutureValue|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>значения accessPackageFilterByCurrentUserOptions

|Member|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="accesspackagerequeststate-values"></a>значения accessPackageRequestState

|Member|
|:---|
|отправлено|
|pendingApproval|
|доставка|
|доставлено|
|deliveryFailed|
|denied|
|scheduled|
|отменено|
|partiallyDelivered|
|unknownFutureValue|

### <a name="accesspackagerequesttype-values"></a>значения accessPackageRequestType

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

### <a name="accesspackagesubjecttype-values"></a>значения accessPackageSubjectType

|Member|
|:---|
|notSpecified|
|user|
|servicePrincipal|
|unknownFutureValue|

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState

|Member|
|:---|
|настроенный|
|предложено|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>accessReviewInstanceDecisionItemFilterByCurrentUserOptions 

|Member|
|:---|
|рецензент|
|unknownFutureValue|

### <a name="volumetype-values"></a>значения volumeType

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="filtermode-values"></a>значения filterMode

|Member|
|:---|
|включить|
|исключение|

### <a name="lifecycleeventtype-values"></a>значения lifecycleEventType

|Member|
|:---|
|пропущено|
|subscriptionRemoved|
|reauthorizationRequired|

### <a name="changetype-values"></a>значения changeType

|Member|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="countrylookupmethodtype-values"></a>значения countryLookupMethodType

|Member|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>consentRequestFilterByCurrentUserOptions 

|Member|
|:---|
|рецензент|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>значения externalEmailOtpState

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>значения educationAddedStudentAction

|Member|
|:---|
|Нет|
|assignIfOpen|
|unknownFutureValue|

### <a name="fido2restrictionenforcementtype-values"></a>значения fido2RestrictionEnforcementType

|Member|
|:---|
|разрешить|
|block|

### <a name="attestationlevel-values"></a>значения attestationLevel

|Member|
|:---|
|засвидетель-|
|notAttested|

### <a name="authenticationmethodtargettype-values"></a>Значения authenticationMethodTargetType

|Member|
|:---|
|user|
|group;|

### <a name="authenticationmethodstate-values"></a>значения authenticationMethodState

|Member|
|:---|
|включено|
|отключено|

### <a name="microsoftauthenticatorauthenticationmode-values"></a>значения MicrosoftAuthenticatorAuthenticationMode

|Member|
|:---|
|любой|
|push|
|deviceBasedPush|

### <a name="keystrength-values"></a>значения keyStrength

|Member|
|:---|
|нормальный|
|слабый|
|unknown|

### <a name="authenticationmethodkeystrength-values"></a>значения authenticationMethodKeyStrength

|Member|
|:---|
|нормальный|
|слабый|
|unknown|

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom values

|Member|
|:---|
|Нет|
|adminsAndGuestInviters|
|adminsGuestInvitersAndAllMembers|
|все|
|unknownFutureValue|

### <a name="datapolicyoperationstatus-values"></a>значения dataPolicyOperationStatus

|Member|
|:---|
|notStarted|
|запуск|
|complete|
|не удалось|
|unknownFutureValue|

### <a name="conditionalaccessdeviceplatform-values"></a>значения conditionalAccessDevicePlatform

| Member       |
|:--------------|
|Android|
|iOS|
|windows|
|WindowsPhone|
|macOS|
|все|
|unknownFutureValue|

### <a name="signinfrequencytype-values"></a>значения signinFrequencyType

| Member       |
|:--------------|
|days|
|часы|

### <a name="persistentbrowsersessionmode-values"></a>persistentBrowserSessionMode values

| Member       |
|:--------------|
|всегда|
|никогда|

### <a name="cloudappsecuritysessioncontroltype-values"></a>значения cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|
|unknownFutureValue|

### <a name="conditionalaccessgrantcontrol-values"></a>значения conditionalAccessGrantControl

| Member       |
|:--------------|
|block|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|
|passwordChange|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>значения conditionalAccessClientApp

|Member|
|:---|
|все|
|Обозреватель|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|другие|
|unknownFutureValue|

### <a name="conditionalaccesspolicystate-values"></a>значения conditionalAccessPolicyState

|Member|
|:---|
|включено|
|отключено|
|enabledForReportingButNotEnforced|

#### <a name="deviceprofiletype-values"></a>значения deviceProfileType
|Member|
|:---|
|RegisteredDevice|
|SecureVM|
|Принтер|
|Shared|
|IoT|

### <a name="appliedconditionalaccesspolicyresult-values"></a>appliedConditionalAccessPolicyResult values 

|Member|
|:---|
|success|
|сбой|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|

### <a name="grouptype-values"></a>значения groupType 

|Member|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="conditionalaccessstatus-values"></a>значения conditionalAccessStatus

|Member|
|:---|
|success|
|сбой|
|notApplied|
|unknownFutureValue|

### <a name="operationresult-values"></a>значения operationResult

|Member|
|:---|
|success|
|сбой|
|timeout|
|unknownFutureValue|

### <a name="tone-values"></a>значения тона

|Member|
|:---|
|tone0|
|tone1|
|tone2|
|tone3|
|tone4|
|tone5|
|tone6|
|tone7|
|tone8|
|tone9|
|звезда|
|pound|
|a|
|b|
|c|
|d|
|flash|

### <a name="mediastate-values"></a>значения mediaState

|Member|
|:---|
|active|
|неактивно|
|unknownFutureValue|

### <a name="basicstatus-values"></a>значения basicStatus

|Member|
|:---|
|active|
|неактивно|

### <a name="callstate-values"></a>значения callState

|Member|
|:---|
|входящий|
|создание|
|звон|
|установлено|
|удержание|
|перенос|
|transferAccepted|
|перенаправление|
|прекращение|
|прекращено|

### <a name="calltype-values"></a>значения callType

|Member|
|:---|
|unknown|
|groupCall|
|peerToPeer|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>значения educationAddToCalendarOptions
|Member|
|:---|
|Нет|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationsubmissionstatus-values"></a>значения educationSubmissionStatus
|Member|
|:---|
|работа|
|отправлено|
|выпущено|
|возвращено|
|unknownFutureValue|
|перенаписано|

### <a name="onlinemeetingrole-values"></a>значения onlineMeetingRole

|Member|
|:---|
|attendee|
|presenter|
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

### <a name="calldirection-values"></a>значения callDirection

|Member|
|:---|
|входящий|
|исходяние|

### <a name="signinaudience-values"></a>Значения signInAudience

|Member|
|:---|
|AzureADMyOrg|
|AzureADMultipleOrgs|
|AzureADandPersonalMicrosoftAccount|
|PersonalMicrosoftAccount|

### <a name="groupmembershipclaims-values"></a>значения groupMembershipClaims

|Member|
|:---|
|Нет|
|SecurityGroup|
|Все|

### <a name="recipientscopetype-values"></a>значения recipientScopeType

|Member|
|:---|
|Нет|
|внутренний|
|внешние|
|externalPartner|
|externalNonPartner|

### <a name="activitytype-values"></a>значения activityType

|Member|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>значения riskDetectionTimingType

|Member|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|автономный режим|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>значения tokenIssuerType

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

### <a name="contactrelationship-values"></a>значения contactRelationship

|Элемент|Значение|Описание|
|:---|:---|:---|
|родитель|0|Родитель пользователя.|
|относительный|1| Родственник пользователя.|
|помощник|2| Помощник пользователя.|
|врач|3| Врач пользователя.|
|guardian|4| Хранитель пользователя.|
|child|5| Ребенок пользователя.|
|другие|6 | Неустановленное отношение к пользователю.|
|unknownFutureValue|7 | Значение маркера для будущей совместимости.|

### <a name="scheduleentitytheme-values"></a>значения scheduleEntityTheme

| Member
|:-------------------------
| white
| blue
| green
| purple
| pink
| yellow
| серый
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>значения timeOffReasonIconType

|Member|
|:---|
|Нет|
|автомобиль|
|calendar|
|запуск|
|плоскость|
|firstAid|
|врач|
|notWorking|
|часы|
|juryDuty|
|глобус|
|чашка|
|phone|
|погода|
|зонт|
|piggyBank|
|собака|
|торт|
|trafficCone|
|пин-код|
|солнечный|
|unknownFutureValue|

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

### <a name="timezonestandard-values"></a>значения timeZoneStandard

| Member
|:-----------------
| windows
| iana


### <a name="freebusystatus-values"></a>значения freeBusyStatus

| Элемент            |Значение
|:------------------|:-------
| бесплатно              | 0
| предварительная         | 1
| занят              | 2
| oof               | 3
| workingElsewhere  | 4
| unknown           | –1


### <a name="attendeetype-values"></a>значения attendeeType

| Member
|:-------------------------
| обязательно
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>значения externalAudienceScope

| Member
|:-------------------------
| Нет
| contactsOnly
| все


### <a name="automaticrepliesstatus-values"></a>значения automaticRepliesStatus

| Member
|:-------------------------
| отключено
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>значения calendarColor

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
| sis                |
| Вручную             |
| unknownFutureValue |

### <a name="educationgender-values"></a>значения educationGender

| Member
|:-------------------------
| женский
| мужской
| другие
| unknownFutureValue


### <a name="eventtype-values"></a>значения eventType

| Member
|:-------------------------
| singleInstance
| возникновение
| исключение
| seriesMaster


### <a name="sensitivity-values"></a>значения чувствительности

| Member
|:-------------------------
| нормальный
| personal
| частный
| конфиденциальность


### <a name="importance-values"></a>значения важности

| Member
|:-------------------------
| низкий
| нормальный
| высокая

### <a name="educationuserrole-values"></a>значения educationUserRole

| Member             |
| :----------------- |
| student            |
| teacher            |
| Нет               |
| unknownFutureValue |

### <a name="meetingmessagetype-values"></a>значения meetingMessageType

| Member
|:-----------------
| Нет
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus values

| Member
|:-------------------------
| notFlagged
| complete
| помечено


### <a name="inferenceclassificationtype-values"></a>значения inferenceClassificationType

| Member
|:-----------------
| сфокусировано
| другие


### <a name="iosnotificationalerttype-values"></a>значения iosNotificationAlertType

| Member
|:-------------------------
| deviceDefault
| баннер
| modal
| Нет

### <a name="deviceenrollmentfailurereason-values"></a>значения deviceEnrollmentFailureReason

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


### <a name="bodytype-values"></a>значения bodyType
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
| отель
| ресторан
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>значения locationUniqueIdType

| Member
|:-------------------------
| unknown
| locationStore
| каталог
| частный
| bing


### <a name="messageactionflag-values"></a>значения messageActionFlag

| Member
|:-------------------------
| любой
| call
| doNotForward
| followUp
| fyi
| forward
| noResponseNecessary
| read
| reply
| replyToAll
| обзор


### <a name="onenoteuserrole-values"></a>значения onenoteUserRole

| Элемент      | Значение
|:------------|:------------
| Владелец       | 0
| Участник | 1
| Reader      | 2
| Нет        | –1


### <a name="operationstatus-values"></a>значения operationStatus

| Member
|:-----------------
|NotStarted
|Работает
|Завершено
|Не выполнено


### <a name="onenotepatchactiontype-values"></a>значения onenotePatchActionType

| Member
|:-------------------------
| Заменить
| Приложение
| Удалить
| Вставка
| Prepend

### <a name="onenotepatchinsertposition-values"></a>значения onenotePatchInsertPosition

| Member
|:-------------------------
| После
| До


### <a name="phonetype-values"></a>значения phoneType

| Member
|:-------------------------
| главная
| бизнес
| мобильный
| другие
| помощник
| homeFax
| businessFax
| otherFax
| pager
| радио


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
| active
| обновлено
| deleted
| пропущено
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex values

| Member
|:-------------------------
| во-первых
| во-вторых
| третий
| четвертый
| последний


### <a name="dayofweek-values"></a>значения dayOfWeek

| Member
|:-------------------------
| воскресенье
| понедельник
| вторник
| среда
| четверг
| пятница
| суббота

### <a name="recurrencepatterntype-values"></a>значения recurrencePatternType

| Member
|:-------------------------
| ежедневно
| еженедельно
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>значения recurrenceRangeType

| Member
|:-------------------------
| endDate
| noEnd
| про номера


### <a name="onenotesourceservice-values"></a>значения onenoteSourceService
| Member
|:---------------------
| Неизвестно
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>Значения responseType

| Member
|:-------------------------
| Нет
| organizer
| предварительноAccepted
| принято
| отклонено
| notResponded


### <a name="activitydomain-values"></a>значения activityDomain

| Member
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>Значения websiteType

| Member
|:-------------------------
| другие
| главная
| work
| Блог
| profile


### <a name="categorycolor-values"></a>значения categoryColor

| Элемент   |Значение
|:---------|:--------
| Нет     | –1
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

### <a name="alertfeedback-values"></a>значения alertFeedback

Возможные значения обратной связи в оповещении, предоставляемом аналитиком.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|truePositive|1|Оповещение — это верно-положительно.|
|falsePositive|2| Оповещение является ложным срабатывательным.|
|benignPositive|3| Оповещение является доброкачественным.|

### <a name="filehashtype-values"></a>значения fileHashType

Enum для типов hash файла.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип.|
|sha1|1|Тип hash SHA1.|
|sha256|2| Тип hash SHA256.|
|md5|3| Тип hash MD5.|
|authenticodeHash256|4| Тип hash AuthenticodeHash256.|
|lsHash|5| Тип hash LsHash.|
|ctph|6 | Тип хаши CTPH.|
|peSha1|7 | Тип hash PESHA1.|
|peSha256|8 | Тип hash PESHA256.|

### <a name="connectiondirection-values"></a>значения connectionDirection

Enum для направления сетевого подключения (входящие и исходящие).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное подключение.|
|входящий|1|Входящий подключение.|
|исходящие|2| Исходящие подключения.|

### <a name="connectionstatus-values"></a>значения connectionStatus

Enum для состояния подключений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние неизвестного подключения.|
|попытка|1|Попытка подключения.|
|успешно|2| Подключение удалось.|
|заблокировано|3| Подключение заблокировано.|
|не удалось|4| Сбой подключения.|

### <a name="processintegritylevel-values"></a>значения processIntegrityLevel

Возможные значения уровня целостности процесса.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|ненарушенной|10 |Уровень целостности не соответствует действительности.|
|низкий|20| Уровень целостности низкий.|
|medium|30| Уровень целостности — средний.|
|высокая|40| Уровень целостности — высокий.|
|system|50| Уровень целостности — system.|

### <a name="registryhive-values"></a>Значения registryHive

Enum для ульев реестра, определяемого [/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный улей.|
|currentConfig|1|HKEY_CURRENT_CONFIG улей.|
|currentUser|2| HKEY_CURRENT_USER улей.|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM улей.|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software улей.|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System улей.|
|usersDefault|6 | \\HKEY_USERS. Улей DEFAULT.|

### <a name="registryoperation-values"></a>Значения registryOperation

Операция, изменивла имя и/или значение ключа реестра.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|create|1|Создание реестра.|
|изменение|2|Изменение реестра.|
|delete|3|Удаление реестра.|

### <a name="registryvaluetype-values"></a>значения registryValueType

Enum для типов значений реестра, определяемого [типами /windows/desktop/sysinfo/registry-value-types](/windows/desktop/sysinfo/registry-value-types).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|двоичный|1|REG_BINARY типа значения реестра.|
|dword|2| REG_DWORD типа значения реестра.|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN тип значения реестра.|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN тип значения реестра.|
|expandSz|5| REG_EXPAND_SZ типа значения реестра.|
|ссылка|6 | REG_LINK тип значения реестра.|
|multiSz|7 | REG_MULTI_SZ тип значения реестра.|
|Нет|8 | REG_NONE типа значения реестра.|
|qword|9 | REG_QWORD тип значения реестра.|
|qwordlittleEndian|10 | REG_QWORD_LITTLE_ENDIAN типа реестра.|
|sz|11| REG_SZ типа значения реестра.|

### <a name="alertseverity-values"></a>значения alertSeverity

Enum для серьезности оповещений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Серьезность неизвестна.|
|информационная|1|Строгость только для сведений.|
|низкий|2| Серьезность низкая.|
|medium|3| Серьезность является средней.|
|высокая|4| Серьезность высока.|

### <a name="alertstatus-values"></a>значения alertStatus

Возможные значения состояния жизненного цикла Alert (этап).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный статус.|
|newAlert|10 | Оповещение является новым.|
|inProgress|20|Оповещение продолжается.|
|resolved|30|Оповещение разрешено.|

### <a name="emailrole-values"></a>значения emailRole
Возможные значения ролей электронной почты.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестная роль.|
|sender|1|Отправитель электронной почты.|
|получатель;|2|Получатель электронной почты.|

### <a name="logontype-values"></a>значения logonType

Возможные значения для метода пользовательского знака.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|интерактивный|0|Logon является интерактивным.|
|remoteInteractive|1| Logon — это удаленный интерактивный.|
|сеть|2| Logon — это сеть.|
|batch|3| Logon является пакетным.|
|служба|4| Logon — это служба.|

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группе) в Windows определения.

|Member|Member|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|стандартный|0|Член группы стандартных пользователей.|
|power|1| Член группы Power Users.|
|администратор|2| Член группы Администраторы.|

### <a name="riskdetail-values"></a>значения riskDetail

|Member|
|:---|
|Нет|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|AdminConfirmedSigninCompromised|
|AdminConfirmedUserCompromised|
|hidden|
|unknownFutureValue|

### <a name="riskeventtypes-values"></a>значения riskEventTypes

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
| общий
| unknownFutureValue

### <a name="riskeventtype-values"></a>значения riskEventType

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
|общий|
|AdminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>значения riskLevel

| Member
|:-------------------------
| Нет
| низкий
| medium
| высокая
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>значения riskState

| Member
|:-------------------------
| Нет
| confirmedSafe
| исправлено
| отклонено
| atRisk
| confirmedCompromised
| unknownFutureValue

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="onlinemeetingprovidertype-values"></a>значения onlineMeetingProviderType

|Member|
|:---|
|unknown|
|SkypeForBusiness|
|SkypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>значения delegateMeetingMessageDeliveryOptions

|Member|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>значения calendarRoleType

|Member|
|:---|
|Нет|
|freeBusyRead|
|limitedRead|
|read|
|write|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|настраиваемый|

### <a name="threatassessmentcontenttype-values"></a>значения threatAssessmentContentType

| Элемент | Значение | Описание             |
|:-------|:------|:------------------------|
| почта;   | 1     | Угроза почты.            |
| url    | 2     | УГРОЗА URL-адреса.             |
| file   | 3     | Угроза файла вложения. |

### <a name="threatexpectedassessment-values"></a>значения threatExpectedAssessment

| Элемент  | Значение | Описание                       |
|:--------|:------|:----------------------------------|
| block   | 1     | Угроза должна быть заблокирована.     |
| разблокировка | 2     | Угрозу не следует блокировать. |

### <a name="threatcategory-values"></a>значения threatCategory

| Элемент             | Значение | Описание        |
|:-------------------|:------|:-------------------|
| уверенности               | 1     | Угроза нежелательной почты.       |
| степенью           | 2     | Фишинговая угроза.   |
| malware            | 3     | Угроза вредоносных программ.    |
| unknownFutureValue | 4     | Член-часовой. |

### <a name="threatassessmentstatus-values"></a>значения threatAssessmentStatus

| Элемент    | Значение | Описание                              |
|:----------|:------|:-----------------------------------------|
| ожидание   | 1     | Оценка угрозы по-прежнему продолжается. |
| завершено | 2     | Оценка угроз завершена.         |

### <a name="threatassessmentrequestsource-values"></a>значения threatAssessmentRequestSource

| Элемент        | Значение | Описание              |
|:--------------|:------|:-------------------------|
| неопределяемая     | 0     | Еще не знаю.            |
| user          | 1     | Отправка пользователя.         |
| администратор | 2     | Отправка администратора клиента. |

### <a name="threatassessmentresulttype-values"></a>значения threatAssessmentResultType

| Элемент             | Значение | Описание                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | Результат проверки политики только для оценки `mail` . |
| rescan             | 2     | Результат rescan.                                   |
| unknownFutureValue | 3     | Член-часовой.                                   |

### <a name="maildestinationroutingreason-values"></a>значения mailDestinationRoutingReason

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| Нет                  | 0     | Еще не знаю.                       |
| mailFlowRule          | 1     | Exchange правила транспорта.            |
| safeSender            | 2     | Сейф отправитель.                   |
| blockedSender         | 3     | Заблокированный список отправитель.                |
| advancedSpamFiltering | 4     | Расширенный параметр flitering нежелательной почты.     |
| domainAllowList       | 5     | Список разрешаемой области отправитель.           |
| domainBlockList       | 6      | Список блоков домена отправитель.           |
| notInAddressBook      | 7      | Исключить отправитель не в адресной книге. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправитель времени.   |
| autoPurgeToInbox      | 9      | TimeTravel перемещает сообщение в почтовый ящик.   |
| autoPurgeToJunk       | 10     | TimeTravel перемещает сообщение в нежелательное.    |
| autoPurgeToDeleted    | 11    | TimeTravel перемещает сообщение на удаление. |
| исходящие              | 12     | Исходящие сообщения.                      |
| notJunk               | 13    | Разрешить из-за не нежелательной.              |
| нежелательной                  | 14     | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15     | Член-часовой.                  |

### <a name="chatmessagetype-values"></a>значения chatMessageType

| Значение |
|:-----------------|
| message |
| chatEvent |
| ввод текста |
| unknownFutureValue |
| systemEventMessage |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>значения chatMessagePolicyViolationDlpActionType

| Значение |
|:-----------------|
| Нет |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>значения chatMessagePolicyViolationUserActionType

| Member   | Значение Int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 | Значение по умолчанию. Это значение для сообщения, если пользователь не принял действий по сообщению, заблокированного DLP. |
| Override | 1 | Отправитель переопределил вердикт сообщения и отправил сообщение в любом случае.|
| ReportFalsePositive | 2 | Отправитель сообщил об отправке сообщения администраторам как ложный срабатыв.|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>значения chatMessagePolicyViolationVerdictDetailsType

| Member   | Значение Int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 |  Пользователю не разрешается переопределять сообщение. Пользователь не может сообщать о сообщении как о ложном срабатывке, если политикаTip не предоставлена. Во всех остальных сценариях пользователь может сообщить о сообщении как о ложном срабатыве.|
| AllowFalsePositiveOverride | 1 |  Пользователю не разрешается явно переопределять блок, если он не объедин с флагами `AllowOverrideWithoutJustification` `AllowOverrideWithJustification` или флагами. Сообщение о ложном срабатывии нарушения автоматически переопределяет блок и отправляет сообщение. |
| AllowOverrideWithoutJustification | 2 | Пользователю разрешено переопределять блок и отправлять сообщение. Текст обоснования не требуется. Эксклюзив для `AllowOverrideWithJustification`. |
| AllowOverrideWithJustification | 4 |  Пользователю разрешено переопределять блок и отправлять сообщение. Требуется текст обоснования. Эксклюзив для `AllowOverrideWithoutJustification`.|

### <a name="channelmembershiptype-values"></a>Значения channelMembershipType

| Элемент             | Значение |Описание|
| :----------------- | :---- |:-----------|
| стандартный           | 0     |Канал наследует список членов родительской команды.|
| частный            | 1     |Канал может иметь членов, которые являются подмножество всех членов родительской команды.|
| unknownFutureValue | 2     |      |
### <a name="wellknownlistname-values"></a>значения wellknownListName
| Member
|:----------------------
| Нет
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>значения taskStatus
| Member
|:----------------------
| notStarted
| inProgress
| завершено
| waitingOnOthers
| отложенный

### <a name="columntypes-values"></a>значения columnTypes

|Member|Описание|
|:-------|:------
|примечание| Многоуровневый текст. |
|текст | Текст одной строки. |
|выбор | Колонка выбора |
|multichoice | Столбец Multichoice. |
|число | Столбец номеров. |
|валюта | Столбец Валюта. |
|dateTime | Столбец DateTime. |
|lookup | Столбец Lookup. |
|boolean | Столбец Да/Нет. |
|user | Столбец Person или group. |
|url | Гиперссылка или столбец изображения. |
|вычисляется | Вычисляется столбец. |
|location | Столбец Расположение. |
|геолокация | Столбец Геолокации. |
|term | Столбец управляемых метаданных. |
|многоступенчатый | Столбец управляемых метаданных с несколькими значениями. |
|эскиз | Столбец изображения. |
|approvalStatus | Столбец утверждения состояния контента. |
|unknownFutureValue | UnknownFuturevalue |

### <a name="permissionclassificationtype-values"></a>значения permissionClassificationType

| Member
|:-------
| низкий

### <a name="permissiontype-values"></a>значения permissionType

| Member
|:-------------------------
| приложение
| делегирована
| delegatedUserConsentable

### <a name="printcolormode-values"></a>printColorMode values 

|Member|
|:---|
|blackAndWhite|
|grayscale|
|color|
|Авто|
|unknownFutureValue|

### <a name="printduplexmode-values"></a>значения printDuplexMode 

|Member|
|:---|
|flipOnLongEdge|
|flipOnShortEdge|
|oneSided|
|unknownFutureValue|

### <a name="printerfeedorientation-values"></a>значения printerFeedOrientation 

|Member|
|:---|
|longEdgeFirst|
|shortEdgeFirst|
|unknownFutureValue|

### <a name="printfinishing-values"></a>printFinishing values 

|Member|
|:---|
|Нет|
|staple|
|punch|
|крышка|
|привязка|
|saddleStitch|
|stitchEdge|
|stapleTopLeft|
|stapleBottomLeft|
|stapleTopRight|
|stapleBottomRight|
|stitchLeftEdge|
|stitchTopEdge|
|stitchRightEdge|
|stitchBottomEdge|
|stapleDualLeft|
|stapleDualTop|
|stapleDualRight|
|stapleDualBottom|
|unknownFutureValue|

### <a name="printmultipagelayout-values"></a>значения printMultipageLayout 

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

### <a name="printorientation-values"></a>значения printOrientation 

|Member|
|:---|
|портрет|
|ландшафт|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>значения printQuality 

|Member|
|:---|
|низкий|
|medium|
|высокая|
|unknownFutureValue|

### <a name="printscaling-values"></a>значения printScaling 

|Member|
|:---|
|Авто|
|shrinkToFit|
|fill|
|fit|
|Нет|
|unknownFutureValue|

### <a name="userflowtype-values"></a>значения userFlowType

|Member
|:----------------------
| signUp
| signIn
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| unknownFutureValue

### <a name="identityuserflowattributedatatype-values"></a>значения identityUserFlowAttributeDataType

| Member                |
|:----------------------|
| string                |
| boolean               |
| int64                 |
| stringCollection      |
| dateTime              |
| unknownFutureValue    |

### <a name="identityuserflowattributetype-values"></a>значения identityUserFlowAttributeType

| Member                |
|:----------------------|
| builtIn               |
| настраиваемый                |
| Обязательный              |
| unknownFutureValue    |

### <a name="identityuserflowattributeinputtype-values"></a>значения identityUserFlowAttributeInputType

| Member                |
|:----------------------|
| textBox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>значения teamworkActivityTopicSource 

| Member    |
| :-------- |
| entityUrl |
| текст      |


### <a name="provisioningresult-values"></a>значения provisioningResult 

|Member|
|:---|
|success|
|сбой|
|пропущено|
|warning|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>provisioningStepType values 

|Member|
|:---|
|импорт|
|scoping|
|соответствие|
|обработка|
|referenceResolution|
|экспорт|
|unknownFutureValue|

### <a name="provisioningstatuserrorcategory-values"></a>provisioningStatusErrorCategory values 

|Member|
|:---|
|сбой|
|nonServiceFailure|
|success|
|unknownFutureValue|

### <a name="provisioningaction-values"></a>значения provisioningAction 

|Member|
|:---|
|другие|
|create|
|delete|
|отключение|
|обновление|
|stagedDelete|
|unknownFutureValue|


### <a name="initiatortype-values"></a>значения initiatorType 

|Member|
|:---|
|user|
|приложение|
|system|
|unknownFutureValue|

### <a name="teamworkapplicationidentitytype-values"></a>значения teamworkApplicationIdentityType 

|Member|
|:---|
|aadApplication|
|бот|
|tenantBot|
|office365Connector|
|исходя изWebhook|
|unknownFutureValue|

### <a name="teamworkconversationidentitytype-values"></a>значения teamworkConversationIdentityType 

|Member|
|:---|
|team|
|канал|
|чат|
|unknownFutureValue|

### <a name="teamworkuseridentitytype-values"></a>значения teamworkUserIdentityType 

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

### <a name="posttype-values"></a>значения postType 

|Member|
|:---|
|регулярные|
|быстрый|
|стратегический|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>значения searchAlterationType

| Member |
|:---------------|
|изменение|
|предложение|

### <a name="servicehealthclassificationtype-values"></a>значения serviceHealthClassificationType 

|Member|
|:---|
|консультативный|
|инцидент|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>значения serviceHealthOrigin 

|Member|
|:---|
|Microsoft|
|thirdParty|
|клиент|
|unknownFutureValue|

### <a name="servicehealthstatus-values"></a>значения serviceHealthStatus 

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
|смягчение|
|resolvedExternal|
|подтверждено|
|сообщается|
|unknownFutureValue|

### <a name="serviceupdatecategory-values"></a>значения serviceUpdateCategory 

|Member|
|:---|
|preventOrFixIssue|
|planForChange|
|stayInformed|
|unknownFutureValue|

### <a name="serviceupdateseverity-values"></a>значения serviceUpdateSeverity 

|Member|
|:---|
|нормальный|
|высокая|
|критически важное значение|
|unknownFutureValue|

### <a name="subjectrightsrequeststage-values"></a>значения subjectRightsRequestStage 

|Member|
|:---|
|contentRetrieval|
|contentReview|
|generateReport|
|contentDeletion|
|caseResolved|
|unknownFutureValue|

### <a name="subjectrightsrequeststagestatus-values"></a>значения subjectRightsRequestStageStatus 

|Member|
|:---|
|notStarted|
|текущий| 
|завершено| 
|не удалось|
|unknownFutureValue|

### <a name="subjectrightsrequeststatus-values"></a>значения subjectRightsRequestStatus 

|Member|
|:---|
|active|
|закрыто|
|unknownFutureValue|

### <a name="subjectrightsrequesttype-values"></a>значения subjectRightsRequestType 

|Member|
|:---|
|экспорт|
|delete|
|доступ|
|tagForAction|
|unknownFutureValue|

### <a name="datasubjecttype-values"></a>значения dataSubjectType 

|Member|
|:---|
|клиент|
|currentEmployee|
|formerEmployee|
|prospectiveEmployee|
|student|
|teacher|
|факультет|
|другие|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>расширенные значенияConfigState 

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="callrecordingstatus-values"></a>значения callRecordingStatus 

|Member|
|:---|
|success|
|сбой|
|начальный|
|chunkFinished|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>значения teamworkCallEventType 

|Member|
|:---|
|call|
|собрание|
|screenShare|
|unknownFutureValue|

### <a name="bookingreminderrecipients-values"></a>значения bookingReminderRecipients 

|Member|
|:---|
|allAttendees|
|персонал|
|клиент|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>значения bookingStaffRole 

|Member|
|:---|
|гость|
|администратор|
|viewer|
|externalGuest|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>answerInputType values 

|Member|
|:---|
|текст|
|radioButton|
|unknownFutureValue|

### <a name="bookingpricetype-values"></a>значения bookingPriceType

|Member|
|:---|
|неопределяемая|
|fixedPrice|
|startingAt|
|почасовая|
|бесплатно|
|priceVaries|
|callUs|
|notSet|
|unknownFutureValue|

### <a name="accessreviewhistorystatus-values"></a>значения accessReviewHistoryStatus

| Member|
|:-----------------|
|done|
|inprogress|
|error|
|запрашивается|
|unknownFutureValue|

### <a name="accessreviewhistorydecisionfilter-values"></a>accessReviewHistoryDecisionFilter values

| Member|
|:-----------------|
|утверждение|
|запретить|
|notReviewed|
|dontKnow|
|notNotified|
|unknownFutureValue|