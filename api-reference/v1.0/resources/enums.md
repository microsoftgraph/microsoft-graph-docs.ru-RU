---
title: Значения Enum
description: Значения переумерия Microsoft Graph.
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: 0ca783518b3244230c776d33609bb6890d8a448c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516117"
---
# <a name="enum-values"></a>Значения Enum

Пространство имен: microsoft.graph

### <a name="activitytype-values"></a>значения activityType

|Элемент|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>значения riskDetectionTimingType

|Элемент|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|автономный режим|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>значения tokenIssuerType

|Элемент|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="attachmenttype-values"></a>Значения attachmentType

| Элемент
|:--------------
| file
| item
| справочник

### <a name="contactrelationship-values"></a>значения contactRelationship

|Элемент|Значение|Описание|
|:---|:---|:---|
|родитель|0|Родитель пользователя.|
|относительный|1 | Родственник пользователя.|
|помощник|2 | Помощник пользователя.|
|врач|3 | Врач пользователя.|
|guardian|4 | Хранитель пользователя.|
|child|5 | Ребенок пользователя.|
|другие|6 | Неустановленное отношение к пользователю.|
|unknownFutureValue|7 | Значение маркера для будущей совместимости.|

### <a name="scheduleentitytheme-values"></a>значения scheduleEntityTheme

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


### <a name="timeoffreasonicontype-values"></a>значения timeOffReasonIconType

|Элемент|
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

### <a name="timezonestandard-values"></a>значения timeZoneStandard

| Элемент
|:-----------------
| Windows
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

| Элемент
|:-------------------------
| Обязательный
| необязательный
| resource


### <a name="externalaudiencescope-values"></a>значения externalAudienceScope

| Элемент
|:-------------------------
| Нет
| contactsOnly
| все


### <a name="automaticrepliesstatus-values"></a>значения automaticRepliesStatus

| Элемент
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

| Элемент
|:-------------------------
| sis
| Вручную
| unknownFutureValue


### <a name="educationgender-values"></a>значения educationGender

| Элемент
|:-------------------------
| женский
| мужской
| другие
| unknownFutureValue


### <a name="eventtype-values"></a>значения eventType

| Элемент
|:-------------------------
| singleInstance
| возникновение
| исключение
| seriesMaster


### <a name="sensitivity-values"></a>значения чувствительности

| Элемент
|:-------------------------
| нормальный
| personal
| частный
| конфиденциальность


### <a name="importance-values"></a>значения важности

| Элемент
|:-------------------------
| низкий
| нормальный
| высокая


### <a name="educationuserrole-values"></a>значения educationUserRole
| Элемент
|:---------------------
| student
| teacher

### <a name="meetingmessagetype-values"></a>значения meetingMessageType

| Элемент
|:-----------------
| Нет
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus values

| Элемент
|:-------------------------
| notFlagged
| complete
| помечено


### <a name="inferenceclassificationtype-values"></a>значения inferenceClassificationType

| Элемент
|:-----------------
| сфокусировано
| другие


### <a name="iosnotificationalerttype-values"></a>значения iosNotificationAlertType

| Элемент
|:-------------------------
| deviceDefault
| баннер
| modal
| Нет

### <a name="deviceenrollmentfailurereason-values"></a>значения deviceEnrollmentFailureReason

| Элемент
|:-------------
| unknown
| проверка подлинности
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
| Элемент
|:---------
| текст
| HTML


### <a name="locationtype-values"></a>Значения locationType

| Элемент
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

| Элемент
|:-------------------------
| unknown
| locationStore
| каталог
| частный
| bing


### <a name="messageactionflag-values"></a>значения messageActionFlag

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
| обзор


### <a name="onenoteuserrole-values"></a>значения onenoteUserRole

| Элемент      | Значение
|:------------|:------------
| Владелец       | 0
| Участник | 1 
| Reader      | 2 
| Нет        | –1


### <a name="operationstatus-values"></a>значения operationStatus

| Элемент
|:-----------------
| NotStarted
| Выполняется
| Completed
| Не выполнено


### <a name="onenotepatchactiontype-values"></a>значения onenotePatchActionType

| Элемент
|:-------------------------
| Заменить
| Приложение
| Удалить
| Вставка
| Prepend

### <a name="onenotepatchinsertposition-values"></a>значения onenotePatchInsertPosition

| Элемент
|:-------------------------
| После
| До


### <a name="phonetype-values"></a>значения phoneType

| Элемент
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

| Элемент
|:-------------------------
| Автоматически
| noPreview
| checklist
| description
| справочник


### <a name="status-values"></a>значения состояния

| Элемент
|:-----------------
| active
| обновлено
| deleted
| пропущено
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex values

| Элемент
|:-------------------------
| во-первых
| во-вторых
| третий
| четвертый
| последний


### <a name="dayofweek-values"></a>значения dayOfWeek

| Элемент
|:-------------------------
| воскресенье
| понедельник
| вторник
| среда
| четверг
| пятница
| суббота

### <a name="recurrencepatterntype-values"></a>значения recurrencePatternType

| Элемент
|:-------------------------
| ежедневно
| еженедельно
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>значения recurrenceRangeType

| Элемент
|:-------------------------
| endDate
| noEnd
| про номера


### <a name="onenotesourceservice-values"></a>значения onenoteSourceService
| Элемент
|:---------------------
| Неизвестно
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>Значения responseType

| Элемент
|:-------------------------
| Нет
| organizer
| предварительноAccepted
| принято
| отклонено
| notResponded


### <a name="activitydomain-values"></a>значения activityDomain

| Элемент
|:-------------------------
| unknown
| work
| personal
| unrestricted


### <a name="websitetype-values"></a>Значения websiteType

| Элемент
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
|truePositive|1 |Оповещение — это верно-положительно.|
|falsePositive|2 | Оповещение является ложным срабатывательным.|
|benignPositive|3 | Оповещение является доброкачественным.|

### <a name="filehashtype-values"></a>значения fileHashType

Enum для типов hash файла.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип.|
|sha1|1 |Тип hash SHA1.|
|sha256|2 | Тип hash SHA256.|
|md5|3 | Тип hash MD5.|
|authenticodeHash256|4 | Тип hash AuthenticodeHash256.|
|lsHash|5 | Тип hash LsHash.|
|ctph|6 | Тип хаши CTPH.|
|peSha1|7 | Тип hash PESHA1.|
|peSha256|8 | Тип hash PESHA256.|

### <a name="connectiondirection-values"></a>значения connectionDirection

Enum для направления сетевого подключения (входящие и исходящие).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное подключение.|
|входящий|1 |Входящий подключение.|
|исходящие|2 | Исходящие подключения.|

### <a name="connectionstatus-values"></a>значения connectionStatus

Enum для состояния подключений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние неизвестного подключения.|
|попытка|1 |Попытка подключения.|
|успешно|2 | Подключение удалось.|
|заблокировано|3 | Подключение заблокировано.|
|не удалось|4 | Сбой подключения.|

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

Enum для ульев реестра, как [определено /windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives).

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный улей.|
|currentConfig|1 |HKEY_CURRENT_CONFIG улей.|
|currentUser|2 | HKEY_CURRENT_USER улей.|
|localMachineSam|3 | HKEY_LOCAL_MACHINE\SAM улей.|
|localMachineSamSoftware|4 | HKEY_LOCAL_MACHINE\Software улей.|
|localMachineSystem|5 | HKEY_LOCAL_MACHINE\System улей.|
|usersDefault|6 | HKEY_USERS \\ . Улей DEFAULT.|

### <a name="registryoperation-values"></a>Значения registryOperation

Операция, изменивла имя и/или значение ключа реестра.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|create|1 |Создание реестра.|
|изменение|2 |Изменение реестра.|
|delete|3 |Удаление реестра.|

### <a name="registryvaluetype-values"></a>значения registryValueType

Enum для типов значений реестра, определяемого [типами /windows/desktop/sysinfo/registry-value-types.](/windows/desktop/sysinfo/registry-value-types)

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный тип значения реестра.|
|двоичный|1 |REG_BINARY типа значения реестра.|
|dword|2 | REG_DWORD типа значения реестра.|
|dwordLittleEndian|3 | REG_DWORD_LITTLE_ENDIAN типа значения реестра.|
|dwordBigEndian|4 | REG_DWORD_BIG_ENDIAN тип значения реестра.|
|expandSz|5 | REG_EXPAND_SZ тип значения реестра.|
|ссылка|6 | REG_LINK тип значения реестра.|
|multiSz|7 | REG_MULTI_SZ тип значения реестра.|
|Нет|8 | REG_NONE тип значения реестра.|
|qword|9 | REG_QWORD тип значения реестра.|
|qwordlittleEndian|10 | REG_QWORD_LITTLE_ENDIAN типа значения реестра.|
|sz|11| REG_SZ тип значения реестра.|

### <a name="alertseverity-values"></a>значения alertSeverity

Enum для серьезности оповещений.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Серьезность неизвестна.|
|информационная|1 |Строгость только для сведений.|
|низкий|2 | Серьезность низкая.|
|medium|3 | Серьезность является средней.|
|высокая|4 | Серьезность высока.|

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
|sender|1 |Отправитель электронной почты.|
|получатель;|2 |Получатель электронной почты.|

### <a name="logontype-values"></a>значения logonType

Возможные значения для метода пользовательского знака.

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|интерактивный|0|Logon является интерактивным.|
|remoteInteractive|1 | Logon — это удаленный интерактивный.|
|сеть|2 | Logon — это сеть.|
|batch|3 | Logon является пакетным.|
|служба|4 | Logon — это служба.|

### <a name="useraccountsecuritytype-values"></a>Значения userAccountSecurityType

Возможные значения для типов учетных записей пользователей (членство в группе) в определении Windows.

|Элемент|Member|Описание|
|:---|:---|:---|
|unknown|–1|Неизвестно.|
|стандартный|0|Член группы стандартных пользователей.|
|power|1 | Член группы Power Users.|
|администратор|2 | Член группы Администраторы.|

### <a name="riskdetail-values"></a>значения riskDetail

| Элемент
|:-------------------------
| adminGeneratedTemporaryPassword
| userPerformedSecuredPasswordChange
| userPerformedSecuredPasswordReset
| adminConfirmedSigninSafe
| aiConfirmedSigninSafe
| userPassedMFADrivenByRiskBasedPolicy
| adminDismissedAllRiskForUser
| AdminConfirmedSigninCompromised
| unknownFutureValue

### <a name="riskeventtypes-values"></a>значения riskEventTypes

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
| общий
| unknownFutureValue

### <a name="riskeventtype-values"></a>значения riskEventType

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
|общий|
|AdminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>значения riskLevel

| Элемент
|:-------------------------
| Нет
| низкий
| medium
| высокая
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>значения riskState

| Элемент
|:-------------------------
| Нет
| confirmedSafe
| исправлено
| отклонено
| atRisk
| confirmedCompromised
| unknownFutureValue

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

|Элемент|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="onlinemeetingprovidertype-values"></a>значения onlineMeetingProviderType

|Элемент|
|:---|
|unknown|
|SkypeForBusiness|
|SkypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>значения delegateMeetingMessageDeliveryOptions

|Элемент|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>значения calendarRoleType

|Элемент|
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
| mail;   | 1      | Угроза почты.            |
| url    | 2      | УГРОЗА URL-адреса.             |
| file   | 3      | Угроза файла вложения. |

### <a name="threatexpectedassessment-values"></a>значения threatExpectedAssessment

| Элемент  | Значение | Описание                       |
|:--------|:------|:----------------------------------|
| block   | 1      | Угроза должна быть заблокирована.     |
| разблокировка | 2      | Угрозу не следует блокировать. |

### <a name="threatcategory-values"></a>значения threatCategory

| Элемент             | Значение | Описание        |
|:-------------------|:------|:-------------------|
| уверенности               | 1      | Угроза нежелательной почты.       |
| степенью           | 2      | Фишинговая угроза.   |
| вредоносные программы            | 3      | Угроза вредоносных программ.    |
| unknownFutureValue | 4      | Член-часовой. |

### <a name="threatassessmentstatus-values"></a>значения threatAssessmentStatus

| Элемент    | Значение | Описание                              |
|:----------|:------|:-----------------------------------------|
| ожидание   | 1      | Оценка угрозы по-прежнему продолжается. |
| завершено | 2      | Оценка угроз завершена.         |

### <a name="threatassessmentrequestsource-values"></a>значения threatAssessmentRequestSource

| Элемент        | Значение | Описание              |
|:--------------|:------|:-------------------------|
| неопределяемая     | 0     | Еще не знаю.            |
| user          | 1      | Отправка пользователя.         |
| администратор | 2      | Отправка администратора клиента. |

### <a name="threatassessmentresulttype-values"></a>значения threatAssessmentResultType

| Элемент             | Значение | Описание                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1      | Результат проверки политики только для `mail` оценки. |
| rescan             | 2      | Результат rescan.                                   |
| unknownFutureValue | 3      | Член-часовой.                                   |

### <a name="maildestinationroutingreason-values"></a>значения mailDestinationRoutingReason

| Элемент                | Значение | Описание                         |
|:----------------------|:------|:------------------------------------|
| Нет                  | 0     | Еще не знаю.                       |
| mailFlowRule          | 1      | Правило транспорта Exchange.            |
| safeSender            | 2      | Безопасный список отправитель.                   |
| blockedSender         | 3      | Заблокированный список отправитель.                |
| advancedSpamFiltering | 4      | Расширенный параметр flitering нежелательной почты.     |
| domainAllowList       | 5      | Список разрешаемой области отправитель.           |
| domainBlockList       | 6      | Список блоков домена отправитель.           |
| notInAddressBook      | 7      | Исключить отправитель не в адресной книге. |
| firstTimeSender       | 8      | Заблокировано из-за первого отправитель времени.   |
| autoPurgeToInbox      | 9      | TimeTravel перемещает сообщение в почтовый ящик.   |
| autoPurgeToJunk       | 10     | TimeTravel перемещает сообщение в нежелательное.    |
| autoPurgeToDeleted    | 11    | TimeTravel перемещает сообщение на удаление. |
| исходящие              | 12     | Исходящие сообщения.                      |
| notJunk               | 13     | Разрешить из-за не нежелательной.              |
| нежелательной                  | 14     | Заблокировано из-за нежелательной почты.                |
| unknownFutureValue    | 15     | Член-часовой.                  |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>значения chatMessagePolicyViolationDlpActionType

| Значение |
|:-----------------|
| Нет |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>значения chatMessagePolicyViolationUserActionType

| Элемент   | Значение Int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 | Значение по умолчанию. Это значение для сообщения, если пользователь не принял действий по сообщению, заблокированного DLP. |
| Override | 1  | Отправитель переопределил вердикт сообщения и отправил сообщение в любом случае.|
| ReportFalsePositive | 2  | Отправитель сообщил об отправке сообщения администраторам как ложный срабатыв.|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>значения chatMessagePolicyViolationVerdictDetailsType

| Элемент   | Значение Int |  Описание |
|:---------------|:--------|:----------|
| Нет | 0 |  Пользователю не разрешается переопределять сообщение. Пользователь не может сообщать о сообщении как о ложном срабатывке, если политикаTip не предоставлена. Во всех остальных сценариях пользователь может сообщить о сообщении как о ложном срабатыве.|
| AllowFalsePositiveOverride | 1  |  Пользователю не разрешается явно переопределять блок, если он не объедин с `AllowOverrideWithoutJustification` `AllowOverrideWithJustification` флагами или флагами. Сообщение о ложном срабатывии нарушения автоматически переопределяет блок и отправляет сообщение. |
| AllowOverrideWithoutJustification | 2  | Пользователю разрешено переопределять блок и отправлять сообщение. Текст обоснования не требуется. Эксклюзив `AllowOverrideWithJustification` для . |
| AllowOverrideWithJustification | 4  |  Пользователю разрешено переопределять блок и отправлять сообщение. Требуется текст обоснования. Эксклюзив `AllowOverrideWithoutJustification` для .|

### <a name="channelmembershiptype-values"></a>Значения channelMembershipType

| Элемент             | Значение |Описание|
| :----------------- | :---- |:-----------|
| стандартный           | 0     |Канал наследует список членов родительской команды.|
| частный            | 1      |Канал может иметь членов, которые являются подмножество всех членов родительской команды.|
| unknownFutureValue | 2      |      |
### <a name="wellknownlistname-values"></a>значения wellknownListName
| Элемент
|:----------------------
| Нет
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>значения taskStatus
| Элемент
|:----------------------
| notStarted
| inProgress
| завершено
| waitingOnOthers
| отложенный

### <a name="permissionclassificationtype-values"></a>значения permissionClassificationType

| Элемент
|:-------
| низкий

### <a name="permissiontype-values"></a>значения permissionType

| Элемент
|:-------------------------
| приложение
| делегирована
| delegatedUserConsentable

### <a name="printcolormode-values"></a>printColorMode values 

|Элемент|
|:---|
|blackAndWhite|
|grayscale|
|color|
|Авто|
|unknownFutureValue|

### <a name="printduplexmode-values"></a>значения printDuplexMode 

|Элемент|
|:---|
|flipOnLongEdge|
|flipOnShortEdge|
|oneSided|
|unknownFutureValue|

### <a name="printerfeedorientation-values"></a>значения printerFeedOrientation 

|Элемент|
|:---|
|longEdgeFirst|
|shortEdgeFirst|
|unknownFutureValue|

### <a name="printfinishing-values"></a>printFinishing values 

|Элемент|
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

|Элемент|
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

|Элемент|
|:---|
|портрет|
|ландшафт|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>значения printQuality 

|Элемент|
|:---|
|низкий|
|medium|
|высокая|
|unknownFutureValue|

### <a name="printscaling-values"></a>значения printScaling 

|Элемент|
|:---|
|Авто|
|shrinkToFit|
|fill|
|fit|
|Нет|
|unknownFutureValue|