---
title: Тип ресурса user
description: Представляет учетную запись пользователя Azure AD. Наследуется от directoryObject.
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 0a237a7ab6abd6c9f6c0f04dfda6174e5a0d436e
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461634"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетную запись пользователя Azure Active Directory (Azure AD). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства. Наследуется от [directoryObject](directoryobject.md).

Ресурс **user** позволяет приложениям указывать пользовательские языковые настройки и форматы даты и времени для основных почтовых ящиков Exchange пользователя и для профиля пользователя Azure AD. Дополнительную информацию см. в разделе [Пользовательские настройки языков и региональных форматов](#user-preferences-for-languages-and-regional-formats).

Чтобы повысить производительность, операции [create](../api/user-post-users.md), [get](../api/user-get.md) и [list](../api/user-list.md) возвращают только подмножество часто используемых свойств по умолчанию. Эти свойства по умолчанию указаны в разделе [Свойства](#properties). Чтобы получить любые свойства, которые не возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:------ |:----------- |:----------- |
| [Перечисление пользователей](../api/user-list.md) | Коллекция объектов [user](user.md) | Получение списка, включающего объекты user. |
| [Создание пользователя](../api/user-post-users.md) | [user](user.md) | Создание объекта user. |
| [Получение пользователя](../api/user-get.md) | [user](user.md) | Чтение свойств и связей объекта пользователя. |
| [Обновление пользователя](../api/user-update.md) | [user](user.md) | Обновление объекта пользователя. |
| [Удаление пользователя](../api/user-delete.md) | Нет | Удаление объекта пользователя. |
| [Получение дельты](../api/user-delta.md) | Коллекция пользователей | Получение добавочных изменений для пользователей. |
| [changePassword](../api/user-changepassword.md) | Нет | Обновление собственного пароля. |
| [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) | Нет | Аннулирование всех маркеров обновления пользователя, выпущенных для приложений. |
| [validatePassword](../api/user-validatepassword.md)|[passwordValidationInformation](../resources/passwordvalidationinformation.md)|Проверка пароля пользователя на соответствие политике проверки паролей организации и определение действительности пароля. |
| **Назначение ролей приложений**|||
| [Перечисление appRoleAssignments](../api/user-list-approleassignments.md) | Коллекция [appRoleAssignment](approleassignment.md) | Получение приложений и ролей приложений, назначенных пользователю. |
| [Добавление объекта appRoleAssignment](../api/user-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | Назначение роли приложения пользователю. |
| [Удаление объекта appRoleAssignment](../api/user-delete-approleassignments.md) | Нет | Удаление назначения роли приложения для пользователя. |
| **Calendar** |||
| [Создание календаря](../api/user-post-calendars.md) | [Calendar](calendar.md) | Создание объекта Calendar путем добавления в коллекцию календарей. |
| [Создание объекта calendarGroup](../api/user-post-calendargroups.md) | [CalendarGroup](calendargroup.md) | Создание объекта CalendarGroup путем записи в коллекцию групп календарей. |
| [Создание события](../api/user-post-events.md) | [event](event.md) | Создание объекта event путем публикации в коллекции объектов event. |
| [findMeetingTimes](../api/user-findmeetingtimes.md) | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) | Получение времени и местоположения для собрания с учетом доступности участника, а также ограничений по местоположению или времени. |
| [findRooms](../api/user-findrooms.md) | Коллекция [emailaddress.md](emailaddress.md) | Получение всех помещений для собраний в клиенте пользователя или определенном списке помещений. |
| [findRoomLists](../api/user-findroomlists.md) | Коллекция [emailaddress.md](emailaddress.md) | Получение списка помещений, определенных в клиенте. |
| [getSchedule](../api/calendar-getschedule.md) | [scheduleInformation](scheduleinformation.md) | Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов (комнат или оборудования) для определенного периода времени. |
| [Список календарей](../api/user-list-calendars.md) | Коллекция [Calendar](calendar.md) | Получение коллекции объектов Calendar. |
| [Список объектов calendarGroup](../api/user-list-calendargroups.md) | Коллекция [CalendarGroup](calendargroup.md) | Получение коллекции объектов CalendarGroup. |
| [Список calendarView](../api/user-list-calendarview.md) | Коллекция [event](event.md) | Получение коллекции объектов event. |
| [Получение списка событий](../api/user-list-events.md) | Коллекция [event](event.md) | Получение списка объектов event в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях. |
| [reminderView](../api/user-reminderview.md) | Коллекция [Reminder](reminder.md) | Возвращает список напоминаний календаря за указанный период времени.|
| **Контакты**|||
| [Создание контакта](../api/user-post-contacts.md)| [contact](contact.md) | Создание контакта путем добавления в коллекцию контактов. |
| [Создание объекта contactFolder](../api/user-post-contactfolders.md) | [contactFolder](contactfolder.md) | Создание объекта contactFolder путем добавления в коллекцию папок контактов. |
| [Список контактов](../api/user-list-contacts.md) | Коллекция [contact](contact.md) | Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя. |
| [Список объектов contactFolder](../api/user-list-contactfolders.md) | Коллекция [contactFolder](contactfolder.md) | Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя. |
| **Объекты каталога**|||
| [activateServicePlan](../api/user-activateserviceplan.md) | Нет | Активация службы с заданными `servicePlanId` и `skuId` для определенного [пользователя](user.md). |
| [assignLicense](../api/user-assignlicense.md) | [user](user.md) | Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской. |
| [exportPersonalData](../api/user-exportpersonaldata.md) | Нет | Отправка запроса операции политики данных, направленного администратором компании для экспорта данных пользователя организации. |
| [getByIds](../api/directoryobject-getbyids.md) | Коллекция String | Возвращает объекты каталогов, указанные в списке идентификаторов. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Коллекция String | Проверка членства в списке групп. Это транзитивная проверка. |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Коллекция String | Проверка участия в списке группы, роли каталога или объектах административных единиц. Это транзитивная проверка. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Коллекция строк | Возвращает все группы, в которых состоит пользователь. Это транзитивная проверка. |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | Коллекция строк | Возвращение всех групп, ролей каталога и административных единиц, в которых состоит пользователь. Это транзитивная проверка. |
| [Получение transitiveReports](../api/user-get-transitivereports.md) | Целое число | Получение количества транзитивных отчетов для пользователя из свойства навигации transitiveReports. |
| [Перечисление createdObjects](../api/user-list-createdobjects.md) | Коллекция [directoryObject](directoryobject.md) | Получение объектов каталога, созданных пользователем, из свойства навигации createdObjects. |
| [Перечисление licenseDetails](../api/user-list-licensedetails.md) | Коллекция объектов [licenseDetails](licensedetails.md) | Получение коллекции объектов licenseDetails. |
| [Список ownedDevices](../api/user-list-owneddevices.md) | Коллекция [directoryObject](directoryobject.md) | Получение устройств, принадлежащих пользователю, из свойства навигации ownedDevices. |
| [Список ownedObjects](../api/user-list-ownedobjects.md) | Коллекция [directoryObject](directoryobject.md) | Получение объектов каталога, принадлежащих пользователю, из свойства навигации ownedObjects. |
| [Список registeredDevices](../api/user-list-registereddevices.md) | Коллекция [directoryObject](directoryobject.md) | Получение устройств, зарегистрированных для пользователя, из свойства навигации registeredDevices. |
| [Перечисление участий с ролью в заданной области](../api/user-list-scopedrolememberof.md) | Коллекция [scopedRoleMembership](scopedrolemembership.md) | Получение участий пользователя в административных единицах с ролью в заданной области. |
| [Список usageRights](../api/user-list-usagerights.md) | Коллекция [usageRight](usageright.md) | Получение коллекции прав использования, предоставленных пользователю. |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md) | [user](user.md) | Переработка назначенных подписок для пользователя. |
| [revokeSignInSessions](../api/user-revokesigninsessions.md) | Нет | Отменяет все маркеры обновления и маркеры сеанса пользователя, выпущенные для приложений, сбрасывая значение свойства **signInSessionsValidFromDateTime** и указывая для него текущую дату и время. Это вынуждает пользователей повторно выполнить вход в эти приложения. Этот метод заменяет метод **invalidateAllRefreshTokens**. |
| [Перечисление удаленных пользователей](../api/directory-deleteditems-list.md) | Коллекция [directoryObject](directoryobject.md) | Получение пользователей, удаленных в клиенте за последние 30 дней. |
| [Получение удаленного пользователя](../api/directory-deleteditems-get.md) | Коллекция [directoryObject](directoryobject.md) | Получение удаленного пользователя по идентификатору. |
| [Восстановление удаленного пользователя](../api/directory-deleteditems-delete.md) | Коллекция [directoryObject](directoryobject.md) | Восстановление пользователя, удаленного в клиенте за последние 30 дней. |
| [Удаление пользователя без возможности восстановления](../api/directory-deleteditems-restore.md) | Коллекция [directoryObject](directoryobject.md) | Окончательное удаление пользователя из клиента. |
| **Drive** |||
| [Получение объекта drive](../api/drive-get.md) | [drive](drive.md) | Получение свойств и связей ресурса Drive. |
| [Список дочерних элементов](../api/driveitem-list-children.md) | [DriveItems](driveitem.md) | Возвращает коллекцию DriveItems в дочерних элементах ресурса DriveItem. |
| **Группы** |||
| [Перечисление объектов joinedTeams](../api/user-list-joinedteams.md) | Коллекция [team](team.md) | Получение команд Microsoft Teams, непосредственным участником которых является пользователь, из свойства навигации joinedTeams. |
| [Список memberOf](../api/user-list-memberof.md) | Коллекция [directoryObject](directoryobject.md) | Получение групп, ролей каталога и административных единиц, непосредственным участником которых является пользователь, из свойства навигации memberOf. |
| [Перечисление транзитивных свойств memberOf](../api/user-list-transitivememberof.md) | Коллекция [directoryObject](directoryobject.md) | Перечисление групп, ролей каталога и административных единиц, в которых состоит пользователь. Эта операция является транзитивной и включает группы, в которых пользователь является вложенным элементом. |
| **Аналитика** |||
| [Список "Общие"](../api/insights-list-shared.md) | Коллекция объектов [sharedInsight](insights-shared.md) | Расчетные данные, возвращающие список файлов, которыми вы поделились с пользователем. |
| [Список "Популярные"](../api/insights-list-trending.md) | Коллекция объектов [trending](insights-trending.md) | Расчетные данные, возвращающие список элементов, популярных в окружении пользователя. |
| [Список "Использованные"](../api/insights-list-used.md) | Коллекция объектов [usedInsight](insights-used.md) | Расчетные данные, возвращающие список файлов, которые вы используете вместе с пользователем. |
| **Почта** |||
| [Создание объекта inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Нет | Создание переопределения сортировки почты для отправителя, определенного SMTP-адресом. |
| [Создание объекта mailFolder](../api/user-post-mailfolders.md) | [mailFolder](mailfolder.md) | Создание объекта mailFolder путем добавления в коллекцию папок почты |
| [Создание сообщения](../api/user-post-messages.md) | [message](message.md) | Создание сообщения путем добавления в коллекцию сообщений. |
| [Создание объекта messageRule](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) | Создает объект messageRule, определяя набор условий и действий. |
| [getMailTips](../api/user-getmailtips.md) | Коллекия [mailTips](mailtips.md) | Возвращение подсказок о доступности одного или нескольких получателей для вошедшего пользователя. |
| [Список объектов mailFolder](../api/user-list-mailfolders.md) | Коллекция [mailFolder](mailfolder.md) | Получение коллекции папок почты в корневой папке вошедшего пользователя. |
| [Список сообщений](../api/user-list-messages.md) | Коллекция [message](message.md) | Получение всех сообщений в почтовом ящике вошедшего пользователя. |
| [Список переопределений](../api/inferenceclassification-list-overrides.md) | Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md) | Получение переопределений сортировки почты, настроенных пользователем для классификации сообщений от определенных отправителей. |
| [Список правил](../api/mailfolder-list-messagerules.md) | Коллекция [messageRule](messagerule.md) | Получение всех объектов messageRule, определенных для папки пользователя "Входящие". |
| [Отправка почты](../api/user-sendmail.md) | Нет | Отправка сообщения, указанного в теле запроса. |
| **Примечания** |||
| [Создание записной книжки](../api/onenote-post-notebooks.md) | [notebook](notebook.md) | Создание записной книжки OneNote. |
| [Список записных книжек](../api/onenote-list-notebooks.md) | Коллекция объектов [notebook](notebook.md) | Получение списка объектов notebook. |
| **Открытые расширения** |||
| [Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс. |
| [Получение открытого расширения](../api/opentypeextension-get.md) | Коллекция объектов [openTypeExtension](opentypeextension.md) | Получение открытого расширения, определяемого именем расширения. |
| **Организационная иерархия** |||
| [Назначение руководителя](../api/user-post-manager.md) | Нет | Назначение руководителя пользователя. |
| [Получение имени руководителя](../api/user-list-manager.md) | [directoryObject](directoryobject.md) | Получение пользователя или контакта, являющегося руководителем пользователя, из свойства навигации manager. |
| [Список directReports](../api/user-list-directreports.md) | Коллекция [directoryObject](directoryobject.md) | Получение пользователей и контактов, являющихся подчиненными данного пользователя, из свойства навигации directReports. |
| **Параметры Outlook** |||
| [Создание категории Outlook](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) | Создание объекта outlookCategory в основном списке категорий пользователя. |
| [Получение supportedLanguages](../api/outlookuser-supportedlanguages.md) | Коллекция объектов [localeInfo](localeinfo.md) | Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя. |
| [Получение supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md collection) | Получение списка поддерживаемых часовых поясов, которые настроены на сервере почтовых ящиков пользователя. |
| [Получение параметров почтового ящика пользователя](../api/user-get-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Получение объекта mailboxSettings пользователя. |
| [Список категорий Outlook](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](outlookcategory.md)                                 | Получение всех категорий, определенных для пользователя. |
| [Преобразование идентификаторов Exchange](../api/user-translateexchangeids.md) | Коллекция [convertIdResult](convertidresult.md) | Перевод идентификаторов ресурсов, связанных с Outlook, между форматами. |
| [Обновление параметров почтового ящика пользователя](../api/user-update-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Включение, настройка или отключение одного или нескольких объектов mailboxSettings пользователя. |
| **Люди** |||
| [Получение списка людей](../api/user-list-people.md) | [person](person.md) | Получение списка объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями. |
| **Фотография** |||
| [Получение фотографии](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) | Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto). |
| [Обновление объекта profilephoto](../api/profilephoto-update.md) | Нет | Обновление фотографии любого пользователя в клиенте, в том числе пользователя, выполнившего вход, либо указанной группы или контакта. |
| **Планировщик** |||
| [Получение объекта plannerUser](../api/planneruser-get.md) | [plannerUser](planneruser.md) | Получение свойств и связей объекта plannerUser. |
| [Список объектов favoritePlans](../api/planneruser-list-favoriteplans.md) | Коллекция объектов [plannerPlan](plannerplan.md) | Получение списка объектов plannerPlan, отмеченных пользователем как избранные. |
| [Список объектов recentPlans](../api/planneruser-list-recentplans.md) | Коллекция объектов [plannerPlan](plannerplan.md) | Получение списка объектов plannerPlan, недавно просмотренных пользователем. |
| [Перечисление задач](../api/planneruser-list-tasks.md) | Коллекция [plannerTask](plannertask.md) | Получает объекты plannerTask, назначенные пользователю.|
| [Обновление plannerUser](../api/planneruser-update.md) | Нет | Обновление свойств объекта plannerUser. |
| **Профиль** |||
| [Получение профиля](../api/profile-get.md) | [profile](profile.md) | Получение свойств и связей объекта profile для указанного пользователя. |
| [Удаление профиля](../api/profile-delete.md) | Нет | Удаление объекта profile из учетной записи пользователя. |
| **Расширения схемы** |||
| [Добавление значений расширений для схемы](/graph/extensibility-schema-groups) | Нет | Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных. |
| **Командная работа** |||
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md) | Коллекция [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя.|
|[Получение приложения, установленного для пользователя](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Список указанных приложений, установленных в личной области пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-post-installedapps.md) | Нет | Добавление (установка) приложения в личную область пользователя.|
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удаление приложения из личной области пользователя.|
|[Обновление приложения, установленного для пользователя](../api/userteamwork-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в личной области пользователя.|
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md)| [Чат](chat.md)| Список индивидуальных чатов между пользователем и приложением. |
| **Задачи To-Do** |||
|[Создание задачи](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Создание [todoTask](todotask.md) в указанном списке задач.|
|[Создание списка задач](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создание списка задач To Do в почтовом ящике пользователя. |
|[Перечисление задач](../api/todotasklist-list-tasks.md)|Коллекция [todoTask](todotask.md)|Получение всех ресурсов [todoTask](todotask.md) в указанном списке.|
|[Перечисление списков задач](../api/todo-list-lists.md) | Коллекция [todoTaskList](todotasklist.md) | Получение всех списков задач в почтовом ящике пользователя. |
| **Параметры пользователя** |||
| [Получение параметров](../api/usersettings-get.md) | [userSettings](usersettings.md) | Чтение объекта settings пользователя и организации. |
| [Обновление параметров](../api/usersettings-update.md) | [userSettings](usersettings.md) | Обновление свойств объекта settings. |
| **Задачи Outlook** (не рекомендуется)|||
| [Создание объекта outlookTask](../api/outlookuser-post-tasks.md) (не рекомендуется) | [outlookTask](outlooktask.md) | Создание задачи Outlook в группе задач по умолчанию ("Мои задачи") и папке задач по умолчанию ("Задачи") в почтовом ящике пользователя. |
| [Перечисление задач](../api/outlookuser-list-tasks.md) (не рекомендуется) | Коллекция объектов [outlookTask](outlooktask.md) | Получение всех задач Outlook в почтовом ящике пользователя. |
| **Облачный ПК**|||
|[Перечисление облачных ПК](../api/user-list-cloudpcs.md)|Коллекция [cloudPC](../resources/cloudpc.md)|Перечислите устройства [cloudPC](../resources/cloudpc.md), которые связаны с вошедшим пользователем.|
|[Получение сведений о запуске](../api/cloudpc-getcloudpclaunchinfo.md)|[cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md)|Получите [cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md) для вошедшего пользователя.|


## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#user-properties).

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| aboutMe | String | Свободное текстовое поле, где пользователь может рассказать о себе. <br><br>Возвращается только с помощью оператора `$select`. |
| accountEnabled | Логический | Значение `true` показывает, что учетная запись включена, значение `false` – что она отключена. Это свойство нужно обязательно указывать при создании пользователя.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not` и `in`). |
| ageGroup | [ageGroup](#agegroup-values) | Устанавливает возрастную группу пользователя. Допустимые значения: `null`, `Minor`, `NotAdult` и `Adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not` и `in`). |
| assignedLicenses | Коллекция [assignedLicense](assignedlicense.md) | Назначенные пользователю лицензии, в том числе наследуемые (на основе групп). <br><br>Значение null не допускается. Поддерживает `$filter` (`eq`, `not` и подсчитывает пустые коллекции). |
| assignedPlans | Коллекция [assignedPlan](assignedplan.md) | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.<br><br>Поддерживает `$filter` (`eq` и `not`). |
| birthday | DateTimeOffset | День рождения пользователя. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и формата времени UTC. Например, полночь 1 января 2014 г. в формате UTC представляется в виде `2014-01-01T00:00:00Z`. <br><br>Возвращается только с помощью оператора `$select`. |
| businessPhones | Коллекция String | Номера телефонов пользователя. Для этого свойства можно указать только один номер.<br><br>"Только для чтения" для пользователей, которые синхронизируются с локальным каталогом. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
| city | String | Город, в котором находится пользователь. Максимальная длина: 128 символов.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| CompanyName | String | Название организации, с которой связан пользователь. Это свойство может быть полезно для описания компании внешнего пользователя. Максимальная длина: 64 символа.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).|
| consentProvidedForMinor | [consentProvidedForMinor](#consentprovidedforminor-values) | Устанавливает, получено ли согласие для несовершеннолетних. Допустимые значения: `null`, `Granted`, `Denied` и `NotRequired`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not` и `in`).|
| country | String | Страна или регион, в котором находится пользователь, например `US` или `UK`. Максимальная длина составляет 128 символов. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| createdDateTime | DateTimeOffset | Дата и время создания пользователя. Значение не может изменяться и заполняется автоматически при создании сущности. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Свойство допускает значение null. Значение null означает, что для пользователя невозможно точно определить время создания. Только для чтения. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
| creationType | Строка | Указывает, была ли учетная запись пользователя создана с помощью одного из следующих методов: <br/> <ul><li>В качестве обычной учебной или рабочей учетной записи (`null`). <li>Как внешняя учетная запись (`Invitation`). <li>В качестве локальной учетной записи для клиента Azure Active Directory B2C (`LocalAccount`). <li>Через самообслуживаемую регистрацию внутренним пользователем с помощью проверки электронной почты (`EmailVerified`). <li>Через самообслуживаемую регистрацию внешним пользователем, регистрирующимся по ссылке, которая является частью пользовательского потока (`SelfServiceSignUp`). </ul> <br>Только для чтения.<br>Поддерживает `$filter` (`eq`, `ne`, `not` и `in`). |
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|Открытый сложный тип, который содержит значение настраиваемого атрибута безопасности, назначенного объекту каталога. Допускается значение NULL.<br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter` (`eq`, `ne`, `not`, `startsWith`).|
| deletedDateTime | DateTimeOffset | Дата и время удаления пользователя. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le` и `in`) |
| department | String | Название отдела, в котором работает пользователь. Максимальная длина: 64 символа.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `eq` и по `null` значениям). |
| displayName | Строка | Имя пользователя, отображаемое в адресной книге. Это значение обычно является сочетанием имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Максимальная длина 256 символов.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям), `$orderBy` и `$search`.|
| employeeHireDate | DateTimeOffset | Дата и время, когда пользователь был нанят или начнет работу в случае найма в будущем. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).|
| employeeId | String | Идентификатор сотрудника, назначенный пользователю организацией. Максимальная длина составляет 16 символов.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`и `eq` для значений `null`).|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |Представляет данные организации (например, подразделение и место возникновения затрат), связанные с пользователем. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).|
| employeeType | String | Фиксирует тип корпоративного работника. Например, `Employee`, `Contractor`, `Consultant` или `Vendor`. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`).|
| externalUserState | String | Для внешних пользователей, приглашенных в клиент с помощью [API приглашений](../api/invitation-post.md), это свойство представляет состояние приглашения пользователя. Для приглашенных пользователей значением состояния может быть `PendingAcceptance` или `Accepted`, а для всех остальных пользователей — `null`. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| externalUserStateChangeDateTime | String | Показывает метку времени последнего изменения в свойстве externalUserState. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| faxNumber | String | Номер факса пользователя. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| givenName | String | Простое имя пользователя. Максимальная длина: 64 символа. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| hireDate | DateTimeOffset | Дата приема пользователя на работу. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. <br><br> Возвращается только с помощью оператора `$select`. <br> **Примечание.** Это свойство относится к Microsoft Office SharePoint Online. Рекомендуем использовать собственное свойство **employeeHireDate**, чтобы устанавливать и обновлять значения даты приема на работу с помощью API Microsoft Graph. |
| id | String | Уникальный идентификатор пользователя. Необходимо считать нечетким идентификатором. Наследуется от [directoryObject](directoryobject.md). Значение null не допускается. Только для чтения. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| identities | Коллекция [objectIdentity](objectIdentity.md) | Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя. Цифровое удостоверение может предоставляться корпорацией Майкрософт (также известно как локальная учетная запись), организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя. Может содержать несколько элементов с одинаковым значением **signInType**. <br><br>Поддерживает `$filter` (`eq`), в том числе по `null` значениям, только если **signInType** не является `userPrincipalName`. |
| imAddresses | Коллекция String | Адреса мгновенных сообщений компьютерной телефонии (VOIP) по протоколу SIP для пользователя. Только для чтения. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
| infoCatalogs | Коллекция объектов string | Определяет сегменты информации, назначенные пользователю. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`). |
| interests; | Коллекция строк | Список интересов пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| isResourceAccount | Логическое | Не используйте — зарезервировано для использования в будущем. |
| jobTitle; | String | Должность пользователя. Максимальная длина: 128 символов. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| lastPasswordChangeDateTime | DateTimeOffset | Время последней смены пароля пользователем Azure AD или время создания его пароля (используется дата выполнения последнего действия). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. <br><br>Возвращается только с помощью оператора `$select`.  |
| legalAgeGroupClassification | [legalAgeGroupClassification](#legalagegroupclassification-values) | Используется корпоративными приложениями для определения юридической возрастной группы пользователя. Это свойство предназначено только для чтения. Вычисляется на основе свойств **ageGroup** и **consentProvidedForMinor**. Допустимые значения: `null`, `MinorWithOutParentalConsent`, `MinorWithParentalConsent`, `MinorNoParentalConsentRequired`, `NotAdult` и `Adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](#legal-age-group-property-definitions). <br><br>Возвращается только на `$select`. |
| licenseAssignmentStates | Коллекция [licenseAssignmentState](licenseassignmentstate.md) | Состояние назначений лицензий для пользователя. Только для чтения.<br><br>Возвращается только с помощью оператора `$select`. |
| почта; | String | SMTP-адрес пользователя, например `admin@contoso.com`. Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес. Для учетных записей Azure AD B2C это свойство можно обновить до десяти раз, используя уникальные адреса протокола SMTP. Это свойство не может содержать диакритические знаки. <br><br> Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, `endsWith` и `eq` по `null` значениям). |
| mailboxSettings | [mailboxSettings](mailboxsettings.md) | Параметры основного почтового ящика пользователя, выполнившего вход. Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры языкового стандарта, часового пояса, отправки автоматических ответов на входящие сообщения. Дополнительные сведения см. в разделе [Пользовательские настройки языков и региональных форматов](#user-preferences-for-languages-and-regional-formats).<br><br>Возвращается только с помощью оператора `$select`. |
| mailNickname | String | Псевдоним электронной почты пользователя. Это свойство должно быть указано при создании пользователя. Максимальная длина: 64 символа.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| mobilePhone | String | Основной сотовый телефон пользователя. "Только для чтения" для пользователей, которые синхронизируются с локальным каталогом. <br><br> Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| mySite | String | URL-адрес личного сайта пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| officeLocation | String | Расположение офиса на месте работы пользователя. Максимальная длина: 128 символов. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| onPremisesDistinguishedName | String | Содержит `distinguished name` или `DN` локальной службы Active Directory. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения.  |
| onPremisesDomainName | String | Содержит локальное `domainFQDN` (другое название — dnsDomainName), синхронизированное из локального каталога. Это свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. |
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | Содержит extensionAttributes1-15 для пользователя. Отдельные атрибуты расширения нельзя выбирать и фильтровать. <br><li>Для пользователей **onPremisesSyncEnabled** исходным центром управления для этого набора свойств является локальная среда, и он предназначен только для чтения. </li><li>Для исключительно облачных пользователей (где значением для **onPremisesSyncEnabled** является `false`) эти свойства можно настроить при создании или обновлении объекта пользователя.  </li><li>Для исключительно облачных пользователей, ранее синхронизированных из локальной службы Active Directory, эти свойства предназначены только для чтения в Microsoft Graph, но могут быть полностью управляемыми с помощью Центра администрирования Exchange или модуля Exchange Online версии 2 в Windows PowerShell.</li><br> Эти атрибуты расширения также называются настраиваемыми атрибутами 1–15 Exchange. <br>Возвращается только с помощью оператора `$select`. |
| onPremisesImmutableId | String | Это свойство используется для сопоставления учетной записи локальной службы Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если для свойства пользователя `userPrincipalName` (UPN) используется федеративный домен. **Примечание.** При определении этого свойства не допускается использование символов **$** и **\_**.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
| onPremisesLastSyncDateTime | DateTimeOffset | Указывает время последней синхронизации объекта с локальным каталогом, например 2013-02-16T03:04:54Z. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 и формата времени UTC. Например, полночь 1 января 2014 г. в формате UTC представляется в виде `2014-01-01T00:00:00Z`. Только для чтения. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Ошибки при использовании продукта синхронизации Майкрософт во время подготовки. <br> Поддерживает `$filter` (`eq`, `not`, `ge`, `le`).|
| onPremisesSamAccountName | String | Содержит локальное `sAMAccountName`, синхронизированное из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. <br><br> Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`).|
| onPremisesSecurityIdentifier | String | Содержит локальный идентификатор безопасности (SID) пользователя, синхронизированного из локальной среды с облаком. Только для чтения. Поддерживает `$filter` (`eq` включая значения `null`).  |
| onPremisesSyncEnabled | Логический | Значение `true` указывает, что этот объект синхронизируется из локального каталога. Значение `false` указывает, что этот объект изначально синхронизировался из локального каталога, но синхронизация больше не выполняется. Значение `null` указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям). |
| onPremisesUserPrincipalName | String | Содержит локальное `userPrincipalName`, синхронизированное из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect. Только для чтения. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`). |
| otherMails | Коллекция строк | Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.<br>ПРИМЕЧАНИЕ. Это свойство не может содержать диакритические знаки.<br><br>Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `in`, `startsWith` и подсчитывает пустые коллекции). |
| passwordPolicies | String | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением `DisableStrongPassword`, позволяющим использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Также можно указать значение `DisablePasswordExpiration`. Эти значения допускается указывать одновременно, например `DisablePasswordExpiration, DisableStrongPassword`. Дополнительную информацию о политиках паролей по умолчанию см. в разделе [Политики паролей Azure AD](/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts). <br><br>Поддерживает `$filter` (`ne`, `not` и `eq` по `null` значениям).|
| passwordProfile | [passwordProfile](passwordprofile.md) | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль. **ПРИМЕЧАНИЕ.** Для клиентов Azure B2C свойству **forceChangePasswordNextSignIn** должно быть присвоено значение `false` и вместо этого должны использоваться настраиваемые политики и пользовательские потоки для принудительного сброса пароля при первом входе. См. раздел [Принудительный сброс пароля при первом входе](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям).|
| pastProjects | Коллекция строк | Список предыдущих проектов пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| postalCode | String | Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код. Максимальная длина 40 символов.<br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| preferredDataLocation | String | Предпочитаемое расположение данных для пользователя. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](/sharepoint/dev/solution-guidance/multigeo-introduction).|
| preferredLanguage | String | Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например `en-US`. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| preferredName | String | Предпочитаемое имя пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| provisionedPlans | Коллекция [provisionedPlan](provisionedplan.md) | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`).|
| proxyAddresses | Коллекция String | Пример: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. Изменения в свойстве **почты** также обновят эту коллекцию, включив в нее значение SMTP-адреса. Дополнительные сведения см. в разделе [Свойства mail и proxyAddresses](#mail-and-proxyaddresses-properties). Прокси-адрес с префиксом `SMTP` (заглавными буквами) являются основным прокси-адресом, а адреса с префиксом `smtp` являются дополнительными прокси-адресами. Для учетных записей Azure AD B2C это свойство имеет ограничение в десять уникальных адресов. Доступно только для чтения в Microsoft Graph. Обновить это свойство можно только с помощью [Центра администрирования Microsoft 365](/exchange/recipients-in-exchange-online/manage-user-mailboxes/add-or-remove-email-addresses). Значение null не допускается. <br><br>Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`, `endsWith` и подсчитывает пустые коллекции). |
| refreshTokensValidFromDateTime | DateTimeOffset | Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. Только для чтения. Сброс можно выполнить с помощью [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md).|
| responsibilities | Коллекция строк | Список обязанностей пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| schools | Коллекция строк | Список учебных заведений, которые посещал пользователь. <br><br>Возвращается только с помощью оператора `$select`. |
| showInAddressList | Логический | Значение `true`, если глобальный список адресов Outlook должен содержать этого пользователя. В противном случае используется значение `false`. Если не задано, будет считаться, что присвоено значение `true`. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение `false`. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| signInSessionsValidFromDateTime | DateTimeOffset | Все маркеры обновления или маркеры сеансов (файлы cookie сеанса), выпущенные до этого момента, являются недопустимыми. В приложениях возникает ошибка при использовании недопустимых маркеров обновления или маркеров сеансов для получения маркера делегированного доступа (для доступа к API, например Microsoft Graph).  В этом случае приложению потребуется получить новый маркер обновления, сделав запрос к конечной точке авторизации. Только для чтения. Сброс можно выполнить с помощью [revokeSignInSessions](../api/user-revokesigninsessions.md).|
| skills | Коллекция строк | Список навыков пользователя. <br><br>Возвращается только с помощью оператора `$select`. |
| signInActivity | [signInActivity](signinactivity.md) | Получение последней даты входа в систему и идентификатора запроса на вход для указанного пользователя. Только для чтения.<br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`), *но* без других фильтруемых свойств. **Примечание.** Сведения для этого свойства требуют лицензии Azure AD Premium P1/P2 и разрешения **AuditLog.Read.All**.<br><br>**Примечание.** <br/><li>Существует [известная проблема](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) с получением этого свойства.<li>Это свойство не возвращается пользователю, который никогда не входил в систему или входил последний раз до апреля 2020 года.|
| state | String | Область, республика, край или округ в адресе пользователя. Максимальная длина: 128 символов. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| streetAddress | String | Почтовый адрес места работы пользователя. Максимальная длина: 1024 символа. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| surname | String | Фамилия пользователя. Максимальная длина: 64 символа. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям). |
| usageLocation | String | Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с юридическим требованием проверять доступность служб в разных странах. Примеры: `US`, `JP` и `GB`. Значение NULL не допускается. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).|
| userPrincipalName | String | Имя субъекта-пользователя (UPN). Это имя используется для входа через Интернет по стандарту RFC 822. Как правило, оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен, при этом домен должен входить в совокупность проверенных доменов клиента. Это свойство необходимо указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md).<br>ПРИМЕЧАНИЕ. Это свойство не может содержать диакритические знаки. Разрешены только следующие символы: `A - Z`, `a - z`, `0 - 9`, ` ' . - _ ! # ^ ~`. Полный список разрешенных символов см. в [политиках имен пользователей](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts). <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, `endsWith`) и `$orderBy`.
| userType | Строка | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`. <br><br>Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям). **ПРИМЕЧАНИЕ.** Дополнительные сведения о разрешениях для участников и гостевых пользователей см. в статье [Разрешения пользователя по умолчанию в Azure Active Directory](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users). |

### <a name="mail-and-proxyaddresses-properties"></a>свойства mail и proxyAddresses
**mail** и **proxyAddresses** — это свойства, связанные с электронной почтой. **proxyAddresses** — это коллекция адресов, относящихся только к Microsoft Exchange Server. Это свойство используется для хранения списка привязанных к одному почтовому ящику почтовых адресов пользователя. Cвойство **mail** используется в качестве адреса электронной почты пользователя для различных целей, включая вход пользователя, и определяет основной прокси-адрес.
 
Свойства **mail** и **proxyAddresses** можно получить с помощью API [GET user](../api/user-get.md) в MS Graph. Свойство **mail** можно обновить с помощью метода [PATCH в API обновления пользователя](../api/user-update.md), но свойство **proxyAddresses** нельзя обновить в Microsoft Graph. При обновлении свойства **mail** пользователя запускается перерасчет **proxyAddresses**, и обновленная почта устанавливается в качестве основного прокси-адреса, за исключением следующих сценариев: 
 
1. Если у пользователя есть лицензия, включающая Microsoft Exchange, все прокси-адреса пользователя должны относиться к проверенному домену клиента. Все, что не относится к проверенным доменам, удаляется без предупреждения.
2. Если пользователь является гостем и основной прокси-адрес содержит строку имени участника-пользователя гостя с #EXT#, почта пользователя НЕ будет установлена в качестве основного прокси-адреса.
3. Если пользователь является гостем, его почта НЕ удаляется, даже если у него больше нет прокси-адресов.
 
Адреса **proxyAddresses** уникальны для объектов каталогов (пользователей, групп и контактов организации). Если свойство **mail** пользователя конфликтует с одним из адресов **proxyAddresses** другого объекта, свойство **mail** будет обновлено; однако новое значение почты не будет добавлено в коллекцию **proxyAddresses**.

### <a name="user-preferences-for-languages-and-regional-formats"></a>Пользовательские настройки языков и региональных форматов
Ресурс **user** содержит свойство [mailboxSettings](../resources/mailboxsettings.md), включающее предпочитаемый язык пользователя, формат даты и времени, стандартный часовой пояс, и другие специальные параметры для основного почтового ящика Exchange. Эти настройки предназначены для почтовых клиентов и доступны только в том случае, если для пользователя подготовлен почтовый ящик. Вы можете использовать свойство **mailboxSettings**, если ваш сценарий предназначен только для почты, календаря, контактов и задач Outlook.

В дополнение к **mailboxSettings** ресурс **user** включает связь посредством [userSettings](../resources/usersettings.md) с [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) — надмножеством настроек языка и регионального формата, которые могут использоваться любым приложением, чтобы предоставить пользователю оптимальный языковой и региональный интерфейс. Используйте **userSettings** для обеспечения согласованного интерфейса в приложениях, имеющих доступ к профилю Azure AD, чтобы отображать одинаковые пользовательские настройки.

### <a name="legal-age-group-property-definitions"></a>Определения свойств юридических возрастных групп

В этом разделе объясняется, как три свойства возрастных групп (**legalAgeGroupClassification**, **ageGroup** и **consentProvidedForMinor**) используются администраторами Azure AD и разработчиками корпоративных приложений для соблюдения нормативных требований, связанных с возрастом.
- Свойство **legalAgeGroupClassification** доступно только для чтения. Это свойство используется разработчиками корпоративных приложений для правильной обработки пользователя с учетом его юридической возрастной группы. Оно вычисляется с учетом свойств пользователя **ageGroup** и **consentProvidedForMinor**.
- **ageGroup** и **consentProvidedForMinor** — это необязательные свойства, используемые администраторами Azure AD для обеспечения правильной обработки используемой учетной записи на основе связанных с возрастом нормативных требований, действующих в стране или регионе пользователя.

Пример: Кэмерон — администратор каталога в начальной школе г. Холипорт в Соединенном Королевстве. В начале учебного года он использует документы приемной комиссии, чтобы получить согласие родителей несовершеннолетних учащихся на основе нормативных требований Соединенного Королевства, связанных с возрастом. Согласие, полученное от родителей, позволяет использовать учетные записи несовершеннолетних учащихся в школе г. Холипорт и приложениях Майкрософт. После этого Кэмерон создает все учетные записи и присваивает свойству ageGroup значение minor, а свойству consentProvidedForMinor значение granted. Приложения, используемые учащимися, могут скрывать функции, не подходящие несовершеннолетним.

<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience but they are String types.-->

#### <a name="legalagegroupclassification-values"></a>значения legalAgeGroupClassification

| Member    | Описание|
|:---------------|:----------|
|null|Значение по умолчанию. Пользователю не присвоено свойство **ageGroup**.|
|MinorWithoutParentalConsent |(Зарезервировано для последующего использования)|
|MinorWithParentalConsent| Пользователь считается несовершеннолетним на основе связанных с возрастом нормативных требований соответствующей страны или региона. Администратор учетной записи получил соответствующее согласие от родителя или опекуна.|
|Adult|Пользователь считается взрослым на основе связанных с возрастом нормативных требований соответствующей страны или региона.|
|NotAdult|Пользователь находится в стране или регионе, использующем дополнительные нормативные требования в отношении возраста (например, США, Соединенное Королевство, Европейский союз или Южная Корея), и возраст пользователя находится между детской и взрослой категорией (устанавливается в зависимости от страны или региона). Обычно это означает, что в странах с такими требованиями подростки рассматриваются как `notAdult`.|
|MinorNoParentalConsentRequired|Пользователь является несовершеннолетним, но находится в стране без нормативных требований, связанных с возрастом.|

#### <a name="agegroup-values"></a>значения ageGroup

| Member    | Описание|
|:---------------|:--------|
|null|Значение по умолчанию. Пользователю не присвоено свойство **ageGroup**.|
|Незначительное|Пользователь считается несовершеннолетним.|
|NotAdult|Пользователь находится в стране с соответствующими нормативными положениями (США, Соединенное Королевство, Европейский союз или Южная Корея), и возраст пользователя превышает верхнюю границу детского возраста (зависит от страны), но меньше нижней границы взрослого возраста (устанавливается в зависимости от страны или региона). Как правило, в странах с такими нормами подростки рассматриваются как `notAdult`.|
|Adult|Пользователь должен считаться взрослым.|

#### <a name="consentprovidedforminor-values"></a>значения consentProvidedForMinor

| Member    | Описание|
|:---------------|:----------|
|null|Значение по умолчанию. Пользователю не присвоено свойство **consentProvidedForMinor**.|
|Granted|Для пользователя получено согласие на наличие учетной записи.|
|Denied|Для пользователя не получено согласие на наличие учетной записи.|
|NotRequired|Пользователь находится в расположении, не требующем согласия.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|agreementAcceptances|Коллекция [agreementAcceptance](agreementacceptance.md)| Состояния принятия пользователем условий использования. Только для чтения. Допускается значение NULL.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Представляет роли приложения, предоставленные пользователю для приложения. Поддерживает `$expand`. |
|authentication|[authentication](../resources/authentication.md)|**ЗАДАЧА: добавить описание**|
|calendar|[calendar](calendar.md)|Основной календарь пользователя. Только для чтения.|
|calendarGroups|Коллекция [calendarGroup](calendargroup.md)|Группы календарей пользователя. Только для чтения. Допускается значение null.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения. Допускается значение null.|
|calendars|Коллекция [calendar](calendar.md)|Календари пользователя. Только для чтения. Допускается значение null.|
|contactFolders|Коллекция [contactFolder](contactfolder.md)|Папки контактов пользователя. Только для чтения. Допускается значение null.|
|contacts|Коллекция [contact](contact.md)|Контакты пользователя. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные пользователем. Только для чтения. Допускается значение null.|
|directReports|Коллекция [directoryObject](directoryobject.md)|Пользователи и контакты, входящие в категорию подчиненных по отношению к данному пользователю (пользователи и контакты, у которых в свойстве manager указан этот пользователь). Только для чтения. Допускается значение NULL. Поддерживает `$expand`. |
|drive|[drive](drive.md)|Хранилище OneDrive пользователя. Только для чтения.|
|drives|Коллекция [drive](drive.md)| Коллекция дисков, доступных для этого пользователя. Только для чтения. |
|events|Коллекция [event](event.md)|События пользователя. По умолчанию отображаются события в стандартном календаре. Только для чтения. Допускается значение null.|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для пользователя. Допускается значение null.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Классификация релевантности для сообщений пользователя, основанная на явных обозначениях, переопределяющих заданные релевантность или важность. |
|insights|[itemInsights](iteminsights.md) | Только для чтения. Допускается значение null.|
|joinedGroups|Коллекция [group](group.md)| Только для чтения. Допускается значение null.|
|mailFolders|Коллекция [mailFolder](mailfolder.md)| Почтовые папки пользователя. Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)|Пользователь или контакт, являющийся руководителем данного пользователя. Только для чтения. (Методы HTTP: GET, PUT, DELETE.). Поддерживает `$expand`.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, роли каталога и административные единицы, в которых состоит пользователь. Только для чтения. Допускается значение NULL. Поддерживает `$expand`. |
|joinedTeams|Коллекция [team](team.md)|Команды Microsoft Teams, участником которых является пользователь. Только для чтения. Допускается значение null.|
|messages|Коллекция [message](message.md)|Сообщения в почтовом ящике или папке. Только для чтения. Допускается значение null.|
|onenote|[onenote](onenote.md)| Только для чтения.|
|outlook|[outlookUser](outlookuser.md)| Выборочные службы Outlook, доступные пользователю. Только для чтения. Допускается значение null.|
|ownedDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, принадлежащие пользователю. Только для чтения. Допускается значение NULL. Поддерживает `$expand`.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, принадлежащие пользователю. Только для чтения. Допускается значение NULL. Поддерживает `$expand`.|
|pendingAccessReviewInstances|[accessReviewInstance](accessreviewinstance.md) | Свойство навигации для получения списка проверок доступа, ожидающих утверждения проверяющим. |
|people|Коллекция [person](person.md)| Только для чтения. Наиболее релевантные люди для пользователя. Коллекция упорядочена по их релевантности для пользователя, которая определяется его общением, совместной работой и бизнес-связями. Человек представляется в виде агрегированных сведений из почты, контактов и социальных сетей.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля пользователя. Только для чтения.|
|photos|Коллекция [photo](photo.md)| Только для чтения. Допускается значение null.|
|planner|[plannerUser](planneruser.md)| Выборочные службы Планировщика, доступные пользователю. Только для чтения. Допускается значение null. |
|profile |[profile](profile.md) | Представляет свойства, описывающие пользователей в клиенте. |
|registeredDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, зарегистрированные для пользователя. Только для чтения. Допускается значение null. Поддержка `$expand`.|
|scopedRoleMemberOf|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Участие пользователя в административных единицах с ролью в заданной области. Только для чтения. Допускается значение null.|
|settings|[userSettings](usersettings.md) | Только для чтения. Допускается значение null.|
|teamwork|[userTeamwork](userteamwork.md)| Контейнер для функций Microsoft Teams, доступных пользователю. Только для чтения. Допускается значение null.|
|todo|[todo](todo.md)|Представляет службы To Do, доступные пользователю. |
|transitiveReports|Коллекция [directoryObject](directoryobject.md) | Транзитивные отчеты для пользователя. Только для чтения.|
|usageRights|Коллекция [usageRight](usageright.md)|Представляет права использования, предоставленные пользователю. |

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
    "profile",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "String",
  "accountEnabled": true,
  "ageGroup": "String",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["String"],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "2019-02-07T21:53:13.067Z",
  "creationType": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "deletedDateTime": "String (timestamp)",
  "department": "String",
  "displayName": "String",
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "String",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "String",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "faxNumber": "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "id": "String (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "interests": ["String"],
  "isResourceAccount": false,
  "jobTitle": "String",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "String",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "String",
  "mobilePhone": "String",
  "mySite": "String",
  "officeLocation": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesDomainName": "String",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "String",
  "otherMails": ["String"],
  "passwordPolicies": "String",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["String"],
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "preferredName": "String",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["String"],
  "refreshTokensValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "responsibilities": ["String"],
  "schools": ["String"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "skills": ["String"],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
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
  "insights": {"@odata.type": "microsoft.graph.itemInsights"},
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
  "profile": {"@odata.type": "microsoft.graph.profile"},
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
