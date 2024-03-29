---
title: Получайте сообщения Outlook в общую или делегированную папку с помощью почтового API Outlook.
description: Используйте почтовый API Outlook, чтобы делиться почтовыми папками с другими и управлять доступом к папкам. Вы также можете делегировать другому пользователю право действовать от вашего имени.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: d0199c3971823f9efe2149860b516b5d1bf89424
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444308"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Получение сообщений Outlook в общей или делегированной папке

Пользователи Outlook могут делиться почтовыми папками и предоставлять права на чтение, создание, изменение и удаление отдельных папок. Outlook также позволяет клиенту делегировать другому пользователю право действовать от имени клиента и получать доступ к определенным папкам или ко всему его почтовому ящику. В Outlook это называется "делегированием".

Что касается программного кода, то Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок. Эта поддержка также применима к делегированным папкам.

Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие". Если Иван войдет в ваше приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Используйте делегированные разрешения, `Mail.Read.Shared` или `Mail.ReadWrite.Shared`, чтобы они могли считывать и записывать сообщения в общей или делегированной папке. 

Обратите внимание на то, что эти два разрешения не поддерживают [подписку на уведомления об изменениях](webhooks.md) для элементов в общих или делегированных папках. Чтобы настроить подписки на уведомления об изменениях сообщений в общей, делегированной или любой другой почтовой папке пользователя в клиенте, используйте разрешение приложения, `Mail.Read`.

Дополнительные сведения см. в разделе [Разрешения для почты](permissions-reference.md#mail-permissions).

## <a name="get-a-message-in-the-shared-folder"></a>Получение сообщения из общей папки

Так вы можете получить определенное сообщение из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](/graph/api/resources/message), указанный параметром `{id}`, из папки "Входящие" Григория.

## <a name="get-all-messages-in-the-shared-folder"></a>Получение всех сообщений из общей папки

Получение всех сообщений из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](/graph/api/resources/message) из папки "Входящие" Григория.

## <a name="get-the-shared-folder"></a>Получение общей папки

Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](/graph/api/resources/mailfolder), представляющий папку "Входящие" Григория.

Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.

Если Григорий не поделился своей папкой "Входящие" с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Григория в этих операциях GET будет возвращена ошибка. 


## <a name="next-steps"></a>Дальнейшие действия

- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование почтового API](/graph/api/resources/mail-api-overview) и [вариантов его использования](/graph/api/resources/mail-api-overview#common-use-cases) в Microsoft Graph версии 1.0
