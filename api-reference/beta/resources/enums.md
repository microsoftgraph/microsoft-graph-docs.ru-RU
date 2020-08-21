---
title: Значения перечисления
description: Значения перечисления Microsoft Graph
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: 06e117900adca3dd12a31e222a98bda58969621e
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849515"
---
# <a name="enum-values"></a>Значения перечисления

Пространство имен: microsoft.graph

### <a name="allowedaudiences-values"></a>Значения allowedAudiences

|Элемент|
|:---|
|me|
|family|
|contacts|
|groupMembers|
|organization;|
|federatedOrganizations|
|everyone|
|unknownFutureValue|

### <a name="emailtype-values"></a>Значения объекта emailType

|Элемент|
|:---|
|unknown|
|work|
|personal|
|main|
|other|

### <a name="anniversarytype-values"></a>Значения anniversaryType 

|Элемент|
|:---|
|birthday|
|wedding|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>Значения skillProficiencyLevel 

|Элемент|
|:---|
|elementary|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|expert|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>Значения languageProficiencyLevel 

|Элемент|
|:---|
|elementary|
|conversational|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>Значения свойства personRelationship 

|Элемент|
|:---|
|manager|
|коллега|
|directReport|
|dotLineReport|
|assistant|
|dotLineManager|
|alternateContact|
|friend|
|spouse|
|сигнал|
|child|
|родитель|
|sponsor|
|emergencyContact|
|other|
|unknownFutureValue|

### <a name="attachmenttype-values"></a>Значения attachmentType

| Элемент
|:--------------
| file
| item
| ссылка

### <a name="analyticsactivitytype-values"></a>Значения analyticsActivityType

| Элемент
|:--------------
| call
| чат
| рассылка
| фокус
| meeting

### <a name="registrationauthmethod-values"></a>Значения registrationAuthMethod

|Элемент|
|:---|
|рассылка|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>Значения объекта entityTypes

|Элемент|
|:---|
|event|
|message|
|driveItem|
|externalItem|

### <a name="contactrelationship-values"></a>Значения contactRelationship

| Элемент             | Значение | Описание                              |
| :----------------- | :---- | :--------------------------------------- |
| родитель             | 0     | Родительский элемент пользователя.                       |
| relative           | 1     | Относительный адрес пользователя.                     |
| aide               | 2     | Пользователь упрощает.                         |
| doctor             | 3     | Клиент пользователя.                       |
| guardian           | 4      | Охрана пользователя.                     |
| child              | 5      | Дочерний элемент пользователя.                        |
| other              | 6      | Неопределенное отношение с пользователем. |
| unknownFutureValue | 7      | Значение маркера для совместимости с будущими версиями.   |

### <a name="scheduleentitytheme-values"></a>Значения scheduleEntityTheme

| Элемент
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

|Элемент|
|:---|
|Нет|
|car|
|calendar|
|running|
|plane|
|firstAid|
|doctor|
|notWorking|
|часы|
|juryDuty|
|globe|
|cup|
|phone|
|погода|
|umbrella|
|piggyBank|
|dog|
|cake|
|trafficCone|
|pin|
|sunny|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>Значения scheduleChangeState

| Элемент
|:----------------------------
|pending
|approved
|declined
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>Значения scheduleChangeRequestActor

| Элемент
|:----------------------------
|отправитель;
|получатель;
|manager
|system
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>Значения параметра workforceIntegrationEncryptionProtocol

| Элемент
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>Значения объекта workforceIntegrationSupportedEntities

| Элемент
|:----------------------------
|Нет
|shift
|swapRequest
|openShift
|openShiftRequest
|userShiftPreferences

### <a name="timezonestandard-values"></a>Значения timeZoneStandard

| Элемент
|:-----------------
| windows
| iana


### <a name="freebusystatus-values"></a>Значения freeBusyStatus

| Элемент           | Значение |
| :--------------- | :---- |
| free             | 0     |
| tentative        | 1     |
| занят             | 2     |
| oof              | 3     |
| workingElsewhere | 4      |
| unknown          | –1    |


### <a name="physicaladdresstype-values"></a>Значения свойства physicalAddressType

| Элемент
|:-------------------------
| unknown
| home
| business
| other


### <a name="attendeetype-values"></a>Значения attendeeType

| Элемент
|:-------------------------
| Обязательный
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>Значения externalAudienceScope

| Элемент
|:-------------------------
| Нет
| contactsOnly
| все


### <a name="automaticrepliesstatus-values"></a>Значения automaticRepliesStatus

| Элемент
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
| lightYellow | 4      |
| lightTeal   | 5      |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>Значения educationSynchronizationProfileState

| Элемент             | Значение |
| :----------------- | :---- |
| удаление           | 2     |
| deletionFailed     | 3     |
| provisioningFailed (сбой подготовки) | 5      |
| подготовлен        | 6      |
| provisioning       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>Значения educationSynchronizationStatus

| Элемент             | Значение |
| :----------------- | :---- |
| пауза             | 0     |
| inProgress         | 1     |
| success            | 2     |
| error              | 3     |
| validationError    | 4      |
| quarantined        | 5      |
| unknownFutureValue | 6      |

### <a name="educationexternalsource-values"></a>Значения educationExternalSource

| Элемент
|:-------------------------
| sis
| lms
| Вручную
| unknownFutureValue

### <a name="educationgender-values"></a>Значения educationGender

| Элемент
|:-------------------------
| female
| male
| other
| unknownFutureValue


### <a name="eventtype-values"></a>Значения eventType

| Элемент
|:-------------------------
| singleInstance
| occurrence
| exception
| seriesMaster


### <a name="sensitivity-values"></a>Значения конфиденциальности

| Элемент
|:-------------------------
| normal
| personal
| private
| конфиденциальность


### <a name="importance-values"></a>значения важности

| Элемент
|:-------------------------
| low
| normal
| high


### <a name="educationuserrole-values"></a>Значения educationUserRole
| Элемент
|:---------------------
| student
| teacher
| преподавательский


### <a name="meetingmessagetype-values"></a>Значения свойства meetingMessageType

| Элемент
|:-----------------
| Нет
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>Значения followupFlagStatus

| Элемент
|:-------------------------
| notFlagged
| complete
| отмечено


### <a name="inferenceclassificationtype-values"></a>Значения параметра inferenceClassificationType

| Элемент
|:-----------------
| focused
| other


### <a name="iosnotificationalerttype-values"></a>Значения iosNotificationAlertType

| Элемент
|:-------------------------
| deviceDefault
| banner
| modal
| Нет

### <a name="deviceenrollmentfailurereason-values"></a>Значения deviceEnrollmentFailureReason

| Элемент
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


### <a name="bodytype-values"></a>Значения свойства bodyType
| Элемент
|:---------
| текст
| html


### <a name="locationtype-values"></a>Значения LocationType

| Элемент
|:-------------------------
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| hotel
| restaurant
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>Значения locationUniqueIdType

| Элемент
|:-------------------------
| unknown
| locationStore
| directory
| private
| bing


### <a name="messageactionflag-values"></a>Значения messageActionFlag

| Элемент
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
| просмотр


### <a name="onenoteuserrole-values"></a>Значения onenoteUserRole

| Элемент      | Значение |
| :---------- | :---- |
| Владелец       | 0     |
| Участник | 1     |
| Читатель      | 2     |
| Нет        | –1    |


### <a name="operationstatus-values"></a>Значения operationStatus

| Элемент
|:-----------------
| NotStarted
| Работает
| Completed
| Не выполнено


### <a name="onenotepatchactiontype-values"></a>Значения onenotePatchActionType

| Элемент
|:-------------------------
| Заменить
| Добавочное
| Удалить
| Вставка
| Prepend

### <a name="onenotepatchinsertposition-values"></a>Значения onenotePatchInsertPosition

| Элемент
|:-------------------------
| После
| До


### <a name="phonetype-values"></a>Значения phoneType

| Элемент
|:-------------------------
| home
| business
| mobile
| other
| assistant
| homeFax
| businessFax
| otherFax
| pager
| radio


### <a name="plannerpreviewtype-values"></a>Значения plannerPreviewType

| Элемент
|:-------------------------
| Автоматически
| noPreview
| checklist
| description
| ссылка


### <a name="status-values"></a>значения состояния

| Элемент
|:-----------------
| active
| updated
| deleted
| пропущено
| unknownFutureValue


### <a name="weekindex-values"></a>Значения weekIndex

| Элемент
|:-------------------------
| first
| second
| третий
| четвертый
| last


### <a name="dayofweek-values"></a>Значения dayOfWeek

| Элемент
|:-------------------------
| sunday
| monday
| суббота
| wednesday
| thursday
| friday
| saturday

### <a name="recurrencepatterntype-values"></a>Значения recurrencePatternType

| Элемент
|:-------------------------
| ежедневно
| еженедельно
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>Значения recurrenceRangeType

| Элемент
|:-------------------------
| endDate
| noEnd
| нумерованный


### <a name="onenotesourceservice-values"></a>Значения onenoteSourceService
| Элемент
|:---------------------
| Unknown
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>Значения параметра responseType

| Элемент
|:-------------------------
| Нет
| organizer
| tentativelyAccepted
| accepted
| declined
| notResponded


### <a name="activitydomain-values"></a>Значения activityDomain

| Элемент
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>Значения websiteType

| Элемент
|:-------------------------
| other
| home
| work
| Блог
| profile


### <a name="categorycolor-values"></a>Значения категории categoryColor

| Элемент   | Значение |
| :------- | :---- |
| Нет     | –1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 2     |
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
| preset13 | 13    |
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

Возможные значения отзыва в оповещении, предоставленном учетом.

| Элемент         | Значение | Описание               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | Неизвестно.                  |
| truePositive   | 1     | Предупреждение "верно-положительный".   |
| falsePositive  | 2     | Предупреждение является ложным срабатыванием.  |
| benignPositive | 3     | Оповещение является богативным положительным. |

### <a name="filehashtype-values"></a>Значения fileHashType

| Элемент              | Значение | Описание                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | Неизвестный тип.                  |
| sha1                | 1     | Тип хэша SHA1.                |
| sha256              | 2     | Тип хэша SHA256.              |
| md5                 | 3     | Тип хэша MD5.                 |
| authenticodeHash256 | 4      | Тип хэша AuthenticodeHash256. |
| lsHash              | 5      | Тип хэша LsHash.              |
| ctph                | 6      | Тип хэша CTPH.                |
| peSha1              | 7      | Тип хэш-службы PESHA1.              |
| peSha256            | 8      | Тип хэша PESHA256.            |

### <a name="connectiondirection-values"></a>Значения connectionDirection

| Элемент   | Значение | Описание          |
| :------- | :---- | :------------------- |
| unknown  | 0     | Неизвестное подключение.  |
| входящие  | 1     | входящее подключение.  |
| исходящие | 2     | Исходящее подключение. |

### <a name="connectionstatus-values"></a>Значения connectionStatus

| Элемент    | Значение | Описание                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | Состояние неизвестного подключения. |
| attempted | 1     | Попытка подключения.      |
| succeeded | 2     | Подключение успешна.      |
| blocked   | 3     | Подключение заблокировано.        |
| failed    | 4      | Не удалось выполнить подключение.         |

### <a name="processintegritylevel-values"></a>Значения processIntegrityLevel

| Элемент    | Значение | Описание                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | Неизвестно.                      |
| untrusted | 10     | Уровень целостности неявляется надежным. |
| low       | 20    | Низкий уровень целостности.       |
| medium    | 30    | Имеет широкий уровень целостности.    |
| high      | 40    | Высокий уровень целостности.      |
| system    | 50    | Уровень целостности системы.    |

### <a name="registryhive-values"></a>значения реестра

Перечисление кустов реестра, как указано [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives) .

| Элемент                  | Значение | Описание                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | Неизвестный куст.                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG куст.         |
| currentUser             | 2     | HKEY_CURRENT_USER куст.           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM hive.      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE\Куст программного обеспечения. |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE\Куст системы.   |
| usersDefault            | 6      | \\HKEY_USERS. Куст ПО УМОЛЧАНИю.        |

### <a name="registryoperation-values"></a>Значения registryOperation

Операция, изменявшая имя раздела реестра и/или значение.

| Элемент  | Значение | Описание                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | Неизвестный тип значения реестра. |
| create  | 1     | Создайте реестр.             |
| modify  | 2     | Изменение реестра             |
| delete  | 3     | Удалите реестр.             |

### <a name="registryvaluetype-values"></a>Значения registryValueType

Перечисление типов значений реестра в зависимости от [типов значений реестра.](https://docs.microsoft.com/windows/desktop/sysinfo/registry-value-types)

| Элемент            | Значение | Описание                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | Неизвестный тип значения реестра.                 |
| двоичный            | 1     | REG_BINARY типа значения реестра.              |
| dword             | 2     | REG_DWORD значения реестра.               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN типа значения реестра. |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN типа значения реестра.    |
| expandSz          | 5      | REG_EXPAND_SZ типа значения реестра.           |
| ссылка              | 6      | REG_LINK типа значения реестра.                |
| multiSz           | 7      | REG_MULTI_SZ типа значения реестра.            |
| Нет              | 8      | REG_NONE типа значения реестра.                |
| qword             | 9      | REG_QWORD параметра реестра.               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN типа. |
| sz                | 11    | REG_SZ типа значения реестра.                  |

### <a name="alertseverity-values"></a>Значения alertSeverity

Перечисление серьезности оповещений.

| Элемент        | Значение | Описание                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | Степень серьезности неизвестна.              |
| informational | 1     | Серьезность информации доступна только для сведений. |
| low           | 2     | Степень серьезности низка.                  |
| medium        | 3     | Степень серьезности имеет средний уровень.               |
| high          | 4      | Степень серьезности высока.                 |

### <a name="alertstatus-values"></a>Значения alertStatus

Возможные значения состояния жизненного цикла оповещения (этап).

| Элемент     | Значение | Описание           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | Неизвестное состояние.       |
| newAlert   | 10     | Оповещение — это новое.         |
| inProgress | 20    | Оповещение выполняется. |
| разрешено   | 30    | Разрешается оповещение.    |

### <a name="emailrole-values"></a>Значения объекта emailRole

Возможные значения для ролей электронной почты.

| Элемент    | Значение | Описание             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | Неизвестная роль.           |
| отправитель;    | 1     | Отправитель сообщения электронной почты.    |
| получатель; | 2     | Получатель сообщения электронной почты. |

### <a name="logontype-values"></a>Значения logonType

Возможные значения для метода входа пользователя.

| Элемент            | Значение | Описание                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | –1    | Неизвестно.                     |
| interactive       | 0     | Вход в систему интерактивный.        |
| remoteInteractive | 1     | Вход в систему выполняется удаленно. |
| сеть           | 2     | Вход в систему сети.            |
| batch             | 3     | Вход является пакетом.              |
| service           | 4      | Вход в систему — это служба.            |

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группах) и каждого определения Windows.

| Элемент        | Значение | Описание                     |
| :------------ | :---- | :------------------------------ |
| unknown       | –1    | Неизвестно.                        |
| standard      | 0     | Группа обычных пользователей. |
| выключено         | 1     | Участник группы "Питание".    |
| administrator | 2     | Членство в группе "Администраторы". |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>Значения scopeOperatorMultiValuedComparisonType

|Элемент|
|:---|
|все|
|любой|

### <a name="risklevel-values"></a>Значения свойства riskLevel

|Элемент|
|:---|
|low|
|medium|
|high|
|hidden|
|Нет|
|unknownFutureValue|

### <a name="riskstate-values"></a>Значения свойства riskState

|Элемент|
|:---|
|Нет|
|confirmedSafe|
|исправлено|
|Dismissed|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="riskdetail-values"></a>Значения riskDetail

|Элемент|
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

### <a name="referenceattachmentpermission-values"></a>Значения referenceAttachmentPermission

|Элемент|
|:---|
|other|
|view|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>Значения referenceAttachmentProvider

|Элемент|
|:---|
|other|
|oneDriveBusiness|
|oneDriveConsumer|
|dropbox|

### <a name="riskeventtype-values"></a>Значения свойства riskEventType

|Элемент|
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

### <a name="networktype-values"></a>Значения параметра networkType

|Элемент|
|:---|
|intranet|
|extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>Значения параметра exchangeIdFormat

|Элемент|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>Значения атрибута attributeFlowBehavior

|Элемент|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>Значения атрибута attributeFlowType

|Элемент|
|:---|
|always|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>Значения objectFlowTypes

| Элемент | Значение |
| :----- | :---- |
| Нет   | 0     |
| Добавление    | 1     |
| Update | 2     |
| Delete | 4      |

### <a name="chatmessagetype-values"></a>Значения свойства chatMessageType

|Элемент|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>Значения параметра chatMessageImportance

|Элемент|
|:---|
|normal|
|high|
|urgent|

### <a name="channelmembershiptype-values"></a>Значения параметра channelMembershipType

| Элемент             | Значение |
| :----------------- | :---- |
| standard           | 0     |
| private            | 1     |
| unknownFutureValue | 2     |

### <a name="stagedfeaturename-values"></a>Значения stagedFeatureName

| Member                    | Описание                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | Сквозная проверка подлинности    |
| seamlessSso               | Беспрепятственный единый вход       |
| passwordHashSync          | Синхронизация хэша паролей |

### <a name="tokenissuertype-values"></a>Значения tokenIssuerType

|Элемент|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>Значения riskDetectionTimingType

|Элемент|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|offline|
|unknownFutureValue|

### <a name="activitytype-values"></a>Значения свойства activityType

|Элемент|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="entitytype-values"></a>Значения объекта EntityType

| Элемент       |
|:--------------|
|event|
|message|
|driveItem|
|externalFile|
|externalItem|

### <a name="onlinemeetingprovidertype-values"></a>Значения onlineMeetingProviderType

|Элемент|
|:---|
|unknown|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>Значения delegateMeetingMessageDeliveryOptions

|Элемент|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>Значения calendarRoleType

|Элемент|
|:---|
|Нет|
|freeBusyRead|
|limitedRead|
|read|
|write|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|custom|

### <a name="contentformat-values"></a>Значения contentFormat

| Элемент  | Значение | Описание                          |
| :------ | :---- | :----------------------------------- |
| default | 0     | Содержимое это файл или тип сообщений, не относящийся к электронной почте. |
| рассылка   | 1     | Содержимое представляет собой сообщение электронной почты.                 |

### <a name="contentstate-values"></a>Значения contentState

| Элемент | Значение | Описание                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| rest   | 0     | Данные нахожут статистящи Например файл, нагласившего ся в совместной работе.                                 |
| движение | 1     | Данные найдены в движении. Файл, перехватываемый сетевым устройством при передаче.         |
| use    | 2     | Используются данные. Файл открыт в клиентском приложении, например в Microsoft Office. |

### <a name="assignmentmethod-values"></a>Значения метода assignmentMethod

| Элемент     | Значение | Описание                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| standard   | 0     | Метка установлена службой или условием политики.                                                                              |
| privileged | 1     | Метка была явно установлена пользователем.                                                                                          |
| Авто       | 2     | Разрешает переопределение любой существующей метки. Требуется ли обриентировочие на понижении версии. Создается результат `standard` в метаданных. |

### <a name="actionsource-values"></a>Значения actionSource

| Элемент        | Значение | Описание                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| Вручную        | 0     | Пользователь вручную выбрал метку.                          |
| Автоматически     | 1     | Метка была выбрана в результате условий политики.       |
| Рекомендуемый   | 2     | Выбрано применение рекомендованной метки.                    |
| policyDefault | 3     | Пользователь не применяет никаких действий, а также примененную политику. |
| обязательный     | 4      | Пользователь выбрал метку.         |

### <a name="contentalignment-values"></a>Значения contentAlignment

| Элемент | Значение | Описание                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | Выравнивайте маркировку содержимого по левому краю.  |
| Правильно  | 1     | Выравнивайте маркировку содержимого по правому краю. |
| center | 2     | Маркировка содержимого центром.             |

### <a name="watermarklayout-values"></a>Значения watermarkLayout

| Элемент     | Значение | Описание                 |
| :--------- | :---- | :-------------------------- |
| horizontal | 0     | Используйте горизонтальный водяной знак. |
| diagonal   | 1     | Используйте диагональную водяную знак.   |

### <a name="conditionalaccesspolicystate"></a>conditionalAccessPolicyState

|Элемент|
|:---|
|включено|
|отключено|

### <a name="conditionalaccessclientapp"></a>conditionalAccessClientApp

| Элемент       |
|:--------------|
|Обозреватель|
|современная версия|
|easSupported|
|easUnsupported|
|other|

### <a name="conditionalaccessgrantcontrol"></a>conditionalAccessGrantControl

| Элемент       |
|:--------------|
|block|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|

### <a name="cloudappsecuritysessioncontroltype"></a>cloudAppSecuritySessionControlType

| Элемент       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="signinfrequencytype"></a>signinFrequencyType

| Элемент       |
|:--------------|
|days|
|hours|

### <a name="persistentbrowsersessionmode"></a>persistentBrowserSessionMode

| Элемент       |
|:--------------|
|always|
|никогда не|

### <a name="conditionalaccessdeviceplatform"></a>conditionalAccessDevicePlatform

| Элемент       |
|:--------------|
|android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|все|

### <a name="priority-values"></a>Значения приоритета

|Элемент|Значение|
|:---|:---|
|Нет|0|
|High (Высокий)|1|
|Низкая|2|

### <a name="threatassessmentcontenttype-values"></a>Значения объекта threatAssessmentContentType

| Элемент | Значение | Описание             |
|:-------|:------|:------------------------|
| mail   | 1     | Угрозы почты.            |
| url    | 2     | Угроза, защита URL-адреса.             |
| file   | 3     | Угроза, касающуюся файла вложения |

### <a name="threatexpectedassessment-values"></a>Значения threatExpectedAssessment

| Элемент  | Значение | Описание                       |
|:--------|:------|:----------------------------------|
| block   | 1     | Угрозу необходимо заблокировать.     |
| разблокировка | 2     | Угрозу не следует блокировать. |

### <a name="threatcategory-values"></a>Значения объекта threatCategory

| Элемент             | Значение | Описание        |
|:-------------------|:------|:-------------------|
| уверенности               | 1     | Угроза спама.       |
| степенью           | 2     | Угроза фишинга.   |
| вредонос            | 3     | Угроза вредоносного ПО.    |
| unknownFutureValue | 4      | Ослабионный участник. |

### <a name="threatassessmentstatus-values"></a>Значения объекта threatAssessmentStatus

| Элемент    | Значение | Описание                              |
|:----------|:------|:-----------------------------------------|
| pending   | 1     | Оценка угроз по-прежнему продолжаетработаться. |
| completed | 2     | Оценка угроз завершена.         |

### <a name="threatassessmentrequestsource-values"></a>Значения объекта threatAssessmentRequestSource

| Элемент        | Значение | Описание              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | Еще не знакомо.            |
| user          | 1     | Отправка пользователя.         |
| administrator | 2     | Отправка администратором клиента. |

### <a name="threatassessmentresulttype-values"></a>Значения объекта threatAssessmentResultType

| Элемент             | Значение | Описание                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | Результат проверки политики, только для `mail` оценки. |
| rescan             | 2     | Результат повторного сканирования.                                   |
| unknownFutureValue | 3     | Ослабионный участник.                                   |

### <a name="maildestinationroutingreason-values"></a>Значения mailDestinationRoutingReason

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| Нет                  | 0     | Еще не знакомо.                       |
| mailFlowRule          | 1     | Правило транспорта Exchange.            |
| safeSender            | 2     | Список надежных отправителей.                   |
| blockedSender         | 3     | список заблокированных отправителей;                |
| advancedSpamFiltering | 4      | Расширенный тип филянга нежелательной почты.     |
| domainAllowList       | 5      | Список разрешенных доменов отправителя.           |
| domainBlockList       | 6      | Список заблокированных доменов отправителя.           |
| notInAddressBook      | 7      | Исключение отправителя из не адресной книги. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправителя.   |
| autoPurgeToInbox      | 9      | Сообщение с перемещением в папку "Входящие".   |
| autoPurgeToJunk       | 10     | Перемещаемое сообщение в спам в timeTravel.    |
| autoPurgeToDeleted    | 11    | Сообщение о перемещении TimeTravel для удаления. |
| исходящие              | 12     | Исходящая почта.                      |
| notJunk               | 13    | Разрешить по причине не нежелательной почты.              |
| junk                  | 14     | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15     | Ослабионный участник.                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>Значения объекта threatAssessmentRequestPivotProperty

| Элемент                       | Значение | Описание                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | Сводный запрос на оценку угроз, который отнесен. `threatCategory`               |
| mailDestinationRoutingReason | 2     | Сводный запрос на оценку угроз, который отнесен. `mailDestinationRoutingReason` |

### <a name="riskeventtypes-values"></a>Значения свойства riskEventTypes

| Элемент
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

### <a name="openidconnectresponsemode-values"></a>Значения openIdConnectResponseMode
| Элемент                
|:----------------------
| Нет
| form_post
| Запрос 
| unknownFutureValue 

### <a name="openidconnectresponsetypes-values"></a>Значения openIdConnectResponseTypes
| Элемент                
|:----------------------
| Нет
| code
| id_token
| token

### <a name="wellknownlistname-values"></a>Значения wellknownListName
| Элемент
|:----------------------
| Нет
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>Значения taskStatus
| Элемент
|:----------------------
| notStarted
| inProgress
| completed
| waitingOnOthers
| deferred