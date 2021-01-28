---
title: Получение сообщений Outlook в общей или делегированной папке
description: Пользователи Outlook могут делиться почтовыми папками и предоставлять права на чтение, создание, изменение и удаление отдельных папок. Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6de4ee7ca1ed179bc538bb7aa1f2a3dacb8adb80
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013445"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="cc531-104">Получение сообщений Outlook в общей или делегированной папке</span><span class="sxs-lookup"><span data-stu-id="cc531-104">Get Outlook messages in a shared or delegated folder</span></span>

<span data-ttu-id="cc531-105">Пользователи Outlook могут делиться почтовыми папками и предоставлять права на чтение, создание, изменение и удаление отдельных папок.</span><span class="sxs-lookup"><span data-stu-id="cc531-105">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="cc531-106">Outlook также позволяет клиенту делегировать другому пользователю право действовать от имени клиента и получать доступ к определенным папкам или ко всему его почтовому ящику. В Outlook это называется "делегированием".</span><span class="sxs-lookup"><span data-stu-id="cc531-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="cc531-107">Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="cc531-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="cc531-108">Поддержка также применима к делегированным папкам.</span><span class="sxs-lookup"><span data-stu-id="cc531-108">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="cc531-109">Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="cc531-109">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="cc531-110">Если Иван войдет в приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="cc531-110">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="cc531-111">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cc531-111">Microsoft Graph permissions</span></span>

<span data-ttu-id="cc531-112">Используйте делегированные разрешения, `Mail.Read.Shared` или `Mail.ReadWrite.Shared`, чтобы они могли считывать и записывать сообщения в общей или делегированной папке.</span><span class="sxs-lookup"><span data-stu-id="cc531-112">Use the delegated permissions, `Mail.Read.Shared` or `Mail.ReadWrite.Shared`, to respectively read or write messages in a shared or delegated folder.</span></span> 

<span data-ttu-id="cc531-113">Обратите внимание на то, что эти два разрешения не поддерживают [подписку на уведомления об изменениях](webhooks.md) для элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="cc531-113">Note that those two permissions do not support [subscribing to change notifications](webhooks.md) on items in shared or delegated folders.</span></span> <span data-ttu-id="cc531-114">Чтобы настроить подписки на уведомления об изменениях сообщений в общей, делегированной или любой другой почтовой папке пользователя в клиенте, используйте разрешение приложения, `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="cc531-114">To set up change notification subscriptions on messages in a shared, delegated, or any other user's mail folder in the tenant, use the application permission, `Mail.Read`.</span></span>

<span data-ttu-id="cc531-115">Дополнительные сведения см. в разделе [Разрешения для почты](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="cc531-115">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="cc531-116">Получение сообщения из общей папки</span><span class="sxs-lookup"><span data-stu-id="cc531-116">Get a message in the shared folder</span></span>

<span data-ttu-id="cc531-117">Так вы можете получить определенное сообщение из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="cc531-117">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="cc531-118">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](/graph/api/resources/message), указанный параметром `{id}`, из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="cc531-118">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="cc531-119">Получение всех сообщений из общей папки</span><span class="sxs-lookup"><span data-stu-id="cc531-119">Get all messages in the shared folder</span></span>

<span data-ttu-id="cc531-120">Получение всех сообщений из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="cc531-120">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="cc531-121">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](/graph/api/resources/message) из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="cc531-121">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="cc531-122">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="cc531-122">Get the shared folder</span></span>

<span data-ttu-id="cc531-123">Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.</span><span class="sxs-lookup"><span data-stu-id="cc531-123">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="cc531-124">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](/graph/api/resources/mailfolder), представляющий папку "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="cc531-124">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="cc531-125">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cc531-125">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="cc531-126">Если Григорий не поделился своей папкой "Входящие" с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Григория в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="cc531-126">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="cc531-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="cc531-127">Next steps</span></span>

<span data-ttu-id="cc531-128">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="cc531-128">Find out more about:</span></span>

- [<span data-ttu-id="cc531-129">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="cc531-129">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="cc531-130">[Использование API почты](/graph/api/resources/mail-api-overview) и [варианты использования](/graph/api/resources/mail-api-overview#common-use-cases) в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="cc531-130">[Using the mail API](/graph/api/resources/mail-api-overview) and its [use cases](/graph/api/resources/mail-api-overview#common-use-cases) in Microsoft Graph v1.0.</span></span>
