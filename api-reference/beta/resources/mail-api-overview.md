---
title: Использование интерфейса API REST почты Outlook
description: Microsoft Graph позволяет получить авторизованные доступ к данным почты Outlook пользователя в личный или организации учетной записи приложения.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 96d2924846adebaae0ed435aed7dcf65934db81a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933017"
---
# <a name="use-the-outlook-mail-rest-api"></a>Использование интерфейса API REST почты Outlook

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Microsoft Graph позволяет вашему приложению получать авторизованный доступ к данным почты Outlook в личной или корпоративной учетной записи. Имея [соответствующие делегированные разрешения или разрешения приложения](/graph/permissions-reference), приложение может получать доступ к данным почты вошедшего пользователя или любого пользователя в клиенте. Данные почты могут находиться в облаке на сервере Exchange Online (составной части Office 365) или на локальном сервере Exchange в [гибридном развертывании](/graph/hybrid-rest-support).

## <a name="using-the-mail-rest-api"></a>Использование REST API почты

Запросы API почты выполняются от имени [пользователя](../resources/user.md), который может определяться свойством пользователя **id** (уникальным GUID), адресом электронной почты или псевдонимом `me`, обозначающим вошедшего пользователя.

Сообщения электронной почты представлены ресурсом [message](../resources/message.md) и упорядочены в почтовой папке [mailFolder](../resources/mailfolder.md). Сообщения и почтовые папки определяются свойством **id**, которое можно получить из операций `GET`.

> **Примечание.** Идентификаторы **message** и **mailfolder** не являются уникальными и неизменяемыми в почтовом ящике. Они могут изменяться после копирования, перемещения или отправки.

Сообщения могут быть в формате HTML или текстовом формате.

Можно использовать имена известных папок, таких как `Inbox`, `Drafts`, `SentItems`, или `DeletedItems` для идентификации определенных почтовых папок, существующих по умолчанию для всех пользователей. Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).

Например можно получить сообщения в папке Outlook **Отправленные** пользователь выполнил вход без получения идентификатор папки:

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
| Предоставление другому пользователю права отправлять сообщения от имени владельца почтового ящика | [message](../resources/message.md) | Установка свойств **из** и **отправителей** в [сообщение](../resources/message.md) |
| Показ более важных сообщений | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [Сортировка почты](../resources/manage-focused-inbox.md) |
| Добавление, получение или удаление вложений сообщения | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Методы ресурса attachment](../resources/attachment.md#methods) |
| Выбрать язык и часовой пояс для пользователя | [localeInfo](localeinfo.md), <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md) <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| Получение или обновление автоматического ответа, языкового стандарта, часового пояса или рабочего времени пользователя | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Получение настроек почтового ящика пользователя](../api/user-get-mailboxsettings.md), <br> [Обновление параметров почтового ящика пользователя](../api/user-update-mailboxsettings.md) |
| Получите подсказки специальные состояние других получателей, например, документов office | [пользователь](../resources/user.md) <br> [почтовые подсказки](../resources/mailtips.md) | [Получите подсказки](../api/user-getmailtips.md) |
| Оповещение пользователя, если упомянутые в другие сообщения (Предварительная версия) | [Упоминание (Предварительная версия)](../resources/mention.md) | [Подробные сведения о @ упоминания в сообщение](../api/message-get.md#request-2) |
| Отменить подписку пользователя в список рассылки по электронной почте (Предварительная версия) | [сообщение (Предварительная версия)](../resources/message.md) | [Unsubscribe](../api/message-unsubscribe.md) |
| **Управление почтой и папками** | | |
| Упорядочивание сообщений в иерархии папок почты | [mailFolder](../resources/mailfolder.md)  | [Методы ресурса mailFolder](../resources/mailfolder.md#methods) |
| Классификации сообщений | [outlookCategory (Предварительная версия)](../resources/outlookcategory.md) | [Методы outlookCategory](../resources/outlookcategory.md#methods) |
| Использование правил папки "Входящие" для автоматизации действий, таких как переадресация определенных входящих сообщений | [messageRule (Предварительная версия)](../resources/messagerule.md) | [Методы messageRule](../resources/messagerule.md#methods) |
| Получение заголовков сообщений Интернета сообщения | [сообщение (Предварительная версия)](../resources/message.md) | [Получите свойство **internetMessageHeaders** сообщения](../api/message-get.md#request-4). |
| Поиск и фильтрация сообщений | [message](../resources/message.md) | [Параметры запроса](/graph/query-parameters)  |
| Получение уведомлений об изменениях сообщений в папке | [subscription](../resources/subscription.md) | [Работа с веб-перехватчиками в Microsoft Graph](../resources/webhooks.md) |
| Синхронизация сообщений или иерархии папок почты | [message](../resources/message.md) | [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages) |
| **Разработка приложений** | | |
| Добавление данных пользовательское приложение как заголовки сообщений Интернета сообщения | [message](../resources/message.md) | Добавление пользовательских данных в коллекцию **internetMessageHeaders** сообщения. |
| Добавление пользовательских данных приложения в сообщение с помощью расширений | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview) |
| Доступ к пользовательским данным для редко предоставляемых свойств Outlook MAPI | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Общие сведения о расширенных свойствах Outlook](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Дальнейшие действия

API почты открывает новые способы взаимодействия с пользователями:

- [Обзор API почты Outlook](/graph/outlook-mail-concept-overview)
- Узнайте больше о [методах](../resources/message.md#methods), [свойствах](../resources/message.md#properties) и [отношениях](../resources/message.md#relationships) ресурсов [message](../resources/message.md) и [mailFolder](../resources/mailfolder.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
