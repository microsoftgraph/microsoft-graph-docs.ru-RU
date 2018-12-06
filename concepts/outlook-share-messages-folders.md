---
title: Получение сообщений Outlook в общей или делегированной папке
description: 'В этих темах также есть похожие разделы: список событий, получение события, получение календаря, список контактов, получение контакта, получение папки контактов.'
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092658"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="7e61a-103">Получение сообщений Outlook в общей или делегированной папке</span><span class="sxs-lookup"><span data-stu-id="7e61a-103">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="7e61a-104">Пользователи Outlook могут делиться почтовыми папками и предоставлять права на чтение, создание, изменение и удаление отдельных папок.</span><span class="sxs-lookup"><span data-stu-id="7e61a-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="7e61a-105">Outlook также позволяет клиенту делегировать другому пользователю право действовать от имени клиента и получать доступ к определенным папкам или ко всему его почтовому ящику. В Outlook это называется "делегированием".</span><span class="sxs-lookup"><span data-stu-id="7e61a-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="7e61a-106">Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="7e61a-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="7e61a-107">Поддержка также применима к делегированным папкам.</span><span class="sxs-lookup"><span data-stu-id="7e61a-107">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="7e61a-108">Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7e61a-108">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="7e61a-109">Если Иван войдет в приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="7e61a-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="7e61a-110">Получение сообщения из общей папки</span><span class="sxs-lookup"><span data-stu-id="7e61a-110">Get a message in the shared folder</span></span>

<span data-ttu-id="7e61a-111">Так вы можете получить определенное сообщение из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="7e61a-111">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="7e61a-112">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](/graph/api/resources/message?view=graph-rest-1.0), указанный параметром `{id}`, из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="7e61a-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="7e61a-113">Получение всех сообщений из общей папки</span><span class="sxs-lookup"><span data-stu-id="7e61a-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="7e61a-114">Получение всех сообщений из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="7e61a-114">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="7e61a-115">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](/graph/api/resources/message?view=graph-rest-1.0) из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="7e61a-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="7e61a-116">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="7e61a-116">Get the shared folder</span></span>

<span data-ttu-id="7e61a-117">Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.</span><span class="sxs-lookup"><span data-stu-id="7e61a-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="7e61a-118">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0), представляющий папку "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="7e61a-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="7e61a-119">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="7e61a-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="7e61a-120">Если Григорий не поделился своей папкой "Входящие" с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Григория в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="7e61a-120">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="7e61a-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="7e61a-121">Next steps</span></span>

<span data-ttu-id="7e61a-122">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="7e61a-122">Find out more about:</span></span>

- [<span data-ttu-id="7e61a-123">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="7e61a-123">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="7e61a-124">[Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [варианты использования](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="7e61a-124">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>