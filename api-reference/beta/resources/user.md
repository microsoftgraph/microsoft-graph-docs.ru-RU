---
title: Тип ресурса user
description: Представляет учетную запись пользователя Azure AD. Наследуется от directoryObject.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee3f42f36ccee18baf4bcbaaf6790c12a717961e
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658865"
---
# <a name="user-resource-type"></a>Тип ресурса user

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетную запись пользователя Azure AD. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Перечисление пользователей](../api/user-list.md) |Коллекция объектов [user](user.md)| Получение списка, включающего объекты user.|
|[Создание пользователя](../api/user-post-users.md) |[user](user.md)| Создание объекта user.|
|[Получение пользователя](../api/user-get.md) | [user](user.md) |Чтение свойств и связей объекта пользователя.|
|[Обновление пользователя](../api/user-update.md) | [user](user.md) |Обновление объекта пользователя. |
|[Удаление пользователя](../api/user-delete.md) | Нет |Удаление объекта пользователя. |
|[Список сообщений](../api/user-list-messages.md) |Коллекция [message](message.md)| Получение всех сообщений в почтовом ящике вошедшего пользователя.|
|[Создание сообщения](../api/user-post-messages.md) |[message](message.md)| Создание сообщения путем добавления в коллекцию сообщений.|
|[Список объектов mailFolder](../api/user-list-mailfolders.md) |Коллекция [mailFolder](mailfolder.md)| Получение коллекции папок почты в корневой папке вошедшего пользователя. |
|[Создание объекта mailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| Создание объекта mailFolder путем добавления в коллекцию папок почты.|
|[sendMail](../api/user-sendmail.md)|Нет|Отправка сообщения, указанного в теле запроса.|
|[Получение списка событий](../api/user-list-events.md) |Коллекция [event](event.md)| Получение списка объектов event в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user-post-events.md) |[event](event.md)| Создание объекта event путем публикации в коллекции объектов event.|
|[Список календарей](../api/user-list-calendars.md) |Коллекция [Calendar](calendar.md)| Получение коллекции объектов Calendar.|
|[Создание календаря](../api/user-post-calendars.md) |[Calendar](calendar.md)| Создание объекта Calendar путем добавления в коллекцию календарей.|
|[Список объектов calendarGroup](../api/user-list-calendargroups.md) |Коллекция [CalendarGroup](calendargroup.md)| Получение коллекции объектов CalendarGroup.|
|[Создание объекта calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Создание объекта CalendarGroup путем записи в коллекцию групп календарей.|
|[Список calendarView](../api/user-list-calendarview.md) |Коллекция [event](event.md)| Получение коллекции объектов event.|
|[Список контактов](../api/user-list-contacts.md) |Коллекция [contact](contact.md)| Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя.|
|[Создание контакта](../api/user-post-contacts.md) |[contact](contact.md)| Создание контакта путем добавления в коллекцию контактов.|
|[Список объектов contactFolder](../api/user-list-contactfolders.md) |Коллекция [contactFolder](contactfolder.md)| Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.|
|[Создание объекта contactFolder](../api/user-post-contactfolders.md) |[contactFolder](contactfolder.md)| Создание объекта contactFolder путем добавления в коллекцию папок контактов.|
|[Список directReports](../api/user-list-directreports.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и контактов, являющихся подчиненными данного пользователя, из свойства навигации directReports.|
|[Получение руководителя](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Получение пользователя или контакта, являющегося руководителем пользователя, из свойства навигации manager.|
|[Список memberOf](../api/user-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп, ролей каталога и административных единиц, непосредственным участником которых является пользователь, из свойства навигации memberOf.|
|[Перечисление транзитивных свойств memberOf](../api/user-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Перечисление групп, ролей каталога и административных единиц, в которых состоит пользователь. Эта операция является транзитивной и включает группы, в которых пользователь является вложенным элементом. |
|[Перечисление объектов joinedTeams](../api/user-list-joinedteams.md) |Коллекция [team](team.md)| Получение команд Microsoft Teams, непосредственным участником которых является пользователь, из свойства навигации joinedTeams.|
|[Список ownedDevices](../api/user-list-owneddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получение устройств, принадлежащих пользователю, из свойства навигации ownedDevices.|
|[Список ownedObjects](../api/user-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, принадлежащих пользователю, из свойства навигации ownedObjects.|
|[Перечисление plannerTasks](../api/planneruser-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получает объекты plannerTask, назначенные пользователю.|
|[Перечисление registeredDevices](../api/user-list-registereddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получение устройств, зарегистрированных для пользователя, из свойства навигации registeredDevices.|
|[Перечисление участий с ролью в заданной области](../api/user-list-scopedrolememberof.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Получение участий пользователя в административных единицах с ролью в заданной области.|
|[Перечисление createdObjects](../api/user-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, созданных пользователем, из свойства навигации createdObjects.|
|[Перечисление agreementAcceptances](../api/user-list-agreementacceptances.md) | Коллекция [agreementAcceptance](agreementacceptance.md) | Получение списка состояний принятия пользователем условий использования.|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.|
|[reprocessLicense](../api/user-reprocesslicenseassignment.md) |[user](user.md)| Переработка назначенных подписок для пользователя.|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) |Коллекция объектов [licenseDetails](licensedetails.md)| Получение коллекции объектов licenseDetails.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|Коллекция строк|Проверка членства в списке групп. Это транзитивная проверка.|
|[checkMemberObjects](../api/user-checkmemberobjects.md)|Коллекция String|Проверка участия в списке группы, роли каталога или объектах административных единиц. Это транзитивная проверка.|
|[delta](../api/user-delta.md)|Коллекция пользователей| Получение добавочных изменений для пользователей. |
|[findMeetingTimes](../api/user-findmeetingtimes.md)|[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)|Получение времени и местоположения для собрания с учетом доступности участника, а также ограничений по местоположению или времени.|
|[findRoomLists](../api/user-findroomlists.md)|Коллекция [emailaddress.md](emailaddress.md) | Получение списка помещений, определенных в клиенте.|
|[findRooms](../api/user-findrooms.md)|Коллекция [emailaddress.md](emailaddress.md) | Получение всех помещений для собраний в клиенте пользователя или определенном списке помещений. |
|[getMailTips](../api/user-getmailtips.md)|Коллекия [mailTips](mailtips.md)|Возвращение подсказок о доступности одного или нескольких получателей для вошедшего пользователя. |
|[getMemberGroups](../api/user-getmembergroups.md)|Коллекция строк|Возвращает все группы, в которых состоит пользователь. Это транзитивная проверка.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Коллекция строк| Возвращение всех групп, ролей каталога и административных единиц, в которых состоит пользователь. Это транзитивная проверка. |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| Нет |Аннулирует все маркеры обновления и маркеры сеанса пользователя, выпущенные для приложений, сбрасывая значения свойства **refreshTokensValidFromDateTime** и указывая для него текущую дату и время. Это вынуждает пользователей повторно выполнить вход в эти приложения. Этот метод заменяется методом **revokeSignInSessions**.|
|[reminderView](../api/user-reminderview.md)|Коллекция [Reminder](reminder.md)|Возвращает список напоминаний календаря за указанный период времени.|
|[revokeSignInSessions](../api/user-revokesigninsessions.md)| Нет |Отменяет все маркеры обновления и маркеры сеанса пользователя, выпущенные для приложений, сбрасывая значение свойства **signInSessionsValidFromDateTime** и указывая для него текущую дату и время. Это вынуждает пользователей повторно выполнить вход в эти приложения. Этот метод заменяет метод **invalidateAllRefreshTokens**.|
|[translateExchangeIds](../api/user-translateexchangeids.md) |Коллекция [convertIdResult](convertidresult.md)| Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
|aboutMe|String|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Логический| Если учетная запись обеспечена — `true`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.    |
|ageGroup|String|Устанавливает возрастную группу пользователя. Допустимые значения: `null`, `minor`, `notAdult` и `adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions). |
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные пользователю. Значение null не допускается.            |
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Планы, назначенные пользователю. Только для чтения. Значение null не допускается. |
|birthday|DateTimeOffset|День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|businessPhones|Коллекция строк|Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.|
|city|String|Город, в котором находится пользователь. Поддерживает параметр $filter.|
|companyName| String | Название организации, с которой связан пользователь. Это свойство может быть полезно для описания компании внешнего пользователя. |
|consentProvidedForMinor|String|Устанавливает, получено ли согласие для несовершеннолетних. Допустимые значения: `null`, `granted`, `denied` и `notRequired`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions).|
|country|String|Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство". Поддерживает параметр $filter.|
|createdDateTime|DateTimeOffset|Дата и время создания пользователя. Значение не может изменяться и заполняется автоматически при создании сущности. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Свойство допускает значение null. Значение null означает, что для пользователя невозможно точно определить время создания. Только для чтения. Поддерживает параметр $filter.|
|creationType|Строка|Указывает, была ли учетная запись пользователя создана как обычная учебная или рабочая учетная запись (`null`), внешняя учетная запись (`Invitation`), локальная учетная запись для клиента Azure Active Directory B2C (`LocalAccount`) или с помощью самостоятельной регистрации с использованием проверки электронной почты (`EmailVerified`). Только для чтения.|
|deletedDateTime|DateTimeOffset| Дата и время удаления пользователя. |
|department|String|Название отдела, в котором работает пользователь. Поддерживает параметр $filter.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Это значение обычно является сочетанием имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.|
|employeeId|String|Идентификатор сотрудника, назначенный пользователю организацией. Поддерживает параметр $filter.|
|externalUserState|String|Для внешних пользователей, приглашенных в клиент с помощью [API приглашений](../api/invitation-post.md), это свойство представляет состояние приглашения пользователя. Для приглашенных пользователей значением состояния может быть `PendingAcceptance` или `Accepted`, а для всех остальных пользователей — `null`. Поддерживает параметр $filter с поддерживаемыми значениями. Пример: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|String|Показывает метку времени последнего изменения в свойстве externalUserState.|
|faxNumber|String|Номер факса пользователя.|
|givenName|String|Простое имя пользователя. Поддерживает параметр $filter.|
|hireDate|DateTimeOffset|Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String|Уникальный идентификатор пользователя. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|identities|Коллекция [objectIdentity](objectIdentity.md)| Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя. Цифровое удостоверение может предоставляться корпорацией Майкрософт (также известно как локальная учетная запись), организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя. Может содержать несколько элементов с одинаковым значением **signInType**. <br>Поддерживает параметр $filter.|
|interests;|Коллекция строк|Список интересов пользователя.|
|isResourceAccount|Логический| Значение `true`, если пользователь является учетной записью ресурса; в противном случае `false`. Пустое значение должно считаться соответствующим значению `false`.|
|jobTitle;|String|Должность пользователя. Поддерживает параметр $filter.|
|lastPasswordChangeDateTime|DateTimeOffset| Время последнего изменения своего пароля пользователем Azure AD. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|legalAgeGroupClassification|String| Используется корпоративными приложениями для определения юридической возрастной группы пользователя. Это свойство предназначено только для чтения. Вычисляется на основе свойств **ageGroup** и **consentProvidedForMinor**. Допустимые значения: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` и `adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions).|
|licenseAssignmentStates|Коллекция [licenseAssignmentState](licenseassignmentstate.md)|Состояние назначений лицензий для пользователя. Только для чтения.|
|mail|String|SMTP-адрес пользователя, например "gregory@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Параметры основного почтового ящика вошедшего пользователя. Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры языкового стандарта, часового пояса, отправки автоматических ответов на входящие сообщения.|
|mailNickname|String|Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|mySite|String|URL-адрес личного сайта пользователя.|
|officeLocation|String|Расположение офиса на месте работы пользователя.|
|onPremisesDistinguishedName|String| Содержит параметры локальной службы Active Directory `distinguished name` или `DN`. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesDomainName|String| Содержит локальный параметр `domainFQDN`, также называемый dnsDomainName, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Содержит свойства extensionAttribute 1–15 для пользователя. Обратите внимание, что отдельные атрибуты расширения нельзя выбирать и фильтровать. Для пользователей `onPremisesSyncEnabled` этот набор свойств управляется локально и предназначен только для чтения. Для исключительно облачных пользователей (где значением для `onPremisesSyncEnabled` является false) эти свойства можно задать при создании или обновлении. |
|onPremisesImmutableId|String|Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства `userPrincipalName` (имени участника-пользователя) используется федеративный домен. **Важно!** В этом свойстве не допускается использование символов **$** и **\_**. Поддерживает параметр $filter. |
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации объекта с локальным каталогом, например: "2013-02-16T03:04:54Z". Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|onPremisesProvisioningErrors|Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Ошибки при использовании продукта синхронизации Майкрософт во время подготовки. |
|onPremisesSamAccountName|String| Содержит локальный параметр `sAMAccountName`, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) локальной группы, синхронизированной с облаком. Только для чтения.|
|onPremisesSyncEnabled|Логический| Значение `true` указывает, что этот объект синхронизируется из локального каталога. Значение `false` указывает, что этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Значение `null` указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения |
|onPremisesUserPrincipalName|String| Содержит локальный параметр `userPrincipalName`, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|otherMails| Коллекция строк | Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`. Поддерживает параметр $filter.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.|
|pastProjects|Коллекция строк|Список предыдущих проектов пользователя.|
|postalCode|String|Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.|
|preferredDataLocation|String|Предпочитаемое расположение данных для пользователя. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".|
|preferredName|String|Предпочитаемое имя пользователя.|
|provisionedPlans|Коллекция [provisionedPlan](provisionedplan.md)|Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается. |
|proxyAddresses|Коллекция строк|Пример: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. В выражениях фильтра для свойств с несколькими значениями требуется оператор **any**. Только для чтения. Значение null не допускается. Поддерживает параметр $filter.          |
|refreshTokensValidFromDateTime|DateTimeOffset| Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. Только для чтения. Сброс можно выполнить с помощью [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md).|
|responsibilities|Коллекция строк|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|showInAddressList|Логический|Значение `true`, если глобальный список адресов Outlook должен содержать этого пользователя. В противном случае используется значение `false`. Если не задано, будет считаться, что присвоено значение `true`. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение `false`.|
|signInSessionsValidFromDateTime|DateTimeOffset| Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. Только для чтения. Сброс можно выполнить с помощью [revokeSignInSessions](../api/user-revokesigninsessions.md).|
|skills|Коллекция строк|Список навыков пользователя.|
|signInActivity|[signInActivity](signinactivity.md)|Получение последней даты входа в систему и идентификатора запроса на вход для указанного пользователя.<br><br>Поддерживается свойство $filter, но без других фильтруемых свойств. <br>Возвращается только с помощью оператора $select.<br>Только для чтения. |
|state|String|Область, республика, край или округ в адресе пользователя. Поддерживает параметр $filter.|
|streetAddress|String|Почтовый адрес места работы пользователя.|
|surname|String|Фамилия пользователя. Поддерживает параметр $filter.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.  Примеры: "RU", "JP" и "GB". Значение null не допускается. Поддерживает параметр $filter.|
|userPrincipalName|String|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby.
|userType|String|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.          |


### <a name="legal-age-group-property-definitions"></a>Определения свойств юридических возрастных групп

В этом разделе объясняется, как три свойства возрастных групп (`legalAgeGroupClassification`, `ageGroup` и `consentProvidedForMinor`) используются администраторами Azure AD и разработчиками корпоративных приложений для соблюдения нормативных требований, связанных с возрастом.

Пример: Кэмерон — администратор каталога в начальной школе г. Холипорт в Соединенном Королевстве. В начале учебного года он использует документы приемной комиссии, чтобы получить согласие родителей несовершеннолетних учащихся на основе нормативных требований Соединенного Королевства, связанных с возрастом. Согласие, полученное от родителей, позволяет использовать учетные записи несовершеннолетних учащихся в школе г. Холипорт и приложениях Майкрософт. После этого Кэмерон создает все учетные записи и присваивает свойству ageGroup значение minor, а свойству consentProvidedForMinor значение granted. Приложения, используемые учащимися, могут скрывать функции, не подходящие несовершеннолетним.

#### <a name="legal-age-group-classification"></a>Классификация юридических возрастных групп

Это свойство, предназначенное только для чтения, используется разработчиками корпоративных приложений для правильной обработки пользователя с учетом его юридической возрастной группы. Оно вычисляется с учетом свойств пользователя `ageGroup` и `consentProvidedForMinor`.

| Значение   | # |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию. Пользователю не присвоено свойство `ageGroup`.|
|minorWithoutParentalConsent |1|(Зарезервировано для последующего использования)|
|minorWithParentalConsent|2| Пользователь считается несовершеннолетним на основе связанных с возрастом нормативных требований соответствующей страны или региона. Администратор учетной записи получил соответствующее согласие от родителя или опекуна.|
|adult|3|Пользователь считается взрослым на основе связанных с возрастом нормативных требований соответствующей страны или региона.|
|notAdult|4|Пользователь находится в стране или регионе, использующем дополнительные нормативные требования в отношении возраста (например, США, Соединенное Королевство, Европейский союз или Южная Корея), и возраст пользователя находится между категорией несовершеннолетия и взрослой категорией (устанавливается в зависимости от страны или региона). Обычно это означает, что в странах с регулированием подростки относятся к категории `notAdult`.|
|minorNoParentalConsentRequired|5|Пользователь является несовершеннолетним, но находится в стране без нормативных требований, связанных с возрастом.|

#### <a name="age-group-and-minor-consent"></a>Возрастная группа и согласие для несовершеннолетних

Возрастная группа и согласие для несовершеннолетних — это необязательные свойства, используемые администраторами Azure AD для обеспечения правильной обработки используемой учетной записи на основе связанных с возрастом нормативных требований, действующих в стране или регионе пользователя.

#### <a name="agegroup-property"></a>Свойство ageGroup

| Значение    | # |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию. Пользователю не присвоено свойство `ageGroup`.|
|minor|1|Пользователь считается несовершеннолетним.|
|notAdult|2|Пользователь находится в стране с нормативными положениями (США, Соединенное Королевство, Европейский союз и Южная Корея) и возраст пользователя превышает верхнюю границу детского возраста (зависит от страны), но меньше нижней границы взрослого возраста (устанавливается в зависимости от страны или региона). По существу, в странах с регулированием подростки относятся к категории `notAdult`.|
|adult|3|Пользователь должен считаться взрослым.|

#### <a name="consentprovidedforminor-property"></a>Свойство consentProvidedForMinor

| Значение    | # |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию. Пользователю не присвоено свойство `consentProvidedForMinor`.|
|granted|1|Для пользователя получено согласие на наличие учетной записи.|
|denied|2|Для пользователя не получено согласие на наличие учетной записи.|
|notRequired|3|Пользователь находится в расположении, не требующем согласия.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|agreementAcceptances|Коллекция [agreementAcceptance](agreementacceptance.md)| Состояния принятия пользователем условий использования. Только для чтения. Допускается значение null.|
|calendar|[calendar](calendar.md)|Основной календарь пользователя. Только для чтения.|
|calendarGroups|Коллекция [calendarGroup](calendargroup.md)|Группы календарей пользователя. Только для чтения. Допускается значение null.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения. Допускается значение null.|
|calendars|Коллекция [calendar](calendar.md)|Календари пользователя. Только для чтения. Допускается значение null.|
|contactFolders|Коллекция [contactFolder](contactfolder.md)|Папки контактов пользователя. Только для чтения. Допускается значение null.|
|contacts|Коллекция [contact](contact.md)|Контакты пользователя. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные пользователем. Только для чтения. Допускается значение null.|
|directReports|Коллекция [directoryObject](directoryobject.md)|Пользователи и контакты, являющиеся подчиненными пользователя (пользователи и контакты, у которых в свойстве manager указан этот пользователь). Только для чтения. Допускается значение null. |
|drive|[drive](drive.md)|Хранилище OneDrive пользователя. Только для чтения.|
|drives|Коллекция [drive](drive.md)| Коллекция дисков, доступных для этого пользователя. Только для чтения. |
|Мероприятия|Коллекция [event](event.md)|События пользователя. По умолчанию отображаются события в стандартном календаре. Только для чтения. Допускается значение null.|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для пользователя. Допускается значение null.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Классификация релевантности для сообщений пользователя, основанная на явных обозначениях, переопределяющих заданные релевантность или важность. |
|insights|[officeGraphInsights](officegraphinsights.md) | Только для чтения. Допускается значение null.|
|joinedGroups|Коллекция [group](group.md)| Только для чтения. Допускается значение null.|
|mailFolders|Коллекция [mailFolder](mailfolder.md)| Почтовые папки пользователя. Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)|Пользователь или контакт, являющийся руководителем пользователя. Только для чтения. (Методы HTTP: GET, PUT, DELETE.)|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, роли каталога и административные единицы, в которых состоит пользователь. Только для чтения. Допускается значение null.|
|joinedTeams|Коллекция [team](team.md)|Команды Microsoft Teams, участником которых является пользователь. Только для чтения. Допускается значение null.|
|teamwork|[userTeamwork](userteamwork.md)| Контейнер для функций Microsoft Teams, доступных пользователю. Только для чтения. Допускается значение null.|
|messages|Коллекция [message](message.md)|Сообщения в почтовом ящике или папке. Только для чтения. Допускается значение null.|
|onenote|[onenote](onenote.md)| Только для чтения.|
|outlook|[outlookUser](outlookuser.md)| Выборочные службы Outlook, доступные пользователю. Только для чтения. Допускается значение null.|
|ownedDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|people|Коллекция [person](person.md)| Только для чтения. Наиболее релевантные люди для пользователя. Коллекция упорядочена по их релевантности для пользователя, которая определяется его общением, совместной работой и бизнес-связями. Человек представляется в виде агрегированных сведений из почты, контактов и социальных сетей.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля пользователя. Только для чтения.|
|photos|Коллекция [photo](photo.md)| Только для чтения. Допускается значение null.|
|planner|[plannerUser](planneruser.md)| Выборочные службы Планировщика, доступные пользователю. Только для чтения. Допускается значение null. |
|scopedRoleMemberOf|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Участие пользователя в административных единицах с ролью в заданной области. Только для чтения. Допускается значение null.|
|параметры|[userSettings](user-settings.md) | Только для чтения. Допускается значение null.|
|registeredDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, зарегистрированные для пользователя. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "drives",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "teamwork",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "createdDateTime": "2019-02-07T21:53:13.067Z",
  "creationType": "string",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "employeeId": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "faxNumber": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDistinguishedName": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "otherMails": ["string"],
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "refreshTokensValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "responsibilities": ["string"],
  "schools": ["string"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",
  "calendar": {"@odata.type": "microsoft.graph.calendar"},
  "calendarGroups": [{"@odata.type": "microsoft.graph.calendarGroup"}],
  "calendarView": [{"@odata.type": "microsoft.graph.event"}],
  "calendars": [{"@odata.type": "microsoft.graph.calendar"}],
  "contacts": [{"@odata.type": "microsoft.graph.contact"}],
  "contactFolders": [{"@odata.type": "microsoft.graph.contactFolder"}],
  "createdObjects": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directReports": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "drive": {"@odata.type": "microsoft.graph.drive"},
  "drives": [{"@odata.type": "microsoft.graph.drive"}],
  "insights": {"@odata.type": "microsoft.graph.officeGraphInsights"},
  "settings": {"@odata.type": "microsoft.graph.userSettings"},
  "events": [{"@odata.type": "microsoft.graph.event"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "inferenceClassification": {"@odata.type": "microsoft.graph.inferenceClassification"},
  "mailFolders": [{"@odata.type": "microsoft.graph.mailFolder"}],
  "manager": {"@odata.type": "microsoft.graph.directoryObject"},
  "memberOf": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "joinedTeams": [{"@odata.type": "microsoft.graph.group"}],
  "teamwork": {"@odata.type": "microsoft.graph.teamwork"},
  "messages": [{ "@odata.type": "microsoft.graph.message"}],
  "outlook": {"@odata.type": "microsoft.graph.outlookUser"},
  "ownedDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "photo": {"@odata.type": "microsoft.graph.profilePhoto"},
  "registeredDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "signInActivity": {"@odata.type": "microsoft.graph.signInActivity"}
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
