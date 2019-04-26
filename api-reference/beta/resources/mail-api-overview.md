---
title: Использование REST API почты Outlook
description: Microsoft Graph позволяет вашему приложению получать авторизованный доступ к данным почты Outlook в личной или корпоративной учетной записи.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a42b1508ab022bfd530b9338dc8049c65f478727
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463798"
---
# <a name="use-the-outlook-mail-rest-api"></a>Использование REST API почты Outlook

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет вашему приложению получать авторизованный доступ к данным почты Outlook в личной или корпоративной учетной записи. Имея [соответствующие делегированные разрешения или разрешения приложения](/graph/permissions-reference), приложение может получать доступ к данным почты вошедшего пользователя или любого пользователя в клиенте. Данные почты могут находиться в облаке на сервере Exchange Online (составной части Office 365) или на локальном сервере Exchange в [гибридном развертывании](/graph/hybrid-rest-support).

## <a name="using-the-mail-rest-api"></a>Использование REST API почты

Запросы API почты выполняются от имени [пользователя](../resources/user.md), который может определяться свойством пользователя **id** (уникальным GUID), адресом электронной почты или псевдонимом `me`, обозначающим вошедшего пользователя.

Сообщения электронной почты представлены ресурсом [message](../resources/message.md) и упорядочены в почтовой папке [mailFolder](../resources/mailfolder.md). Сообщения и почтовые папки определяются свойством **id**, которое можно получить из операций `GET`.

> **Примечание.** Идентификаторы **message** и **mailfolder** не являются уникальными и неизменяемыми в почтовом ящике. Они могут изменяться после копирования, перемещения или отправки.

Сообщения могут быть в формате HTML или текстовом формате.

Вы можете использовать такие известные имена папок, как `Inbox`, `Drafts`, `SentItems` или `DeletedItems`, чтобы указать почтовые папки, которые существуют по умолчанию для всех пользователей. Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).

Например, вы можете получить сообщения из папки Outlook **Отправленные** вошедшего пользователя, не получая идентификатор папки:

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Основные варианты использования

Ресурс **message** предоставляет такие свойства, как **categories**, **conversationId**, **flag** и **importance**, которые соответствуют функциям, доступным в пользовательском интерфейсе, позволяя приложениям автоматизировать работу или интегрироваться со встроенными возможностями Outlook.

В API Microsoft Graph также есть методы и действия, которые поддерживают основные варианты использования сообщений.

| Варианты использования | Ресурсы REST | См. также |
|:----------|:---------------|:---------|
| **Действия, ориентированные на пользователя** | | |
| Создание, чтение, ответ, пересылка, отправка, обновление или удаление сообщений | [message](../resources/message.md) | [Методы ресурса message](../resources/message.md#methods) |
| Предоставление другому пользователю права отправлять сообщения от имени владельца почтового ящика | [message](../resources/message.md) | Задание свойств **from** и **sender** в ресурсе [message](../resources/message.md) |
| Показ более важных сообщений | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [Сортировка почты](../resources/manage-focused-inbox.md) |
| Получение содержимого MIME сообщения или его вложения (предварительная версия) | [message](../resources/message.md) | [Получение содержимого MIME](/graph/outlook-get-mime-message) |
| Добавление, получение или удаление вложений сообщения | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Методы ресурса attachment](../resources/attachment.md#methods) |
| Получение настроек языка и часовых поясов для пользователя | [localeInfo](localeinfo.md), <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md), <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| Получение или обновление автоматического ответа, языкового стандарта, часового пояса или рабочего времени пользователя | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Получение настроек почтового ящика пользователя](../api/user-get-mailboxsettings.md), <br> [Обновление параметров почтового ящика пользователя](../api/user-update-mailboxsettings.md) |
| Получение подсказок об особом состоянии других пользователей, например об отсутствии на месте | [user](../resources/user.md), <br> [mailTips](../resources/mailtips.md) | [Получение подсказок](../api/user-getmailtips.md) |
| Оповещение пользователя при его упоминании в других сообщениях (предварительная версия) | [mention (предварительная версия)](../resources/mention.md) | [Получение сведений об @упоминаниях в сообщении](../api/message-get.md#request-2) |
| Отмена подписки пользователя на список рассылки электронной почты (предварительная версия) | [message (предварительная версия)](../resources/message.md) | [Отмена подписки](../api/message-unsubscribe.md) |
| **Управление почтой и папками** | | |
| Упорядочивание сообщений в иерархии папок почты | [mailFolder](../resources/mailfolder.md)  | [Методы ресурса mailFolder](../resources/mailfolder.md#methods) |
| Классификация сообщений | [outlookCategory (предварительная версия)](../resources/outlookcategory.md) | [Методы ресурса outlookCategory](../resources/outlookcategory.md#methods) |
| Автоматизация действий, например пересылка определенных входящих сообщений, с помощью правил папки "Входящие" | [messageRule (предварительная версия)](../resources/messagerule.md) | [Методы ресурса messageRule](../resources/messagerule.md#methods) |
| Получение заголовков сообщений Интернета для сообщения | [message (предварительная версия)](../resources/message.md) | [Получение свойства **internetMessageHeaders** сообщения](../api/message-get.md#request-4). |
| Поиск и фильтрация сообщений | [message](../resources/message.md) | [Параметры запроса](/graph/query-parameters)  |
| Получение уведомлений об изменениях сообщений в папке | [subscription](../resources/subscription.md) | [Работа с веб-перехватчиками в Microsoft Graph](../resources/webhooks.md) |
| Синхронизация сообщений или иерархии папок почты | [message](../resources/message.md) | [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages) |
| **Разработка приложений** | | |
| Получение пользовательских данных приложения в виде заголовков сообщений Интернета для сообщения | [message](../resources/message.md) | Добавление пользовательских данных в коллекцию **internetMessageHeaders** сообщения. |
| Добавление пользовательских данных приложения в сообщение с помощью расширений | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview) |
| Доступ к пользовательским данным для редко предоставляемых свойств Outlook MAPI | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Общие сведения о расширенных свойствах Outlook](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Дальнейшие действия

API почты открывает новые способы взаимодействия с пользователями:

- [Обзор API почты Outlook](/graph/outlook-mail-concept-overview)
- Узнайте больше о [методах](../resources/message.md#methods), [свойствах](../resources/message.md#properties) и [отношениях](../resources/message.md#relationships) ресурсов [message](../resources/message.md) и [mailFolder](../resources/mailfolder.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
