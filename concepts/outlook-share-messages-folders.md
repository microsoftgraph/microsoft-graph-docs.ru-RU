---
title: Получение сообщений Outlook в общей или делегированной папке
description: 'В этих темах также есть похожие разделы: список событий, получение события, получение календаря, список контактов, получение контакта, получение папки контактов.'
author: angelgolfer-ms
ms.openlocfilehash: d90fa5d37fd7a07e4069bd5bcc0eb46f0cae29a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320113"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Получение сообщений Outlook в общей или делегированной папке

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Пользователи Outlook могут делиться почтовыми папками и предоставлять права на чтение, создание, изменение и удаление отдельных папок. Outlook также позволяет клиенту делегировать другому пользователю право действовать от имени клиента и получать доступ к определенным папкам или ко всему его почтовому ящику. В Outlook это называется "делегированием".

Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок. Поддержка также применима к делегированным папкам.

Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие". Если Иван войдет в приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.

## <a name="get-a-message-in-the-shared-folder"></a>Получение сообщения из общей папки

Так вы можете получить определенное сообщение из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](/graph/api/resources/message?view=graph-rest-1.0), указанный параметром `{id}`, из папки "Входящие" Григория.

## <a name="get-all-messages-in-the-shared-folder"></a>Получение всех сообщений из общей папки

Получение всех сообщений из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](/graph/api/resources/message?view=graph-rest-1.0) из папки "Входящие" Григория.

## <a name="get-the-shared-folder"></a>Получение общей папки

Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0), представляющий папку "Входящие" Григория.

Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.

Если Григорий не поделился своей папкой "Входящие" с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Григория в этих операциях GET будет возвращена ошибка. 


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [варианты использования](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) в Microsoft Graph 1.0.