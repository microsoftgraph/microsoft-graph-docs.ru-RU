---
title: Тип ресурса user
description: Represents an Azure AD user account. Inherits from directoryObject.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: dc425a389984e8fe4717820e640b910e9ca486a1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863770"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

## <a name="methods"></a>Методы

| Метод                                                                                     | Возвращаемый тип                                                                      | Описание                                                                                                                                                                                                                         |
|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Перечисление пользователей](../api/user-list.md)                                                          | Коллекция объектов [user](user.md)                                                       | Получение списка, включающего объекты user.                                                                                                                                                                                                         |
| [Создание пользователя](../api/user-post-users.md)                                                   | [user](user.md)                                                                  | Создание объекта user.                                                                                                                                                                                                           |
| [Получение пользователя](../api/user-get.md)                                                             | [user](user.md)                                                                  | Чтение свойств и связей объекта пользователя.                                                                                                                                                                                   |
| [Обновление пользователя](../api/user-update.md)                                                       | [user](user.md)                                                                  | Обновление объекта пользователя.                                                                                                                                                                                                                 |
| [Удаление пользователя](../api/user-delete.md)                                                       | Нет                                                                             | Удаление объекта пользователя.                                                                                                                                                                                                                 |
| [Получение дельты](../api/user-delta.md)                                                          | Коллекция объектов [user](user.md)                                                       | Получение добавочных изменений для пользователей.                                                                                                                                                                                                  |
| **Назначения ролей приложений**                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [Перечисление appRoleAssignments](../api/user-list-approleassignments.md)                          | Коллекция [appRoleAssignment](approleassignment.md)                             | Получение приложений и ролей приложений, которым назначен этот пользователь.                                                                                                                                                                       |
| [Добавление Аппролеассигнмент](../api/user-post-approleassignments.md)                            | [appRoleAssignment](approleassignment.md)                                        | Назначьте роль приложения этому пользователю.                                                                                                                                                                                                    |
| [Удаление Аппролеассигнмент](../api/user-delete-approleassignments.md)                       | Нет                                                                             | Удаление назначения роли приложения для этого пользователя.                                                                                                                                                                                       |
| **Календарь**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание календаря](../api/user-post-calendars.md)                                           | [Calendar](calendar.md)                                                          | Создание объекта Calendar путем добавления в коллекцию календарей.                                                                                                                                                                       |
| [Создание объекта calendarGroup](../api/user-post-calendargroups.md)                                 | [CalendarGroup](calendargroup.md)                                                | Создание объекта CalendarGroup путем записи в коллекцию групп календарей.                                                                                                                                                             |
| [Создание события](../api/user-post-events.md)                                                 | [event](event.md)                                                                | Создание объекта event путем публикации в коллекции объектов event.                                                                                                                                                                             |
| [findMeetingTimes](../api/user-findmeetingtimes.md)                                        | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)                  | Получение времени и местоположения для собрания с учетом доступности участника, а также ограничений по местоположению или времени.                                                                                                                                      |
| [getSchedule](../api/calendar-getschedule.md)                                              | [scheduleInformation](scheduleinformation.md)                                    | Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов (комнат или оборудования) для определенного периода времени.                                                                           |
| [Список календарей](../api/user-list-calendars.md)                                            | Коллекция [calendar](calendar.md)                                               | Получение коллекции объектов Calendar.                                                                                                                                                                                                   |
| [Список объектов calendarGroup](../api/user-list-calendargroups.md)                                  | Коллекция [calendarGroup](calendargroup.md)                                     | Получение коллекции объектов CalendarGroup.                                                                                                                                                                                              |
| [Список calendarView](../api/user-list-calendarview.md)                                      | Коллекция [event](event.md)                                                     | Получение коллекции объектов Event.                                                                                                                                                                                                      |
| [Получение списка событий](../api/user-list-events.md)                                                  | Коллекция [event](event.md)                                                     | Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.                                                                                                                   |
| [reminderView](../api/user-reminderview.md)                                                | Коллекция [Reminder](reminder.md)                                               | Возвращает список напоминаний календаря за указанный период времени.                                                                                                                                                       |
| **Контакты**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание контакта](../api/user-post-contacts.md)                                             | [contact](contact.md)                                                            | Создание объекта Contact путем добавления в коллекцию контактов.                                                                                                                                                                         |
| [Создание объекта contactFolder](../api/user-post-contactfolders.md)                                 | [contactFolder](contactfolder.md)                                                | Создание объекта ContactFolder путем добавления в коллекцию папок контактов.                                                                                                                                                             |
| [Список контактов](../api/user-list-contacts.md)                                              | Коллекция [contact](contact.md)                                                 | Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя.                                                                                                                                                    |
| [Список объектов contactFolder](../api/user-list-contactfolders.md)                                  | Коллекция [contactFolder](contactfolder.md)                                     | Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.                                                                                                                                             |
| **Объекты каталога**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [assignLicense](../api/user-assignlicense.md)                                              | [user](user.md)                                                                  | Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.                                                                                                            |
| [checkMemberGroups](../api/user-checkmembergroups.md)                                      | Коллекция String                                                                | Check for membership in a list of groups. The check is transitive.                                                                                                                                                                  |
| [checkMemberObjects](../api/user-checkmemberobjects.md)                                    | Коллекция String                                                                | Проверка участия в списке группы, роли каталога или объектах административных единиц. Это транзитивная функция.                                                                                                                |
| [exportPersonalData](../api/user-exportpersonaldata.md)                                    | Нет                                                                             | Отправка запроса операции политики данных, направленного администратором компании для экспорта данных пользователя организации.                                                                                                                   |
| [getByIds](../api/directoryobject-getbyids.md)                                             | Коллекция String                                                                | Возвращает объекты каталогов, указанные в списке идентификаторов.                                                                                                                                                                           |
| [getMemberGroups](../api/user-getmembergroups.md)                                          | Коллекция String                                                                | Return all the groups that the user is a member of. The check is transitive.                                                                                                                                                        |
| [getMemberObjects](../api/user-getmemberobjects.md)                                        | Коллекция строк                                                                | Return all of the groups and directory roles that the user is a member of. The check is transitive.                                                                                                                                 |
| [Перечисление createdObjects](../api/user-list-createdobjects.md)                                  | Коллекция [directoryObject](directoryobject.md)                                 | Получение объектов каталога, созданных пользователем, из свойства навигации createdObjects.                                                                                                                                          |
| [Перечисление licenseDetails](../api/user-list-licensedetails.md)                                  | Коллекция объектов [licenseDetails](licensedetails.md)                                   | Получение коллекции объектов licenseDetails.                                                                                                                                                                                             |
| [Список ownedDevices](../api/user-list-owneddevices.md)                                      | Коллекция [directoryObject](directoryobject.md)                                 | Получение устройств, принадлежащих пользователю, из свойства навигации ownedDevices.                                                                                                                                               |
| [Список ownedObjects](../api/user-list-ownedobjects.md)                                      | Коллекция [directoryObject](directoryobject.md)                                 | Получение объектов каталога, принадлежащих пользователю, из свойства навигации ownedObjects.                                                                                                                                     |
| [Список registeredDevices](../api/user-list-registereddevices.md)                            | Коллекция [directoryObject](directoryobject.md)                                 | Получение устройств, зарегистрированных для пользователя, из свойства навигации registeredDevices.                                                                                                                                    |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md)                              | [user](user.md)                                                                  | Переработка назначенных подписок для пользователя.                                                                                                                                                                                    |
| [revokeSignInSessions](../api/user-revokesigninsessions.md)                                | Нет                                                                             | Отменяет все маркеры обновления и маркеры сеанса пользователя, выпущенные для приложений, сбрасывая значение свойства **signInSessionsValidFromDateTime** и указывая для него текущую дату и время. Это вынуждает пользователей повторно выполнить вход в эти приложения. |
| **Drive**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Получение объекта drive](../api/drive-get.md)                                                           | [drive](drive.md)                                                                | Получение свойств и связей ресурса Drive.                                                                                                                                                                      |
| [Список дочерних элементов](../api/driveitem-list-children.md)                                         | [DriveItems](driveitem.md)                                                       | Возвращает коллекцию DriveItems в дочерних элементах ресурса DriveItem.                                                                                                                                                      |
| **Группы**                                                                                 |                                                                                  |                                                                                                                                                                                                                                     |
| [Перечисление объектов joinedTeams](../api/user-list-joinedteams.md)                                        | Коллекция [team](team.md)                                                       | Получение команд Microsoft Teams, непосредственным участником которых является пользователь, из свойства навигации joinedTeams.                                                                                                                         |
| [Список memberOf](../api/user-list-memberof.md)                                              | Коллекция [directoryObject](directoryobject.md)                                 | Получение групп и ролей каталога, непосредственным участником которых является пользователь, из свойства навигации memberOf.                                                                                                                       |
| [Перечисление транзитивных свойств memberOf](../api/user-list-transitivememberof.md)                         | Коллекция [directoryObject](directoryobject.md)                                 | Перечисление групп и ролей каталога, участником которых является пользователь. Эта операция является транзитивной и включает группы, в которых пользователь является вложенным элементом.                                                                         |
| **Почта**                                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание объекта inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Создание переопределения сортировки почты для отправителя, определенного SMTP-адресом.      |                                                                                                                                                                                                                                     |
| [Создание объекта mailFolder](../api/user-post-mailfolders.md)                                       | [mailFolder](mailfolder.md)                                                      | Создание объекта MailFolder путем добавления в коллекцию папок почты.                                                                                                                                                                   |
| [Создание сообщения](../api/user-post-messages.md)                                             | [message](message.md)                                                            | Создание объекта Message путем добавления в коллекцию сообщений.                                                                                                                                                                         |
| [Создание объекта messageRule](../api/mailfolder-post-messagerules.md)                               | [messageRule](messagerule.md)                                                    | Создает объект messageRule, определяя набор условий и действий.                                                                                                                                                          |
| [getMailTips](../api/user-getmailtips.md)                                                  | Коллекия [mailTips](mailtips.md)                                               | Возвращение подсказок о доступности одного или нескольких получателей для вошедшего пользователя.                                                                                                                                                   |
| [Список объектов mailFolder](../api/user-list-mailfolders.md)                                        | Коллекция [mailFolder](mailfolder.md)                                           | Получение коллекции папок почты в корневой папке вошедшего пользователя.                                                                                                                                                         |
| [Список сообщений](../api/user-list-messages.md)                                              | Коллекция [message](message.md)                                                 | Получение всех сообщений в почтовом ящике вошедшего пользователя.                                                                                                                                                                               |
| [Список переопределений](../api/inferenceclassification-list-overrides.md)                         | Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md) | Получение переопределений сортировки почты, настроенных пользователем для классификации сообщений от определенных отправителей.                                                                                                           |
| [Список правил](../api/mailfolder-list-messagerules.md)                                       | Коллекция [messageRule](messagerule.md)                                         | Получение всех объектов messageRule, определенных для папки пользователя "Входящие".                                                                                                                                                                       |
| [Отправка почты](../api/user-sendmail.md)                                                       | Нет                                                                             | Отправка сообщения, указанного в теле запроса.                                                                                                                                                                                     |
| **Примечания**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание записной книжки](../api/onenote-post-notebooks.md)                                        | [notebook](notebook.md)                                                          | Создание записной книжки OneNote.                                                                                                                                                                                                      |
| [Список записных книжек](../api/onenote-list-notebooks.md)                                         | Коллекция объектов [notebook](notebook.md)                                               | Получение списка объектов notebook.                                                                                                                                                                                                |
| **Открытые расширения**                                                                        |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md)                | [openTypeExtension](opentypeextension.md)                                        | Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.                                                                                                                                                   |
| [Получение открытого расширения](../api/opentypeextension-get.md)                                      | Коллекция объектов [openTypeExtension](opentypeextension.md)                             | Получение открытого расширения, определяемого именем расширения.                                                                                                                                                                             |
| **Организационная иерархия**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [Назначение руководителя](../api/user-post-manager.md)                                              | [directoryObject](directoryobject.md)                                            | Назначение пользователя или контакта организации в качестве руководителя пользователя.                                                                                                                                                                  |
| [Получение имени руководителя](../api/user-list-manager.md)                                                 | [directoryObject](directoryobject.md)                                            | Получение пользователя или контакта организации, являющегося руководителем пользователя, из свойства навигации manager.                                                                                                                            |
| [Список directReports](../api/user-list-directreports.md)                                    | Коллекция [directoryObject](directoryobject.md)                                 | Получение пользователей и контактов, являющихся подчиненными данного пользователя, из свойства навигации directReports.                                                                                                                                      |
| **Параметры Outlook**                                                                       |                                                                                  |                                                                                                                                                                                                                                     |
| [Создание категории Outlook](../api/outlookuser-post-mastercategories.md)                     | [outlookCategory](outlookcategory.md)                                            | Создание объекта outlookCategory в основном списке категорий пользователя.                                                                                                                                                           |
| [Получение supportedLanguages](../api/outlookuser-supportedlanguages.md)                         | Коллекция объектов [localeInfo](localeinfo.md)                                           | Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.                                                                                                                  |
| [Получение supportedTimeZones](../api/outlookuser-supportedtimezones.md)                         | [timeZoneInformation](timezoneinformation.md collection)                         | Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя.                                                                                                                             |
| [Получение параметров почтового ящика пользователя](../api/user-get-mailboxsettings.md)                            | [mailboxSettings](mailboxsettings.md)                                            | Получение объекта mailboxSettings пользователя.                                                                                                                                                                                                     |
| [Список категорий Outlook](../api/outlookuser-list-mastercategories.md)                     | Коллекция [outlookCategory](outlookcategory.md)                                 | Получение всех категорий, определенных для пользователя.                                                                                                                                                                         |
| [Преобразование идентификаторов Exchange](../api/user-translateexchangeids.md)                              | Коллекция [convertIdResult](convertidresult.md)                                 | Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.                                                                                                                                                                 |
| [Обновление параметров почтового ящика пользователя](../api/user-update-mailboxsettings.md)                      | [mailboxSettings](mailboxsettings.md)                                            | Включение, настройка или отключение одного или нескольких объектов mailboxSettings пользователя.                                                                                                                                                                   |
| **Фотография**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Получение фотографии](../api/profilephoto-get.md)                                                    | [profilePhoto](profilephoto.md)                                                  | Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).                                                                                                                                                           |
| [Обновление объекта profilephoto](../api/profilephoto-update.md)                                       | Нет                                                                             | Обновление фотографии любого пользователя в клиенте, в том числе пользователя, выполнившего вход, либо указанной группы или контакта.                                                                                                                        |
| **Планировщик**                                                                                |                                                                                  |                                                                                                                                                                                                                                     |
| [Перечисление задач](../api/planneruser-list-tasks.md)                                             | Коллекция [plannerTask](plannertask.md)                                         | Получает объекты plannerTask, назначенные пользователю.                                                                                                                                                                                              |
| **Расширения схемы**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [Добавление значений расширений для схемы](/graph/extensibility-schema-groups)                          | Нет                                                                             | Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.                                                                                                                                        |
| **Параметры пользователя**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [Получение параметров](../api/usersettings-get.md)                                                 | [userSettings](usersettings.md)                                                  | Чтение объекта settings пользователя и организации.                                                                                                                                                                                     |
| [Обновление параметров](../api/usersettings-update.md)                                           | [userSettings](usersettings.md)                                                  | Обновление свойств объекта settings.                                                                                                                                                                                       |

## <a name="properties"></a>Свойства

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|aboutMe|String|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Boolean| **true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.    |
|ageGroup|String|Устанавливает возрастную группу пользователя. Допустимые значения: `null`, `minor`, `notAdult` и `adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions). |
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|The licenses that are assigned to the user. Not nullable.            |
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|The plans that are assigned to the user. Read-only. Not nullable. |
|birthday|DateTimeOffset|The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|businessPhones|Коллекция String|The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.|
|city|String|The city in which the user is located. Supports $filter.|
|companyName | String | Название организации, с которой связан пользователь. Это свойство может быть полезно для описания компании внешнего пользователя. |
|consentProvidedForMinor|String|Устанавливает, получено ли согласие для несовершеннолетних. Допустимые значения: `null`, `granted`, `denied` и `notRequired`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions).|
|country|Строка|The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.|
|createdDateTime | DateTimeOffset |Дата создания объекта пользователя. |
|creationType|String|Указывает, была ли учетная запись пользователя создана как обычная учебная или рабочая учетная запись (`null`), внешняя учетная запись (`Invitation`), локальная учетная запись для клиента Azure Active Directory B2C (`LocalAccount`) или с помощью самостоятельной регистрации с использованием проверки электронной почты (`EmailVerified`). Только для чтения.|
|deletedDateTime| DateTimeOffset | Дата и время удаления пользователя. <br><br>Возвращается только с помощью оператора $select. |
|department|String|The name for the department in which the user works. Supports $filter.|
|displayName|String|The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|employeeId|String|Идентификатор сотрудника, назначенный пользователю организацией. Поддерживает параметр $filter.|
|externalUserState|String|Для внешних пользователей, приглашенных в клиент с помощью [API приглашений](../api/invitation-post.md), это свойство представляет состояние приглашения пользователя. Для приглашенных пользователей значением состояния может быть `PendingAcceptance` или `Accepted`, а для всех остальных пользователей — `null`. <br><br>Возвращается только для `$select` . Поддерживает `$filter` Поддерживаемые значения. Пример: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|DateTimeOffset|Показывает отметку времени последнего изменения свойства **Свойства** . <br><br>Возвращается только для `$select` .|
|faxNumber|String|Номер факса пользователя.|
|givenName|String|The given name (first name) of the user. Supports $filter.|
|hireDate|DateTimeOffset|The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|id|String|The unique identifier for the user. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.|
|identities|Коллекция [objectIdentity](objectIdentity.md)| Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя. Цифровое удостоверение может предоставляться корпорацией Майкрософт (также известно как локальная учетная запись), организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя. Может содержать несколько элементов с одинаковым значением **signInType**. <br>Поддерживает параметр $filter.|
|imAddresses|Коллекция String|The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.|
|interests|Коллекция строк|Список интересов пользователя.|
|isResourceAccount|Boolean| Не используйте зарезервированное резервирование для будущего использования.|
|jobTitle;|String|The user’s job title. Supports $filter.|
|lastPasswordChangeDateTime| DateTimeOffset | Время последнего изменения своего пароля пользователем Azure AD. Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z"|
|legalAgeGroupClassification|String| Используется корпоративными приложениями для определения юридической возрастной группы пользователя. Это свойство предназначено только для чтения. Вычисляется на основе свойств `ageGroup` и `consentProvidedForMinor`. Допустимые значения: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` и `adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions).|
|licenseAssignmentStates|Коллекция [licenseAssignmentState](licenseassignmentstate.md)|Состояние назначений лицензий для пользователя. Только для чтения.|
|mail|String|The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com". Read-Only. Supports $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Settings for the primary mailbox of the signed-in user. You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) settings for sending automatic replies to incoming messages, locale and time zone.|
|mailNickname|String|The mail alias for the user. This property must be specified when a user is created. Supports $filter.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|mySite|String|URL-адрес личного сайта пользователя.|
|officeLocation|String|Расположение офиса на месте работы пользователя.|
|onPremisesDistinguishedName|String| Содержит параметры локальной службы Active Directory `distinguished name` или `DN`. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesDomainName|String| Содержит локальный параметр `domainFQDN`, также называемый dnsDomainName, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Содержит свойства extensionAttribute 1–15 для пользователя. Обратите внимание, что отдельные атрибуты расширения нельзя выбирать и фильтровать. Для `onPremisesSyncEnabled` пользователя источник полномочий для этого набора свойств является локальным и доступен только для чтения. Для исключительно облачных пользователей (где значением для `onPremisesSyncEnabled` является false) эти свойства можно задать при создании или обновлении. Эти атрибуты расширения также называются пользовательскими атрибутами Exchange 1-15. |
|onPremisesImmutableId|String|Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен. **Важно!** В этом свойстве не допускается использование символов **$** и **\_**. Поддерживает параметр $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indicates the last time at which the object was synced with the on-premises directory; for example: "2013-02-16T03:04:54Z". The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.|
|onPremisesProvisioningErrors|Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Ошибки при использовании продукта синхронизации Майкрософт во время подготовки. |
|onPremisesSamAccountName|String| Содержит локальный параметр `samAccountName`, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|onPremisesSecurityIdentifier|String|Contains the on-premises security identifier (SID) for the user that was synchronized from on-premises to the cloud. Read-only.|
|onPremisesSyncEnabled|Boolean| **true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default). Read-only |
|onPremisesUserPrincipalName|String| Содержит локальный параметр `userPrincipalName`, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
|otherMails|String| Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`. Поддерживает параметр $filter.|
|passwordPolicies|String|Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.|
|pastProjects|Коллекция String|Список предыдущих проектов пользователя.|
|postalCode|String|The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.|
|preferredDataLocation|String|Предпочитаемое расположение данных для пользователя. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".|
|preferredName|String|Предпочитаемое имя пользователя.|
|provisionedPlans|Коллекция [provisionedPlan](provisionedplan.md)|The plans that are provisioned for the user. Read-only. Not nullable. |
|proxyAddresses|Коллекция строк|For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties. Read-only, Not nullable. Supports $filter.|
|refreshTokensValidFromDateTime|DateTimeOffset|Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. <br><br>Возвращается только с помощью оператора $select. Только для чтения. |
|responsibilities;|Коллекция String|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|showInAddressList|Boolean|Значение **true**, если глобальный список адресов Outlook должен содержать этого пользователя. В противном случае используется значение **false**. Если не задано, будет считаться, что присвоено значение **true**. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение **false**.|
|skills|Коллекция строк|Список навыков пользователя.|
|signInSessionsValidFromDateTime|DateTimeOffset| Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. Только для чтения. Сброс можно выполнить с помощью [revokeSignInSessions](../api/user-revokesigninsessions.md).|
|state|Строка|The state or province in the user's address. Supports $filter.|
|streetAddress|String|Почтовый адрес места работы пользователя.|
|surname|String|The user's surname (family name or last name). Supports $filter.|
|usageLocation|String|A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.|
|userPrincipalName|String|The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](organization.md). Supports $filter and $orderby.
|userType|String|A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.          |

### <a name="legal-age-group-property-definitions"></a>Определения свойств возрастных групп

В этом разделе объясняется, как три свойства возрастных групп (`legalAgeGroupClassification`, `ageGroup` и `consentProvidedForMinor`) используются администраторами Azure AD и разработчиками корпоративных приложений для соблюдения нормативных требований, связанных с возрастом.

Пример: Кэмерон — администратор каталога в начальной школе г. Холипорт в Соединенном Королевстве. В начале учебного года он использует документы приемной комиссии, чтобы получить согласие родителей несовершеннолетних учащихся на основе нормативных требований Соединенного Королевства, связанных с возрастом. Согласие, полученное от родителей, позволяет использовать учетные записи несовершеннолетних учащихся в школе г. Холипорт и приложениях Майкрософт. После этого Кэмерон создает все учетные записи и присваивает свойству ageGroup значение minor, а свойству consentProvidedForMinor значение granted. Приложения, используемые учащимися, могут скрывать функции, не подходящие несовершеннолетним.

#### <a name="legal-age-group-classification"></a>Классификация юридических возрастных групп

Это свойство, предназначенное только для чтения, используется разработчиками корпоративных приложений для правильной обработки пользователя с учетом его юридической возрастной группы. Оно вычисляется с учетом свойств пользователя `ageGroup` и `consentProvidedForMinor`.

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|нуль|Значение по умолчанию. Пользователю не присвоено свойство `ageGroup`.|
|minorWithoutParentalConsent |1 |(Зарезервировано для последующего использования)|
|minorWithParentalConsent|2| Пользователь считается несовершеннолетним на основе связанных с возрастом нормативных требований соответствующей страны или региона. Администратор учетной записи получил соответствующее согласие от родителя или опекуна.|
|adult|4|Пользователь считается взрослым на основе связанных с возрастом нормативных требований соответствующей страны или региона.|
|notAdult|4 |Пользователь находится в стране или регионе, использующем дополнительные нормативные требования в отношении возраста (например, США, Соединенное Королевство, Европейский союз или Южная Корея), и возраст пользователя находится между категорией несовершеннолетия и взрослой категорией (устанавливается в зависимости от страны или региона). Обычно это означает, что в странах с регулированием подростки относятся к категории `notAdult`.|
|minorNoParentalConsentRequired|5 |Пользователь является несовершеннолетним, но находится в стране без нормативных требований, связанных с возрастом.|

#### <a name="age-group-and-minor-consent"></a>Возрастная группа и согласие для несовершеннолетних

Возрастная группа и согласие для несовершеннолетних — это необязательные свойства, используемые администраторами Azure AD для обеспечения правильной обработки используемой учетной записи на основе связанных с возрастом нормативных требований, действующих в стране или регионе пользователя.

#### <a name="agegroup-property"></a>Свойство ageGroup

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|нуль|Значение по умолчанию. Пользователю не присвоено свойство `ageGroup`.|
|minor|1 |Пользователь считается незначительным.|
|notAdult|2|Пользователь находится в стране с нормативными положениями (США, Соединенное Королевство, Европейский союз и Южная Корея) и возраст пользователя превышает верхнюю границу детского возраста (зависит от страны), но меньше нижней границы взрослого возраста (устанавливается в зависимости от страны или региона). По существу, в странах с регулированием подростки относятся к категории `notAdult`.|
|adult|4|Пользователь должен считаться взрослым.|

#### <a name="consentprovidedforminor-property"></a>Свойство consentProvidedForMinor

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|нуль|Значение по умолчанию. Пользователю не присвоено свойство `consentProvidedForMinor`.|
|granted|1 |Для пользователя получено согласие на наличие учетной записи.|
|denied|2|Для пользователя не получено согласие на наличие учетной записи.|
|notRequired|4|Пользователь находится в расположении, не требующем согласия.|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|activities|Коллекция [userActivity](projectrome-activity.md)|Действия пользователя на разных устройствах. Только для чтения. Допускается значение null.|
|calendar|[calendar](calendar.md)|The user's primary calendar. Read-only.|
|calendarGroups|Коллекция [calendarGroup](calendargroup.md)|The user's calendar groups. Read-only. Nullable.|
|calendarView|Коллекция [event](event.md)|The calendar view for the calendar. Read-only. Nullable.|
|calendars|Коллекция [calendar](calendar.md)|The user's calendars. Read-only. Nullable.|
|contactFolders|Коллекция [contactFolder](contactfolder.md)|The user's contacts folders. Read-only. Nullable.|
|contacts|Коллекция [contact](contact.md)|The user's contacts. Read-only. Nullable.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Directory objects that were created by the user. Read-only. Nullable.|
|directReports|Коллекция [directoryObject](directoryobject.md)|The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable. |
|drive|[drive](drive.md)|The user's OneDrive. Read-only.|
|drives|Коллекция [drive](drive.md)| A collection of drives available for this user. Read-only. |
|events|Коллекция [event](event.md)|The user's events. Default is to show Events under the Default Calendar. Read-only. Nullable.|
|extensions|Коллекция [extension](extension.md)|The collection of open extensions defined for the user. Read-only. Nullable.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | Классификация релевантности для сообщений пользователя, основанная на явных обозначениях, переопределяющих заданные релевантность или важность. |
|insights|[officeGraphInsights](officegraphinsights.md) | Read-only. Nullable.|
|licenseDetails|Коллекция объектов [licenseDetails](licensedetails.md)|Коллекция сведений о лицензии этого пользователя. Только для чтения.|
|mailFolders|Коллекция [mailFolder](mailfolder.md)| The user's mail folders. Read-only. Nullable.|
|manager|[directoryObject](directoryobject.md)|The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)|
|memberOf|Коллекция [directoryObject](directoryobject.md)|The groups and directory roles that the user is a member of. Read-only. Nullable.|
|messages|Коллекция [message](message.md)|The messages in a mailbox or folder. Read-only. Nullable.|
|onenote|[onenote](onenote.md)| Только для чтения.|
|outlook|[outlookUser](outlookuser.md)| Только для чтения.|
|ownedDevices|Коллекция [directoryObject](directoryobject.md)|Devices that are owned by the user. Read-only. Nullable.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Directory objects that are owned by the user. Read-only. Nullable.|
|people|Коллекция [person](person.md)| Люди, которые являются релевантными для пользователя. Только для чтения. Допускается значение null.
|photo|[profilePhoto](profilephoto.md)| The user's profile photo. Read-only.|
|planner|[plannerUser](planneruser.md)| Точка входа в ресурс Planner, который может существовать для пользователя. Только для чтения.|
|registeredDevices|Коллекция [directoryObject](directoryobject.md)|Devices that are registered for the user. Read-only. Nullable.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "createdDateTime": "String (timestamp)",
  "creationType": "string",
  "department": "string",
  "displayName": "string",
  "employeeId": "string",
  "faxNumber" : "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "imAddresses": ["string"],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "lastPasswordChangeDateTime": "String (timestamp)",
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
  "otherMails": "string",
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
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
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
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
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
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
