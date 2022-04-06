---
title: Exchange веб-служб (EWS) для сопоставлений API Graph Microsoft
description: В этой статье перечислены API microsoft Graph, которые Exchange API веб-служб (EWS).
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 89aa884baf0ae5d2a67d31f3e28d4c818be2c9af
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516578"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange веб-служб (EWS) для сопоставлений API Graph Microsoft

В этой статье перечислены API microsoft Graph, которые Exchange API веб-служб (EWS).

## <a name="utility-apis"></a>API-утилиты

| EWS API                                                                                             | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [Перевод Exchange ID](/graph/api/user-translateexchangeids) |
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

### <a name="attachments"></a>Attachments

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
> Microsoft Graph требуется подписка только для push-уведомлений. Если вы в настоящее время используете уведомления о вытягиве [EWS](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange), см. [в сообщении Get messages delta](/graph/api/message-delta).

| EWS API                                                                                                    | API Microsoft Graph |
|------------------------------------------------------------------------------------------------------------|-----|
| [GetEvents](/exchange/client-developer/web-service-reference/getevents-operation)                          | [Дельта сообщений](/graph/api/message-delta) |
| [Подписка](/exchange/client-developer/web-service-reference/subscribe-operation) (push-уведомления)     | [Создание подписки](/graph/api/subscription-post-subscriptions) |
| [Отписать](/exchange/client-developer/web-service-reference/unsubscribe-operation) (push-уведомления) | [Удаление подписки](/graph/api/subscription-delete) |

### <a name="synchronization"></a>Синхронизация

| EWS API                                                                                               | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [SyncFolderHierarchy](/exchange/client-developer/web-service-reference/syncfolderhierarchy-operation) | [Получение дельты папки почты](/graph/api/mailfolder-delta) |
| [SyncFolderItems](/exchange/client-developer/web-service-reference/syncfolderitems-operation)         | [Дельта сообщений](/graph/api/message-delta) |

## <a name="calendar-apis"></a>API календаря

### <a name="availability"></a>Доступность

| EWS API                                                                                               | API Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation) | [Получение сведений о доступности](/graph/api/calendar-getschedule) |

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Представление напоминаний](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Отмена напоминания](/graph/api/event-dismissreminder)<br/>[Откладывание напоминания](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->
