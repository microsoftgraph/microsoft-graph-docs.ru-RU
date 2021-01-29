---
title: Значения enum
description: Значения для индексирования Microsoft Graph
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: b3b6cb7bbc2abacc02939ad374808f4e1ddbed85
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052540"
---
# <a name="enum-values"></a>Значения enum

Пространство имен: microsoft.graph

### <a name="appliedconditionalaccesspolicyresult-values"></a>значения appliedConditionalAccessPolicyResult 



|Member|
|:---|
|success|
|failure|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|
|reportOnlySuccess|
|reportOnlyFailure|
|reportOnlyNotApplied|
|reportOnlyInterrupted|

### <a name="authenticationmethodfeature-values"></a>Значения authenticationMethodFeature 



|Member|
|:---|
|ssprRegistered|
|ssprEnabled|
|ssprCapable|
|passwordlessCapable|
|mfaCapable|

### <a name="authmethodstype-values"></a>значения authMethodsType 



|Member|
|:---|
|email|
|mobileSMS|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appNotificationCode|
|appNotificationAndCode|
|appPassword|
|fido|
|alternateMobilePhone|
|mobilePhoneAndSMS|
|unknownFutureValue|

### <a name="azureadlicensetype-values"></a>значения azureADLicenseType 



|Member|
|:---|
|Нет|
|free|
|basic|
|premiumP1|
|premiumP2|
|unknownFutureValue|

### <a name="conditionalaccessconditions-values"></a>значения conditionalAccessConditions 



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
|client|

### <a name="conditionalaccessstatus-values"></a>значения conditionalAccessStatus 



|Member|
|:---|
|success|
|failure|
|notApplied|
|unknownFutureValue|

### <a name="featuretype-values"></a>Значения featureType 



|Member|
|:---|
|registration|
|сброс|
|unknownFutureValue|

### <a name="grouptype-values"></a>значения groupType 



|Member|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="includeduserroles-values"></a>значения includedUserRoles 



|Member|
|:---|
|all|
|privilegedAdmin|
|admin|
|user|
|unknownFutureValue|

### <a name="includedusertypes-values"></a>значения includedUserTypes 



|Member|
|:---|
|all|
|участники|
|guest|
|unknownFutureValue|

### <a name="initiatortype-values"></a>Значения initiatorType 



|Member|
|:---|
|user|
|приложение|
|system|
|unknownFutureValue|

### <a name="migrationstatus-values"></a>Значения migrationStatus 



|Member|
|:---|
|ready|
|needsReview|
|additionalStepsRequired|
|unknownFutureValue|

### <a name="networktype-values"></a>значения networkType 



|Member|
|:---|
|интрасеть|
|extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

### <a name="operationresult-values"></a>Значения operationResult 



|Member|
|:---|
|success|
|failure|
|timeout|
|unknownFutureValue|

### <a name="provisioningresult-values"></a>значения provisioningResult 



|Member|
|:---|
|success|
|failure|
|пропущено|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>значения provisioningStepType 



|Member|
|:---|
|import|
|scoping|
|matching|
|обработка|
|referenceResolution|
|export|
|unknownFutureValue|

### <a name="registrationauthmethod-values"></a>значения registrationAuthMethod 



|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|
|fido|
|appPassword|
|unknownFutureValue|

### <a name="registrationstatustype-values"></a>значения registrationStatusType 



|Member|
|:---|
|registered|
|включено|
|capable|
|mfaRegistered|
|unknownFutureValue|

### <a name="requirementprovider-values"></a>значения requirementProvider 



|Member|
|:---|
|Многофакторная проверка подлинности|
|ЦС|
|unknownFutureValue|

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
|adminConfirmedSigninCompromised|
|hidden|
|adminConfirmedUserCompromised|
|unknownFutureValue|

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
|generic|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>Значения riskLevel 



|Member|
|:---|
|low|
|medium|
|high|
|hidden|
|Нет|
|unknownFutureValue|

### <a name="riskstate-values"></a>значения riskState 



|Member|
|:---|
|Нет|
|confirmedSafe|
|исправлено|
|dismissed|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>Значения tokenIssuerType 



|Member|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="usageauthmethod-values"></a>значения usageAuthMethod 



|Member|
|:---|
|email|
|mobileSMS|
|mobileCall|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobileCall|
|fido|
|appPassword|
|unknownFutureValue|

### <a name="authenticationmethodkeystrength-values"></a>Значения authenticationMethodKeyStrength

|Member|
|:---|
|normal|
|weak|
|unknown|

### <a name="educationaddedstudentaction-values"></a>значения educationAddedStudentAction

|Member|
|:---|
|Нет|
|assignIfOpen|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>значения externalEmailOtpState

|Member|
|:---|
|default|
|включено|
|отключено|
|unknownFutureValue|

### <a name="replyrestriction-values"></a>значения replyRestriction

| Member
|:--------------
| все
| authorAndModerators
| unknownFutureValue

### <a name="usernewmessagerestriction-values"></a>Значения userNewMessageRestriction

| Member
|:--------------
|все
|everyoneExceptGuests
|модераторы
|unknownFutureValue

### <a name="volumetype-values"></a>значения volumeType

| Member
|:--------------
| operatingSystemVolume
| fixedDataVolume
| removableDataVolume
| unknownFutureValue

### <a name="allowedaudiences-values"></a>значения allowedAudiences

|Member|
|:---|
|me|
|family|
|contacts|
|groupMembers|
|organization;|
|federatedOrganizations|
|все|
|unknownFutureValue|

### <a name="attestationlevel-values"></a>значения attestationLevel

|Member|
|:---|
|attested|
|notAttested|

### <a name="emailtype-values"></a>Значения emailType

|Member|
|:---|
|unknown|
|work|
|personal|
|main|
|other|

### <a name="authenticationmethodtargettype-values"></a>Значения authenticationMethodTargetType

|Member|
|:---|
|user|
|group|

### <a name="authenticationmethodstate-values"></a>Значения authenticationMethodState

|Member|
|:---|
|включено|
|отключено|

### <a name="fido2restrictionenforcementtype-values"></a>Значения fido2RestrictionEnforcementType

|Member|
|:---|
|allow|
|block|

### <a name="authenticatorappcontexttype-values"></a>Значения authenticatorAppContextType

|Member|
|:---|
|расположение;|
|приложение|

### <a name="anniversarytype-values"></a>Значения anniversaryType

|Member|
|:---|
|birthday|
|1|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>Значения skillProficiencyLevel

|Member|
|:---|
|y|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|expert|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>Значения languageProficiencyLevel

|Member|
|:---|
|y|
|conversational|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>значения personRelationship

|Member|
|:---|
|manager|
|colleague|
|directReport|
|dotLineReport|
|assistant|
|dotLineManager|
|alternateContact|
|friend|
|spouse|
|sibling|
|child|
|родитель|
|sponsor|
|emergencyContact|
|other|
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
| meeting

### <a name="registrationauthmethod-values"></a>значения registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>Значения entityTypes

|Member|
|:---|
|event|
|message|
|driveItem|
|externalItem|
|site|
|список|
|listItem|
|drive|

### <a name="bucketaggregationsortproperty-values"></a>Значения bucketAggregationSortProperty

|Member|
|:---|
|count|
|keyAsString|
|keyAsNumber|

### <a name="contactrelationship-values"></a>значения contactRelationship

| Элемент             | Значение | Описание                              |
| :----------------- | :---- | :--------------------------------------- |
| родитель             | 0     | Родительский пользователь.                       |
| relative           | 1      | Относительный пользователь.                     |
| aide               | 2      | Помощник пользователя.                         |
| 1             | 3     | Пользователь должен быть в сети.                       |
| guardian           | 4      | Защитник пользователя.                     |
| child              | 5      | Дитя пользователя.                        |
| other              | 6      | Неопределенные отношения с пользователем. |
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
| серый
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
|car|
|calendar|
|running|
|plane|
|firstAid|
|1|
|notWorking|
|clock|
|время в окнах|
|globe|
|cup|
|phone|
|погода|
|umbrella|
|gyBank|
|dog|
|1|
|trafficCone|
|pin|
|10|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>Значения scheduleChangeState

| Member
|:----------------------------
|pending
|утверждено
|отклонено
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

| Member
|:----------------------------
|Нет
|shift
|swapRequest
|openShift
|openShiftRequest
|userShiftPreferences

### <a name="timezonestandard-values"></a>Значения timeZoneStandard

| Member
|:-----------------
| windows
| iana


### <a name="freebusystatus-values"></a>Значения freeBusyStatus

| Элемент           | Значение |
| :--------------- | :---- |
| free             | 0     |
| tentative        | 1      |
| busy             | 2      |
| oof              | 3     |
| workingElsewhere | 4      |
| unknown          | –1    |


### <a name="physicaladdresstype-values"></a>Значения physicalAddressType

| Member
|:-------------------------
| unknown
| home
| бизнес
| other


### <a name="attendeetype-values"></a>значения attendeeType

| Member
|:-------------------------
| Обязательный
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>значения externalAudienceScope

| Member
|:-------------------------
| Нет
| contactsOnly
| all


### <a name="automaticrepliesstatus-values"></a>Значения automaticRepliesStatus

| Member
|:-------------------------
| отключено
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>значения calendarColor

| Элемент      | Значение |
| :---------- | :---- |
| Авто        | –1    |
| lightBlue   | 0     |
| lightGreen  | 1      |
| lightOrange | 2      |
| lightGray   | 3     |
| lightYellow | 4      |
| lightTeal   | 5      |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>значения educationSynchronizationProfileState

| Элемент             | Значение |
| :----------------- | :---- |
| удаление           | 2      |
| deletionFailed     | 3     |
| provisioningFailed | 5      |
| provisioned        | 6      |
| подготовка       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>значения educationSynchronizationStatus

| Элемент             | Значение |
| :----------------- | :---- |
| paused             | 0     |
| inProgress         | 1      |
| success            | 2      |
| error              | 3     |
| validationError    | 4      |
| карантин        | 5      |
| unknownFutureValue | 6      |

### <a name="educationexternalsource-values"></a>значения educationExternalSource

| Member
|:-------------------------
| sis
| lms
| Вручную
| unknownFutureValue

### <a name="educationgender-values"></a>значения educationGender

| Member
|:-------------------------
| female
| male
| other
| unknownFutureValue


### <a name="eventtype-values"></a>значения eventType

| Member
|:-------------------------
| singleInstance
| occurrence
| exception
| seriesMaster


### <a name="sensitivity-values"></a>значения конфиденциальности

| Member
|:-------------------------
| normal
| personal
| private
| confidential


### <a name="importance-values"></a>значения важности

| Member
|:-------------------------
| low
| normal
| high


### <a name="educationuserrole-values"></a>значения educationUserRole
| Member
|:---------------------
| student
| teacher
| faculty


### <a name="meetingmessagetype-values"></a>значения meetingMessageType

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
| flagged


### <a name="inferenceclassificationtype-values"></a>значения inferenceClassificationType

| Member
|:-----------------
| focused
| other


### <a name="iosnotificationalerttype-values"></a>Значения iosNotificationAlertType

| Member
|:-------------------------
| deviceDefault
| banner
| modal
| Нет

### <a name="deviceenrollmentfailurereason-values"></a>Значения deviceEnrollmentFailureReason

| Member
|:-------------
| unknown
| проверка подлинности
| authorization
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
| html


### <a name="locationtype-values"></a>Значения locationType

| Member
|:-------------------------
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| hotel
| ресторан
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>Значения locationUniqueIdType

| Member
|:-------------------------
| unknown
| locationStore
| каталог
| private
| bing


### <a name="messageactionflag-values"></a>Значения messageActionFlag

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
| review


### <a name="onenoteuserrole-values"></a>Значения onenoteUserRole

| Элемент      | Значение |
| :---------- | :---- |
| Владелец       | 0     |
| Участник | 1      |
| Читатель      | 2      |
| Нет        | –1    |


### <a name="operationstatus-values"></a>значения operationStatus

| Member
|:-----------------
| NotStarted
| Выполняется
| Completed
| Не выполнено


### <a name="onenotepatchactiontype-values"></a>Значения onenotePatchActionType

| Member
|:-------------------------
| Заменить
| Append
| Удалить
| Вставка
| Prepend

### <a name="onenotepatchinsertposition-values"></a>Значения onenotePatchInsertPosition

| Member
|:-------------------------
| После
| До


### <a name="phonetype-values"></a>Значения phoneType

| Member
|:-------------------------
| home
| бизнес
| мобильный
| other
| assistant
| homeFax
| businessFax
| otherFax
| pager
| radio


### <a name="plannerpreviewtype-values"></a>Значения plannerPreviewType

| Member
|:-------------------------
| Автоматически
| noPreview
| checklist
| (описание)
| справочник


### <a name="status-values"></a>значения состояния

| Member
|:-----------------
| active
| updated
| deleted
| пропущено
| unknownFutureValue


### <a name="weekindex-values"></a>Значения weekIndex

| Member
|:-------------------------
| first
| second
| third
| fourth
| last


### <a name="dayofweek-values"></a>значения dayOfWeek

| Member
|:-------------------------
| sunday
| monday
| tuesday
| wednesday
| thursday
| friday
| saturday

### <a name="recurrencepatterntype-values"></a>значения recurrencePatternType

| Member
|:-------------------------
| daily
| еженедельно
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>Значения recurrenceRangeType

| Member
|:-------------------------
| endDate
| noEnd
| numbered


### <a name="onenotesourceservice-values"></a>Значения onenoteSourceService
| Member
|:---------------------
| Неизвестно
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>значения responseType

| Member
|:-------------------------
| Нет
| organizer
| tentativelyAccepted
| accepted
| отклонено
| notResponded


### <a name="activitydomain-values"></a>значения activityDomain

| Member
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>значения websiteType

| Member
|:-------------------------
| other
| home
| work
| Блог
| profile


### <a name="categorycolor-values"></a>значения categoryColor

| Элемент   | Значение |
| :------- | :---- |
| Нет     | –1    |
| preset0  | 0     |
| preset1  | 1      |
| preset2  | 2      |
| preset3  | 3     |
| preset4  | 4      |
| preset5  | 5      |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10     |
| preset11 | 11    |
| preset12 | 12     |
| preset13 | 13     |
| preset14 | 14     |
| preset15 | 15     |
| preset16 | 16     |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 20    |
| preset21 | 21    |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>Значения alertFeedback

Возможные значения отзывов в оповещении, предоставленного аналитиком.

| Элемент         | Значение | Описание               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | Неизвестно.                  |
| truePositive   | 1      | Оповещение имеет положительный результат.   |
| falsePositive  | 2      | Оповещение имеет ложное срабатыващение.  |
| benignPositive | 3     | Оповещение положительное. |

### <a name="filehashtype-values"></a>Значения fileHashType

| Элемент              | Значение | Описание                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | Неизвестный тип.                  |
| sha1                | 1      | Тип hash SHA1.                |
| sha256              | 2      | Тип hash SHA256.              |
| md5                 | 3     | Тип hash MD5.                 |
| authenticodeHash256 | 4      | Тип hash AuthenticodeHash256. |
| lsHash              | 5      | Тип hash LsHash.              |
| CTPH                | 6      | Тип hash CTPH.                |
| peSha1              | 7      | Тип hash PESHA1.              |
| peSha256            | 8      | Тип hash PESHA256.            |

### <a name="connectiondirection-values"></a>значения connectionDirection

| Элемент   | Значение | Описание          |
| :------- | :---- | :------------------- |
| unknown  | 0     | Неизвестное подключение.  |
| входящий  | 1      | Входящий подключение.  |
| исходящие | 2      | Исходящие подключения. |

### <a name="connectionstatus-values"></a>значения connectionStatus

| Элемент    | Значение | Описание                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | Неизвестное состояние подключения. |
| attempted | 1      | Попытка подключения.      |
| succeeded | 2      | Подключение успешно.      |
| blocked   | 3     | Подключение заблокировано.        |
| failed    | 4      | Сбой подключения.         |

### <a name="processintegritylevel-values"></a>значения processIntegrityLevel

| Элемент    | Значение | Описание                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | Неизвестно.                      |
| untrusted | 10     | Уровень целостности не является недоверным. |
| low       | 20    | Уровень целостности низкий.       |
| medium    | 30    | Уровень целостности средний.    |
| high      | 40    | Уровень целостности высокий.      |
| system    | 50    | Уровень целостности — "Система".    |

### <a name="registryhive-values"></a>значения registryHive

Enum for registry hives as defined by [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives) .

| Элемент                  | Значение | Описание                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | Неизвестный улей.                     |
| currentConfig           | 1      | HKEY_CURRENT_CONFIG.         |
| currentUser             | 2      | HKEY_CURRENT_USER.           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM.      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE\Software. |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE\System.   |
| usersDefault            | 6      | HKEY_USERS \\ . Hive по умолчанию.        |

### <a name="registryoperation-values"></a>значения registryOperation

Операция, которая изменила имя и/или значение ключа реестра.

| Элемент  | Значение | Описание                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | Неизвестный тип значения реестра. |
| create  | 1      | Создайте реестр.             |
| modify  | 2      | Изменение реестра.             |
| delete  | 3     | Удаление реестра.             |

### <a name="registryvaluetype-values"></a>значения registryValueType

Enum for registry value types as defined by [Registry value types](/windows/desktop/sysinfo/registry-value-types).

| Элемент            | Значение | Описание                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | Неизвестный тип значения реестра.                 |
| двоичный            | 1      | REG_BINARY реестра.              |
| dword             | 2      | REG_DWORD реестра.               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN реестра. |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN реестра.    |
| expandSz          | 5      | REG_EXPAND_SZ реестра.           |
| ссылка              | 6      | REG_LINK реестра.                |
| multiSz           | 7      | REG_MULTI_SZ реестра.            |
| Нет              | 8      | REG_NONE реестра.                |
| qword             | 9      | REG_QWORD реестра.               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN реестра. |
| sz                | 11    | REG_SZ реестра.                  |

### <a name="alertseverity-values"></a>Значения alertSeverity

Enum for severity of alerts.

| Элемент        | Значение | Описание                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | Серьезность неизвестна.              |
| информационный | 1      | Серьезность только для сведений. |
| low           | 2      | Степень серьезности низка.                  |
| medium        | 3     | Степень серьезности средняя.               |
| high          | 4      | Степень серьезности высока.                 |

### <a name="alertstatus-values"></a>Значения alertStatus

Возможные значения состояния жизненного цикла оповещений (стадии).

| Элемент     | Значение | Описание           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | Неизвестное состояние.       |
| newAlert   | 10     | Оповещение является новым.         |
| inProgress | 20    | Оповещение находится в процессе выполнения. |
| resolved   | 30    | Оповещение устранено.    |

### <a name="emailrole-values"></a>Значения emailRole

Возможные значения для ролей электронной почты.

| Элемент    | Значение | Описание             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | Неизвестная роль.           |
| sender    | 1      | Отправитель сообщения электронной почты.    |
| получатель; | 2      | Получатель сообщения электронной почты. |

### <a name="logontype-values"></a>Значения logonType

Возможные значения для метода входе пользователя.

| Элемент            | Значение | Описание                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | –1    | Неизвестно.                     |
| interactive       | 0     | В этом режиме можно в интерактивном режиме.        |
| remoteInteractive | 1      | В этом режиме можно использовать удаленный интерактивный режим. |
| сеть           | 2      | Во время logon это сеть.            |
| batch             | 3     | В этом пакетном пакете.              |
| служба           | 4      | Logon is service.            |

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группах) в определении Windows.

| Элемент        | Значение | Описание                     |
| :------------ | :---- | :------------------------------ |
| unknown       | –1    | Неизвестно.                        |
| standard      | 0     | Участник группы "Стандартные пользователи". |
| power         | 1      | Участник группы "Power Users".    |
| administrator | 2      | Участник группы администраторов. |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>Значения chatMessagePolicyViolationDlpActionType

| Значение |
|:-----------------|
| Нет |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>значения scopeOperatorMultiValuedComparisonType

|Member|
|:---|
|all|
|любой|

### <a name="risklevel-values"></a>Значения riskLevel

|Member|
|:---|
|low|
|medium|
|high|
|hidden|
|Нет|
|unknownFutureValue|

### <a name="riskstate-values"></a>значения riskState

|Member|
|:---|
|Нет|
|confirmedSafe|
|исправлено|
|dismissed|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

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
|adminConfirmedSigninCompromised|
|adminConfirmedUserCompromised|
|hidden|
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>значения referenceAttachmentPermission

|Member|
|:---|
|other|
|представление|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>Значения referenceAttachmentProvider

|Member|
|:---|
|other|
|oneDriveBusiness|
|oneDriveConsumer|
|dropbox|

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
|generic|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="networktype-values"></a>значения networkType

|Member|
|:---|
|интрасеть|
|extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>значения attributeFlowBehavior

|Member|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>Значения attributeFlowType

|Member|
|:---|
|always|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>значения objectFlowTypes

| Элемент | Значение |
| :----- | :---- |
| Нет   | 0     |
| Добавление    | 1      |
| Update | 2      |
| Delete | 4      |

### <a name="chatmessagetype-values"></a>Значения chatMessageType

|Member|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>значения chatMessageImportance

|Member|
|:---|
|normal|
|high|
|urgent|

### <a name="channelmembershiptype-values"></a>Значения channelMembershipType

| Элемент             | Значение |
| :----------------- | :---- |
| standard           | 0     |
| private            | 1      |
| unknownFutureValue | 2      |

### <a name="stagedfeaturename-values"></a>значения stagedFeatureName

| Member                    | Описание                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | Passthrough Authentication    |
| seamlessSso               | Бесперебойный единый вход       |
| passwordHashSync          | Синхронизация hash паролей |

### <a name="tokenissuertype-values"></a>Значения tokenIssuerType

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>значения riskDetectionTimingType

|Member|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|автономный режим|
|unknownFutureValue|

### <a name="activitytype-values"></a>значения activityType

|Member|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>Значения chatMessagePolicyViolationUserActionType

| Member   | Значение int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 | Значение по умолчанию. Это значение в сообщении, если пользователь не принял действие с сообщением, заблокированным DLP. |
| Override | 1  | Отправитель переопределил решение и отправил сообщение.|
| ReportFalsePositive | 2  | Отправитель сообщил администраторам о ложном срабатывии.|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>Значения chatMessagePolicyViolationVerdictDetailsType

| Member   | Значение int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 |  Пользователю запрещено переопределять сообщение. Пользователь не может сообщить о ложном срабатывии, если не предоставлена политика. Во всех остальных сценариях пользователь может сообщить о ложном срабатывии сообщения.|
| AllowFalsePositiveOverride | 1  |  Пользователю не разрешено явно переопределять блок, если он не объединен с ним или `AllowOverrideWithoutJustification` не `AllowOverrideWithJustification` имеет флагов. Сообщение о ложном срабатывии при нарушении автоматически переопределяет блокировку и отправляет сообщение. |
| AllowOverrideWithoutJustification | 2  | Пользователю разрешено переопределять блокировку и отправлять сообщение. Текст обоснования не требуется. Монопольно `AllowOverrideWithJustification` для . |
| AllowOverrideWithJustification | 4  |  Пользователю разрешено переопределять блокировку и отправлять сообщение. Требуется текст обоснования. Монопольно `AllowOverrideWithoutJustification` для .|

### <a name="entitytype-values"></a>Значения entityType

| Member       |
|:--------------|
|event|
|message|
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
|custom|

### <a name="contentformat-values"></a>значения contentFormat

| Элемент  | Значение | Описание                          |
| :------ | :---- | :----------------------------------- |
| default | 0     | Содержимое является файлом или типом, не относянымся к электронной почте. |
| email   | 1      | Содержимое — это сообщение электронной почты.                 |

### <a name="contentstate-values"></a>значения contentState

| Элемент | Значение | Описание                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| rest   | 0     | Неавтные данные; Например, файл в папке.                                 |
| движение | 1      | Данные в движении. Файл, перехваченный сетевым устройством в пути.         |
| use    | 2      | Данные используются. Файл открыт в клиентских приложениях, таких как Microsoft Office. |

### <a name="assignmentmethod-values"></a>Значения assignmentMethod

| Элемент     | Значение | Описание                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| standard   | 0     | Метка была установлена с помощью условия службы или политики.                                                                              |
| privileged | 1      | Метка была явно установлена пользователем.                                                                                          |
| Авто       | 2      | Разрешает переопределять любую существующую метку. Обоснование, необходимое для понижения. Приводит к `standard` методу назначения в метаданных. |

### <a name="actionsource-values"></a>значения actionSource

| Элемент        | Значение | Описание                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| Вручную        | 0     | Пользователь вручную выбрал метку.                          |
| Автоматически     | 1      | Метка была выбрана в результате условий политики.       |
| Рекомендуемый   | 2      | Выбрано применение рекомендуемой метки.                    |
| policyDefault | 3     | Пользователь не применял действие и метку по умолчанию политики. |
| mandatory     | 4      | Пользователь выбрал метку после принудительных выборов.         |

### <a name="contentalignment-values"></a>значения contentAlignment

| Элемент | Значение | Описание                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | Выравнивание пометки содержимого слева.  |
| Правильно  | 1      | Выравнивание пометки содержимого справа. |
| center | 2      | Маркировка содержимого по центру.             |

### <a name="watermarklayout-values"></a>значения watermarkLayout

| Элемент     | Значение | Описание                 |
| :--------- | :---- | :-------------------------- |
| horizontal | 0     | Используйте горизонтальный водяной знак. |
| diagonal   | 1      | Используйте диагональный водяной знак.   |

### <a name="conditionalaccesspolicystate"></a>conditionalAccessPolicyState

|Member|
|:---|
|включено|
|отключено|

### <a name="conditionalaccessclientapp"></a>conditionalAccessClientApp

| Member       |
|:--------------|
|Обозреватель|
|современная версия|
|easSupported|
|easUnsupported|
|other|

### <a name="conditionalaccessgrantcontrol"></a>conditionalAccessGrantControl

| Member       |
|:--------------|
|block|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|

### <a name="cloudappsecuritysessioncontroltype"></a>cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="signinfrequencytype"></a>signinFrequencyType

| Member       |
|:--------------|
|days|
|часы|

### <a name="persistentbrowsersessionmode"></a>persistentBrowserSessionMode

| Member       |
|:--------------|
|always|
|never|

### <a name="conditionalaccessdeviceplatform"></a>conditionalAccessDevicePlatform

| Member       |
|:--------------|
|android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|all|

### <a name="priority-values"></a>значения приоритета

|Элемент|Значение|
|:---|:---|
|Нет|0|
|High (Высокий)|1 |
|Низкие|2 |

### <a name="threatassessmentcontenttype-values"></a>Значения threatAssessmentContentType

| Элемент | Значение | Описание             |
|:-------|:------|:------------------------|
| mail   | 1      | Угроза почты.            |
| url    | 2      | Угроза URL-адреса.             |
| file   | 3     | Угроза файла вложения. |

### <a name="threatexpectedassessment-values"></a>значения threatExpectedAssessment

| Элемент  | Значение | Описание                       |
|:--------|:------|:----------------------------------|
| block   | 1      | Угрозу следует заблокировать.     |
| unblock | 2      | Угрозу не следует блокировать. |

### <a name="threatcategory-values"></a>значения threatCategory

| Элемент             | Значение | Описание        |
|:-------------------|:------|:-------------------|
| уверенности               | 1      | Угроза нежелательной почты.       |
| степенью           | 2      | Фишинговая угроза.   |
| malware            | 3     | Угроза вредоносного ПО.    |
| unknownFutureValue | 4      | Член sentinel. |

### <a name="threatassessmentstatus-values"></a>Значения threatAssessmentStatus

| Элемент    | Значение | Описание                              |
|:----------|:------|:-----------------------------------------|
| pending   | 1      | Оценка угроз все еще продолжается. |
| completed | 2      | Оценка угроз завершена.         |

### <a name="threatassessmentrequestsource-values"></a>Значения threatAssessmentRequestSource

| Элемент        | Значение | Описание              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | Пока не известно.            |
| user          | 1      | Отправка пользователя.         |
| administrator | 2      | Отправка администратора клиента. |

### <a name="threatassessmentresulttype-values"></a>Значения threatAssessmentResultType

| Элемент             | Значение | Описание                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1      | Результат проверки политики только для `mail` оценки. |
| rescan             | 2      | Результат повторного скана.                                   |
| unknownFutureValue | 3     | Член sentinel.                                   |

### <a name="maildestinationroutingreason-values"></a>Значения mailDestinationRoutingReason

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| Нет                  | 0     | Пока не известно.                       |
| mailFlowRule          | 1      | Правило транспорта Exchange.            |
| safeSender            | 2      | Список надежных отправитель.                   |
| blockedSender         | 3     | Список заблокированных отправитель.                |
| advancedSpamFiltering | 4      | Расширенный параметр размещания нежелательной почты.     |
| domainAllowList       | 5      | Список разрешает домен отправитель.           |
| domainBlockList       | 6      | Список заблокированных доменов отправитель.           |
| notInAddressBook      | 7      | Исключить отправитель не в адресной книге. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправитель.   |
| autoPurgeToInbox      | 9      | TimeTravel перемещает сообщение в "Входящие".   |
| autoPurgeToJunk       | 10     | TimeTravel перемещает сообщение в нежелательное.    |
| autoPurgeToDeleted    | 11    | Сообщение с перемещением TimeTravel в удаленное. |
| исходящие              | 12     | Исходящие сообщения.                      |
| notJunk               | 13     | Разрешить из-за того, что не является нежелательным.              |
| junk                  | 14     | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15     | Член sentinel.                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>Значения threatAssessmentRequestPivotProperty

| Элемент                       | Значение | Описание                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1      | Агрегатный запрос на оценку угроз по `threatCategory` .               |
| mailDestinationRoutingReason | 2      | Агрегатный запрос на оценку угроз по `mailDestinationRoutingReason` . |

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
| generic
| unknownFutureValue

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

### <a name="openidconnectresponsemode-values"></a>Значения openIdConnectResponseMode

| Member
|:----------------------
| Нет
| form_post
| Запрос
| unknownFutureValue

### <a name="openidconnectresponsetypes-values"></a>Значения openIdConnectResponseTypes

| Member
|:----------------------
| Нет
| code
| id_token
| token

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
| completed
| waitingOnOthers
| deferred

### <a name="connectedorganizationstate-values"></a>значения connectedOrganizationState

| Элемент                | Значение | Описание                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| configured            | 0     | Подключенные организации с этим значением состояния включаются в политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запросителя.                                                          |
| proposed              | 1      | Подключенные организации, автоматически созданные системой, имеют это значение состояния. Они не включаются в политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запросителя.   |
| unknownFutureValue    | 2      | Член sentinel.                                                                                                                                                                                                 |

### <a name="identitysourcetype-values"></a>Значения identitySourceType

|Member|
|:---|
|azureActiveDirectory|
|external|

### <a name="externalgroupmembertype-values"></a>значения externalGroupMemberType

|Member|
|:---|
|user|
|group|

### <a name="identityuserflowattributedatatype-values"></a>Значения identityUserFlowAttributeDataType

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| string                | 1      | строковый тип данных                    |
| boolean               | 2      | тип данных Boolean                   |
| int64                 | 3     | Тип данных Int                       |
| stringCollection      | 4      | Тип данных коллекции строк         |
| unknownFutureValue    | 5      | Член sentinel.                  |

### <a name="identityuserflowattributetype-values"></a>Значения identityUserFlowAttributeType

| Элемент                | Значение | Описание                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| builtIn               | 1      | Этот тип атрибута пользовательского потока означает, что он был создан системой |
| custom                | 2      | Этот тип атрибута потока пользователя обозначает, что он был создан пользователем   |
| unknownFutureValue    | 3     | Член sentinel.                                                 |

### <a name="connectionstate-values"></a>значения connectionState

|Member|
|:---|
|draft|
|ready|
|устаревшее|
|limitExceeded|

### <a name="permissionclassificationtype-values"></a>Значения permissionClassificationType

| Member
|:-------
| low

### <a name="permissiontype-values"></a>Значения permissionType

| Member
|:-------------------------
| приложение
| delegated
| delegatedUserConsentable

### <a name="identityuserflowattributeinputtype-values"></a>Значения identityUserFlowAttributeInputType

| Member                |
|:----------------------|
| textBox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>значения teamworkActivityTopicSource

| Member
|:---
| entityUrl
| текст

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>Значения cloudPcProvisioningPolicyImageType

|Member|
|:---|
|custom|
|gallery|

### <a name="chattype-values"></a>значения chatType 

| Элемент             | Значение | Описание               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Указывает, что чат является чатом 1:1. Для этого типа чата зафиксирован размер группы, член не может быть удален или добавлен.                  |
|group               | 1      | Указывает, что чат является групповым чатом. Для этого типа чата можно обновить размер группы (не менее 2 человек). Члены можно удалить или добавить позже.   |
|meeting             | 2      | Указывает, что чат является чатом собрания, который создается как побочный эффект создания OnlineMeeting.  |
|unknownFutureValue  | 3     | Значение Sentinel, чтобы указать будущие значения. |

### <a name="plannercontainertype-values"></a>значения plannerContainerType 

|Member|
|:---|
|group|
|unknownFutureValue|