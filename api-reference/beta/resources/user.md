---
title: Тип ресурса user
description: Представляет учетную запись пользователя Azure AD. Наследуется от directoryObject.
ms.openlocfilehash: 496e349162ddffe918c2d293cc9032cff6fd14c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081730"
---
# <a name="user-resource-type"></a>Тип ресурса user

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет учетную запись пользователя Azure AD. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- Добавление настраиваемых свойств данные как [расширения](/graph/extensibility-overview).
- Подписка на [уведомления об изменении](/graph/webhooks).
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Перечисление пользователей](../api/user-list.md) |Коллекция объектов [user](user.md)| Получение списка, включающего объекты user.|
|[Создание пользователя](../api/user-post-users.md) |[user](user.md)| Создание объекта user.|
|[Получение пользователя](../api/user-get.md) | [user](user.md) |Чтение свойств и связей объекта пользователя.|
|[Обновление пользователя](../api/user-update.md) | [user](user.md) |Обновление объекта пользователя. |
|[Удаление пользователя](../api/user-delete.md) | Нет |Удаление объекта пользователя. |
|[Список сообщений](../api/user-list-messages.md) |Коллекция [Message](message.md)| Получение всех сообщений в почтовом ящике вошедшего пользователя.|
|[Создание объекта Message](../api/user-post-messages.md) |[Message](message.md)| Создание сообщения с учета в коллекцию сообщения.|
|[Список объектов mailFolder](../api/user-list-mailfolders.md) |Коллекция [MailFolder](mailfolder.md)| Получение коллекции папок почты в корневой папке вошедшего пользователя. |
|[Создание объекта MailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| Создание объекта MailFolder путем добавления в коллекцию папок почты.|
|[sendMail](../api/user-sendmail.md)|Нет|Отправка сообщения, указанного в теле запроса.|
|[Получение списка событий](../api/user-list-events.md) |Коллекция [Event](event.md)| Получение списка объектов event в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user-post-events.md) |[Event](event.md)| Создание объекта Event путем добавления в коллекцию событий.|
|[Список календарей](../api/user-list-calendars.md) |Коллекция [Calendar](calendar.md)| Получение коллекции объектов Calendar.|
|[Создание календаря](../api/user-post-calendars.md) |[Calendar](calendar.md)| Создание объекта Calendar путем добавления в коллекцию календарей.|
|[Список объектов calendarGroup](../api/user-list-calendargroups.md) |Коллекция [CalendarGroup](calendargroup.md)| Получение коллекции объектов CalendarGroup.|
|[Создание объекта calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Создание объекта CalendarGroup путем записи в коллекцию групп календарей.|
|[Список calendarView](../api/user-list-calendarview.md) |Коллекция [Event](event.md)| Получение коллекции объектов событий.|
|[Список контактов](../api/user-list-contacts.md) |Коллекция [Contact](contact.md)| Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя.|
|[Создание контакта](../api/user-post-contacts.md) |[Contact](contact.md)| Создание объекта Contact путем добавления в коллекцию контактов.|
|[Список объектов contactFolder](../api/user-list-contactfolders.md) |Коллекция [ContactFolder](contactfolder.md)| Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.|
|[Создание объекта ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| Создание объекта ContactFolder путем добавления в коллекцию папок контактов.|
|[Список directReports](../api/user-list-directreports.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и контактов, являющихся подчиненными данного пользователя, из свойства навигации directReports.|
|[Получение руководителя](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Получение пользователя или контакта, являющегося руководителем пользователя, из свойства навигации manager.|
|[Список memberOf](../api/user-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получите групп, каталог ролей и административных единиц измерения, которые пользователь принадлежит к прямой из свойства навигации член групп.|
|[Доверия транзитивных член списка](../api/user-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, каталог ролей и административных единиц измерения, которыми пользователь. Эта операция доверия транзитивных и включает в себя группы, которые пользователь является участником вложенными. |
|[Список joinedTeams](../api/user-list-joinedteams.md) |семейства сайтов [групп](group.md)| Получите группами Майкрософт, что пользователь является прямое членом из свойства joinedTeams навигации.|
|[Список ownedDevices](../api/user-list-owneddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получение устройств, принадлежащих пользователю, из свойства навигации ownedDevices.|
|[Список ownedObjects](../api/user-list-ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, принадлежащих пользователю, из свойства навигации ownedObjects.|
|[Перечисление объектов plannerTasks](../api/planneruser-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получите plannerTasks, назначенные пользователю.|
|[Список registeredDevices](../api/user-list-registereddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получите устройств, зарегистрированных для пользователя из свойства registeredDevices навигации.|
|[Членство в пределах ролях списка](../api/user-list-scopedrolememberof.md) |[scopedRoleMembership](scopedrolemembership.md) коллекции| Участие в группах административные единицы Get областью действия роли для этого пользователя.|
|[Список createdObjects](../api/user-list-createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, созданных пользователем, из свойства навигации createdObjects.|
|[Список agreementAcceptances](../api/user-list-agreementacceptances.md) | [agreementAcceptance](agreementacceptance.md) коллекции | Ознакомьтесь со списком условия использования приемки состояния пользователя.|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) |Коллекция объектов [licenseDetails](licensedetails.md)| Получение коллекции объектов licenseDetails.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|Коллекция строк|Проверка членства в списке групп. Это транзитивная проверка.|
|[findmeetingtimes](../api/user-findmeetingtimes.md)|[meetingTimeCandidate](meetingtimecandidate.md)|Время поиска и расположений в соответствии с на основании сведений о доступности участника, расположение или ограничений по времени.|
|[findRoomLists](../api/user-findroomlists.md)|[EmailAddress.md](emailaddress.md) коллекции | Получение списков комнат, определенных в клиент.|
|[findRooms](../api/user-findrooms.md)|[EmailAddress.md](emailaddress.md) коллекции | Получение всех комнатах для собраний в клиент пользователя или в списке конкретных комнаты. |
|[getMailTips](../api/user-getmailtips.md)|[почтовые подсказки](mailtips.md) семейства сайтов|Снова подсказок одного или нескольких получателей как доступные пользователь выполнил вход. |
|[getMemberGroups](../api/user-getmembergroups.md)|Коллекция строк|Возвращает все группы, в которых состоит пользователь. Это транзитивная проверка.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Коллекция String| Возврат групп, каталог ролей и административных единиц измерения, которыми пользователь. Проверка доверия транзитивных. |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| Нет |Признает недействительным пользователя обновления и сеанса маркеры, выданные к приложениям, путем присвоения свойству пользователя **refreshTokensValidFromDateTime** текущая дата и время. Это заставляет пользователя выполнить повторный вход для этих приложений.|
|[reminderView](../api/user-reminderview.md)|Коллекция [Reminder](reminder.md)|Возвращает список напоминаний календаря за указанный период времени.|
|[delta](../api/user-delta.md)|Коллекция пользователей| Получение добавочных изменений для пользователей. |
|[Переводить идентификаторы Outlook](../api/user-translateexchangeids.md) |Коллекция [типов ресурсов convertIdResult](convertidresult.md)| Переведите идентификаторы, связанные с Outlook ресурсов форматов.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
|aboutMe|String|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Логический| Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.    |
|ageGroup|String|Задает срок хранения в группу пользователя. Допускаются значения: `null`, `minor`, `notAdult` и `adult`. Обратитесь к [определения свойств группы юридическом срок хранения](#legal-age-group-property-definitions) для получения дополнительных сведений. |
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные пользователю. Значение null не допускается.            |
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Планы, назначенные пользователю. Только для чтения. Значение null не допускается. |
|birthday|DateTimeOffset|День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|city|String|Город, в котором находится пользователь. Поддерживает параметр $filter.|
|companyName| String | Название организации, с которой связан пользователь. Только для чтения.
|consentProvidedForMinor|String|Задает для минорам после получения подтверждения. Допускаются значения: `null`, `granted`, `denied` и `notRequired`. Обратитесь к [определения свойств группы юридическом срок хранения](#legal-age-group-property-definitions) для получения дополнительных сведений.|
|country|String|Страна или регион, в котором расположен пользователь; Например, «US» или «(Великобритания)». Поддерживает параметр $filter.|
|deletedDateTime|DateTimeOffset| Дата и время, которое пользователь был удален. |
|department|String|Название отдела, в котором работает пользователь. Поддерживает параметр $filter.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Это значение обычно представляет собой комбинацию имя пользователя, средней имя и Фамилия. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.|
|employeeId|String|Идентификатор сотрудника, назначенных пользователю организацией. Поддерживает параметр $filter.|
|externalUserState|String|Для внешних пользователей к клиенту с помощью [API приглашение](../api/invitation-post.md)на участие это свойство представляет состояние приглашения приглашенные пользователи. Приглашенные пользователи состояние могут быть «PendingAcceptance» или «Принято», или `null` для всех других пользователей. Поддерживает $filter на поддерживаемые значения. Пример: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|String|Показана метка времени последнего изменения к свойству externalUserState.|
|Номер факса|String|Номер факса пользователя.|
|givenName|String|Простое имя пользователя. Поддерживает параметр $filter.|
|hireDate|DateTimeOffset|Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String|Уникальный идентификатор пользователя. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение NULL не допускается. Только для чтения.|
|interests|Коллекция строк|Список интересов пользователя.|
|jobTitle|String|Должность пользователя. Поддерживает параметр $filter.|
|legalAgeGroupClassification|String| Используется для определения срока хранения юридическом группы пользователя корпоративных приложений. Это свойство только для чтения и вычисляемых на основе `ageGroup` и `consentProvidedForMinor` свойства. Допускаются значения: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` и `adult`. Обратитесь к [определения свойств группы юридическом срок хранения](#legal-age-group-property-definitions) для получения дополнительных сведений.)|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md) коллекции|Состояние лицензии назначения для этого пользователя. Только для чтения.|
|mail|String|SMTP-адрес пользователя, например "gregory@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Параметры основного параметра вошедшего пользователя. Можно [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры для отправки автоматические ответы, которые входящих сообщений, языковой стандарт и часового пояса.|
|mailNickname|String|Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|mySite|String|URL-адрес личного сайта пользователя.|
|officeLocation|String|Расположение офиса на месте работы пользователя.|
|onPremisesDistinguishedName|String| Содержит Active Directory локальной `distinguished name` или `DN`. Свойство заполняется только для клиентов, которым выполняется синхронизация их локального каталога для Azure Active Directory с помощью Azure AD подключение. Только для чтения. |
|onPremisesDomainName|String| Содержит локальной `domainFQDN`, также называемый dnsDomainName синхронизируются из локального каталога. Свойство заполняется только для клиентов, которым выполняется синхронизация их локального каталога для Azure Active Directory с помощью Azure AD подключение. Только для чтения. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|Содержит extensionAttributes 1 – 15 для пользователя. Обратите внимание, что атрибуты отдельных расширения фильтруемые ни доступно для выбора. Для `onPremisesSyncEnabled` пользователя, этот набор свойств, создаются в локальной и доступен только для чтения. Для пользователей только в облаке (где `onPremisesSyncEnabled` присвоено значение false), эти свойства могут быть установлены во время создания или обновления. |
|onPremisesImmutableId|String|Это свойство используется для сопоставления учетной записи пользователя в локальной Active Directory для объекта пользователя их Azure AD. Это свойство должен быть указан при создании учетной записи пользователя на графике, при использовании федеративного домена для пользователя `userPrincipalName` свойство (UPN). **Важные:** **$** И **_** знаки нельзя использовать при указании этого свойства. Поддерживает параметр $filter. |
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации объекта с локальным каталогом, например: "2013-02-16T03:04:54Z". Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) коллекции| Ошибки при использовании продуктов Майкрософт синхронизации во время подготовки. |
|onPremisesSamAccountName|String| Содержит локальной `sAMAccountName` синхронизируются из локального каталога. Свойство заполняется только для клиентов, которым выполняется синхронизация их локального каталога для Azure Active Directory с помощью Azure AD подключение. Только для чтения. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) локальной группы, синхронизированной с облаком. Только для чтения.|
|onPremisesSyncEnabled|Логическое| Значение **true** указывает, что этот объект синхронизируется из локального каталога. Значение **false** указывает, что этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Значение **null** указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения |
|onPremisesUserPrincipalName|String| Содержит локальной `userPrincipalName` синхронизируются из локального каталога. Свойство заполняется только для клиентов, которым выполняется синхронизация их локального каталога для Azure Active Directory с помощью Azure AD подключение. Только для чтения. |
|otherMails|String| Список дополнительные адреса электронной почты пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`. Поддерживает параметр $filter.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.|
|pastProjects|Коллекция строк|Список предыдущих проектов пользователя.|
|postalCode|String|Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.|
|preferredDataLocation|String|Расположение предпочитаемый данных для пользователя. Для получения дополнительных сведений см [OneDrive Online Multi-географически](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".|
|preferredName|String|Предпочитаемое имя пользователя.|
|provisionedPlans|Коллекция [ProvisionedPlan](provisionedplan.md)|Планы, подготовленные для пользователя. Только для чтения. Значение null не допускается. |
|proxyAddresses|Коллекция строк|Пример: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. В выражениях фильтра для свойств с несколькими значениями требуется оператор **any**. Только для чтения. Значение null не допускается. Поддерживает параметр $filter.          |
|refreshTokensValidFromDateTime|DateTimeOffset| Любые обновления маркеры или на основе маркеров сеансов (cookie сеанса) выдается до этого времени недопустимы и приложения появится сообщение об ошибке при использовании недопустимых обновления или сеансах маркера для получения делегированный доступ маркеров (получить доступ к API-интерфейсы, такие как Microsoft Graph).  В этом случае приложения необходимо получить новый маркер обновления при выполнении запроса к конечной точке авторизовать. Только для чтения. Используйте [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) , чтобы сбросить.|
|responsibilities|Коллекция строк|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|showInAddressList|Логический|**значение true,** Если Outlook глобального списка адресов должны содержать этот пользователь, в противном случае — **false**. Если не установлен, это будет рассматриваться как **значение true**. Для пользователей, диспетчер приглашение на участие это свойство будет иметь значение **false**.|
|skills|Коллекция строк|Список навыков пользователя.|
|state|String|Область, республика, край или округ в адресе пользователя. Поддерживает параметр $filter.|
|streetAddress|String|Почтовый адрес места работы пользователя.|
|surname|String|Фамилия пользователя. Поддерживает параметр $filter.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.  Примеры: "RU", "JP" и "GB". Значение null не допускается. Поддерживает параметр $filter.|
|userPrincipalName|String|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby.
|userType|String|Строковое значение, которое можно использовать для классификации типов пользователей в каталоге, например «Элемент» и «Гость». Поддерживает параметр $filter.          |

### <a name="legal-age-group-property-definitions"></a>Срок хранения в юридическом определения свойств группы

В этом разделе объясняется, как до трех лет свойств группы (`legalAgeGroupClassification`, `ageGroup` и `consentProvidedForMinor`) используются для обеспечить соответствие правовым нормам, связанные с срок хранения с Azure AD администраторам и разработчикам приложений предприятия.

Например: Кэмерон является администратором каталога для школа в Holyport в Великобритании. В начало года школа он использует приемной комиссии документацию для получения разрешения от родительского вспомогательных на основании правилам связанные с срока хранения в Соединенное Королевство. Подтверждения, полученный от родительского сайта позволяет вспомогательных учетной записи для использования с Holyport school и приложений Microsoft. Затем Кэмерон создает все учетные записи и задает ageGroup для «незначительная» и consentProvidedForMinor для «узел». Затем приложений, используемых свой студентов могут отключить функции, которые не подходят для минорам.

#### <a name="legal-age-group-classification"></a>Срок хранения в юридическом группы классификации

Это свойство только для чтения используется разработчиками приложения enterprise, чтобы обеспечить правильную обработку пользователя, основываясь на группе срок хранения в юридическом. Рассчитывается на его основе `ageGroup` и `consentProvidedForMinor` свойства.

| Значение   | # |Description|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию не `ageGroup` имеет значение для пользователя.|
|minorWithoutParentalConsent |1|(Зарезервировано для будущего использования)|
|minorWithParentalConsent|2| Пользователь считается вспомогательных, на основании правилам связанные с срока хранения в своей страны или региона и администратора учетной записи получил соответствующие разрешения от родительского или опекуном.|
|для взрослых|3|На основании правилам связанные с срока хранения из своей страны или региона взрослых считается, что пользователь.|
|notAdult|4|Пользователь является из страны или региона, где используется дополнительные правилам в связанных с срок хранения (например, США, Великобритания, Европейский союз или Южная Корея) и возраста пользователя находится в пределах вспомогательные и взрослых срок хранения (как настоящим на основе страны или региона). Как правило, это означает, что подростков считаются `notAdult` в регулируемого странах.|
|minorNoParentalConsentRequired|5|Пользователь является дополнительную, но не из страны или региона, где используется не связанные с срок хранения нормам в области коммуникаций.|

#### <a name="age-group-and-minor-consent"></a>Срок хранения в группу и вспомогательные согласия

Срок хранения в группу и вспомогательные согласия свойств, дополнительные свойства используется администраторами Azure AD, чтобы гарантировать, что использование учетной записи обрабатывается правильно на основании связанных с срок хранения нормативные правила, управляющие страны или региона пользователя.

#### <a name="agegroup-property"></a>Свойство ageGroup

| Значение    | # |Description|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию не `ageGroup` имеет значение для пользователя.|
|дополнительный номер|1|Пользователь является рассмотрите возможность вспомогательных.|
|notAdult|2|Пользователь является из страны с обязательной законодательства США, Великобритания, Европейский союз или Южная Корея) и возраста пользователя — это больше, чем максимальный срок хранения kid (согласно страны) и меньше, чем нижний предел возраста для взрослых (как настоящим на основе страну или регион) . По сути, считаются подростков `notAdult` в регулируемого странах.|
|для взрослых|3|Пользователь должен быть обработки приложением как взрослых.|

#### <a name="consentprovidedforminor-property"></a>Свойство consentProvidedForMinor

| Значение    | # |Description|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию не `consentProvidedForMinor` имеет значение для пользователя.|
|предоставлено|1|После получения согласия пользователя для для учетной записи пользователя.|
|denied|2|Разрешения для учетной записи пользователя не были полученный.|
|notRequired|3|Пользователь является из расположения, не требуются разрешения.|

## <a name="relationships"></a>Связи

| Связь | Тип |Description|
|:---------------|:--------|:----------|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md) коллекции| Условия пользователя статусов допустимости использования. Только для чтения. Допускается значение null.|
|календарь|[calendar](calendar.md)|Основной календарь пользователя. Только для чтения.|
|calendarGroups|[calendarGroup](calendargroup.md) коллекции|Группы календарей пользователя. Только для чтения. Допускается значение null.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения. Допускается значение null.|
|calendars|Коллекция [calendar](calendar.md)|Календари пользователя. Только для чтения. Допускается значение null.|
|contactFolders|[contactFolder](contactfolder.md) коллекции|Папки контактов пользователя. Только для чтения. Допускается значение null.|
|contacts|Коллекция [contact](contact.md)|Контакты пользователя. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные пользователем. Только для чтения. Допускается значение null.|
|directReports|Коллекция [directoryObject](directoryobject.md)|Пользователи и контакты, являющиеся подчиненными пользователя (пользователи и контакты, у которых в свойстве manager указан этот пользователь). Только для чтения. Допускается значение null. |
|drive|[drive](drive.md)|Хранилище OneDrive пользователя. Только для чтения.|
|events|Коллекция [event](event.md)|События пользователя. По умолчанию отображаются события в стандартном календаре. Только для чтения. Допускается значение null.|
|extensions|Коллекция [extension](extension.md)|Коллекция open расширения, определенные для пользователя. Допускается значение null.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Классификация релевантности для сообщений пользователя, основанная на явных обозначениях, переопределяющих заданные релевантность или важность. |
|полезные сведения о|[полезные сведения о](insights.md) коллекции| Только для чтения. Допускается значение null.|
|joinedGroups|Коллекция объектов [group](group.md)| Только для чтения. Допускается значение null.|
|mailFolders|Коллекция [mailFolder](mailfolder.md)| Почтовые папки пользователя. Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)|Пользователь или контакт, являющийся руководителем пользователя. Только для чтения. (Методы HTTP: GET, PUT, DELETE.)|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, роли каталога и административных единиц измерения, которыми пользователь. Только для чтения. Допускается значение null.|
|joinedTeams|Коллекция объектов [group](group.md)|Группами Майкрософт, который входит пользователь. Только для чтения. Допускается значение null.|
|messages|Коллекция объектов [message](message.md)|Сообщения в почтовом ящике или папке. Только для чтения. Допускается значение null.|
|onenote|[OneNote](onenote.md)| Только для чтения.|
|Outlook|[outlookUser](outlookuser.md)| Выборочный Outlook службы, доступные для пользователя. Только для чтения. Допускается значение null.|
|ownedDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|людей|Коллекция [человека](person.md)| Только для чтения. Наиболее подходящих людей для пользователя. Коллекция упорядочивается по их важности для пользователя, который определяет, какие связи, совместной работы и устанавливать деловые контакты пользователя. Пользователь является объединенные данные из всех почта, контакты и социальными сетями.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля пользователя. Только для чтения.|
|photos|Коллекция [фотографий](photo.md)| Только для чтения. Допускается значение null.|
|planner|[plannerUser](planneruser.md)| Выборочный планировщик работы службы, доступные для пользователя. Только для чтения. Допускается значение null. |
|SharePoint|[SharePoint](sharepoint.md)| Доступ к сайту SharePoint пользователя. Только для чтения. |
|scopedRoleMemberOf|[scopedRoleMembership](scopedrolemembership.md) коллекции| Единица областью действия роли участие в группах для этого пользователя. Только для чтения. Допускается значение null.|
|settings|набор [параметров](user-settings.md)| Только для чтения. Допускается значение null.|
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
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
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
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "insights": { "@odata.type": "microsoft.graph.officeGraphInsights" },
  "settings": { "@odata.type": "microsoft.graph.userSettings" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "joinedTeams": [ { "@odata.type": "microsoft.graph.group" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
