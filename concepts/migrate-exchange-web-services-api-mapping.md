---
title: Exchange веб-служб (EWS) с сопоставлением API Graph Майкрософт
description: В этой статье перечислены API microsoft Graph, которые сопоставляются Exchange API веб-служб (EWS).
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 93ecef5daccc29743a74258eae1624e8e78dcd4f
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549612"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange веб-служб (EWS) с сопоставлением API Graph Майкрософт

В этой статье перечислены API microsoft Graph, которые сопоставляются Exchange API веб-служб (EWS).

## <a name="utility-apis"></a>Программные API

| EWS API                                                                                             | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [Перевод Exchange идентификаторов](/graph/api/user-translateexchangeids) |
| [ResolveNames](/exchange/client-developer/web-service-reference/resolvenames-operation)             | [Получение списка людей](/graph/api/user-list-people) |
| [GetServerTimeZones](/exchange/client-developer/web-service-reference/getservertimezones-operation) | [Получение настроек часовых поясов](/graph/api/outlookuser-supportedtimezones) |

## <a name="mail-apis"></a>API почты

### <a name="messages"></a>Сообщения

| EWS API                                                                             | API Microsoft Graph |
|-------------------------------------------------------------------------------------|-----|
| [CreateItem](/exchange/client-developer/web-service-reference/createitem-operation) | [Создание сообщения](/graph/api/user-post-messages) |
| [CopyItem](/exchange/client-developer/web-service-reference/copyitem-operation)     | [Копирование сообщения](/graph/api/message-copy) |
| [DeleteItem](/exchange/client-developer/web-service-reference/deleteitem-operation) | [Удалить сообщение](/graph/api/message-delete) |
| [FindItem](/exchange/client-developer/web-service-reference/finditem-operation)     | [Список сообщений](/graph/api/user-list-messages) |
| [GetItem](/exchange/client-developer/web-service-reference/getitem-operation)       | [Получение сообщения](/graph/api/message-get) |
| [MoveItem](/exchange/client-developer/web-service-reference/moveitem-operation)     | [Перемещение сообщения](/graph/api/message-move) |
| [SendItem](/exchange/client-developer/web-service-reference/senditem-operation)     | [Отправка сообщения](/graph/api/message-send) или [отправка почты](/graph/api/user-sendmail) |
| [UpdateItem](/exchange/client-developer/web-service-reference/updateitem-operation) | [Обновление сообщения](/graph/api/message-update) |

### <a name="folders"></a>Folders

| EWS API                                                                                 | API Microsoft Graph |
|-----------------------------------------------------------------------------------------|-----|
| [CreateFolder](/exchange/client-developer/web-service-reference/createfolder-operation) | [Создание папки почты](/graph/api/user-post-mailfolders) |
| [CopyFolder](/exchange/client-developer/web-service-reference/copyfolder-operation)     | [Копирование папки с почтой](/graph/api/mailfolder-copy) |
| [DeleteFolder](/exchange/client-developer/web-service-reference/deletefolder-operation) | [Удаление папки почты](/graph/api/mailfolder-delete) |
| [GetFolder](/exchange/client-developer/web-service-reference/getfolder-operation)       | [Получение папки почты](/graph/api/mailfolder-get) |
| [MoveFolder](/exchange/client-developer/web-service-reference/movefolder-operation)     | [Перемещение папки с почтой](/graph/api/mailfolder-move) |
| [UpdateFolder](/exchange/client-developer/web-service-reference/updatefolder-operation) | [Обновление папки почты](/graph/api/mailfolder-update) |

### <a name="attachments"></a>Вложения

| EWS API                                                                                         | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------|-----|
| [CreateAttachment](/exchange/client-developer/web-service-reference/createattachment-operation) | [Добавление вложения](/graph/api/message-post-attachments) |
| [GetAttachment](/exchange/client-developer/web-service-reference/getattachment-operation)       | [Получение вложения](/graph/api/attachment-get) |
| [DeleteAttachment](/exchange/client-developer/web-service-reference/deleteattachment-operation) | [Удаление вложения](/graph/api/attachment-delete) |

### <a name="rules"></a>Rules

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                         | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------|-----|
| [GetInboxRules](/exchange/client-developer/web-service-reference/getinboxrules-operation)       | [Список правил](/graph/api/mailfolder-list-messagerules) |
| [UpdateInboxRules](/exchange/client-developer/web-service-reference/updateinboxrules-operation) | [Создание правила](/graph/api/mailfolder-post-messagerules)<br/>[Обновление правила](/graph/api/messagerule-update)<br/>[Удаление правила](/graph/api/messagerule-delete) |
<!-- markdownlint-enable MD033 -->

### <a name="mailtips"></a>Подсказки

| EWS API                                                                               | API Microsoft Graph |
|---------------------------------------------------------------------------------------|-----|
| [GetMailTips](/exchange/client-developer/web-service-reference/getmailtips-operation) | [Получение подсказок](/graph/api/user-getmailtips) |

### <a name="out-of-office-oof-settings"></a>Параметры Office (OOF)

| EWS API                                                                                             | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [GetUserOofSettings](/exchange/client-developer/web-service-reference/getuseroofsettings-operation) | [Получение параметров почтового ящика пользователя](/graph/api/user-get-mailboxsettings) |
| [SetUserOofSettings](/exchange/client-developer/web-service-reference/setuseroofsettings-operation) | [Обновление параметров почтового ящика пользователя](/graph/api/user-update-mailboxsettings) |

### <a name="notifications"></a>Уведомления

> [!NOTE]
> Microsoft Graph требуется только подписка для push-уведомлений. Если в настоящее время вы используете [уведомления по запросу EWS](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange), см. раздел ["Получение разностных сообщений"](/graph/api/message-delta).

| EWS API                                                                                                    | API Microsoft Graph |
|------------------------------------------------------------------------------------------------------------|-----|
| [GetEvents](/exchange/client-developer/web-service-reference/getevents-operation)                          | [Получение разностных сообщений](/graph/api/message-delta) |
| [Подписка](/exchange/client-developer/web-service-reference/subscribe-operation) (push-уведомления)     | [Создание подписки](/graph/api/subscription-post-subscriptions) |
| [Отмена подписки](/exchange/client-developer/web-service-reference/unsubscribe-operation) (push-уведомления) | [Удаление подписки](/graph/api/subscription-delete) |

### <a name="synchronization"></a>Синхронизация

| EWS API                                                                                               | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [SyncFolderHierarchy](/exchange/client-developer/web-service-reference/syncfolderhierarchy-operation) | [Получение дельты папки почты](/graph/api/mailfolder-delta) |
| [SyncFolderItems](/exchange/client-developer/web-service-reference/syncfolderitems-operation)         | [Получение разностных сообщений](/graph/api/message-delta) |

## <a name="calendar-apis"></a>API календаря

### <a name="availability"></a>Доступность

| EWS API                                                                                               | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation)<br/>FindAvailableMeetingTimes | [Получение сведений о доступности](/graph/api/calendar-getschedule)|
 

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Представление напоминаний](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Отмена напоминания](/graph/api/event-dismissreminder)<br/>[Откладывание напоминания](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->

### <a name="permissions"></a>Разрешения

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Представление напоминаний](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Отмена напоминания](/graph/api/event-dismissreminder)<br/>[Откладывание напоминания](/graph/api/event-snoozereminder) |
|CreateSharingPermission,GetSharingPermission | [Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании](outlook-share-or-delegate-calendar.md#calendar-owner-get-sharing-or-delegation-information-and-permissions)|
|UpdateSharingPermission | [Получение сведений календаря о получателях общего доступа и делегатах, а также обновление отдельных разрешений](outlook-share-or-delegate-calendar.md#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions)|
|DeleteSharingPermission| [Удаление получателя общего доступа или делегата календаря](outlook-share-or-delegate-calendar.md#delete-a-sharee-or-delegate-of-a-calendar)|
|GetSharingPermissionInfo | [Владелец календаря. Получение свойств общего или делегированного календаря](outlook-share-or-delegate-calendar.md#get-properties-of-a-shared-or-delegated-calendar)|

### <a name="invitations"></a>Приглашения
| EWS API                                                                                                   | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
|ActivateSharingInvitation | [Предоставление общего доступа к календарю или его делегирование в Outlook](/graph/outlook-share-or-delegate-calendar)|
|GetSharingInvitation | [Получатель общего доступа: получение общего календаря или его событий непосредственно из почтового ящика владельца календаря](outlook-get-shared-events-calendars.md#sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox)|
|DeleteSharingInvitation | [Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре](outlook-share-or-delegate-calendar.md#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)|
|CreateSharingInvitation | [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf)|

### <a name="shared-information"></a>Общие сведения
| EWS API                                                                                                   | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| GetCalendarSharedInformation,GetConsumerCalendarSharedInformation | [Список календарей](/graph/api/user-list-calendars) |
## <a name="groups-apis"></a>API групп

| EWS API                                                                                               | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| GetUserUnifiedGroups | [List memberof](/graph/api/user-list-memberof) |
| GetUnifiedGroupsSettings | [groupSetting](/graph/api/resources/groupsetting) |
| GetUnifiedGroupDetails | [Получение группы](/graph/api/group-get) |
| GetUnifiedGroupMembers | [Перечисление участников](/graph/api/group-list-members) |
| GetUnifiedGroupUnseenCount | [Получение группы](/graph/api/group-get) |
| SetUnifiedGroupMembershipState | [Добавление или удаление участника или владельца](/graph/api/resources/group) |
| FindUnifiedGroups | [Список групп](/graph/api/group-list) |
| SetUnifiedGroupUserSubscribeState | [Подписка или отмена подпискиByMail](/graph/api/group-subscribebymail) |
| UpdateUnifiedGroup | [Обновление группы](/graph/api/group-update) |
| CreateUnifiedGroup | [Создание группы](/graph/api/group-post-groups) |
| RemoveUnifiedGroup | [Удаление группы](/graph/api/group-delete) |
| SetUnifiedGroupFavoriteState | [Group addFavorite](/graph/api/group-addfavorite) |
| JoinPrivateUnifiedGroup | [Подписка или отмена подпискиByMail](/graph/api/group-subscribebymail) |
| GetDlMembersForUnifiedGroup | [Перечисление участников группы](/graph/api/group-list-members) |
