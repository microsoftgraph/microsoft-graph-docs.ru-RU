---
title: Получение контактов Outlook из общей папки
description: " это также "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092608"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="01da4-103">Получение контактов Outlook из общей папки</span><span class="sxs-lookup"><span data-stu-id="01da4-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="01da4-104">Пользователи Outlook могут делиться папками и предоставлять права на чтение, создание, изменение или удаление отдельных папок контактов.</span><span class="sxs-lookup"><span data-stu-id="01da4-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="01da4-105">Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента и получать доступ к определенным папкам или ко всему почтовому ящику клиента. В Outlook это также называется "делегированием".</span><span class="sxs-lookup"><span data-stu-id="01da4-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="01da4-106">Что касается программного кода, Microsoft Graph поддерживает получение контактов из папок контактов, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="01da4-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="01da4-107">Поддержка также относится к папкам в делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="01da4-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="01da4-108">Допустим, Григорий поделился с Иваном пользовательской папкой контактов и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="01da4-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="01da4-109">Если Иван войдет в приложение и предоставит делегированные разрешения (Contacts.Read.Shared or Contacts.ReadWrite.Shared), то приложение сможет получать доступ к пользовательской папке контактов Григория и контактам из нее, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="01da4-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="01da4-110">Получение контакта из общей папки</span><span class="sxs-lookup"><span data-stu-id="01da4-110">Get a message in the shared folder</span></span>

<span data-ttu-id="01da4-111">Можно получить определенный контакт из пользовательской папки контактов, которой Григорий поделился с Иваном:</span><span class="sxs-lookup"><span data-stu-id="01da4-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="01da4-112">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0), указанный параметром `{id}`, из общей папки контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="01da4-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="01da4-113">Получение всех контактов из общей папки</span><span class="sxs-lookup"><span data-stu-id="01da4-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="01da4-114">Получение всех контактов из общей папки контактов Григория:</span><span class="sxs-lookup"><span data-stu-id="01da4-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="01da4-115">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0) из общей папки контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="01da4-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="01da4-116">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="01da4-116">Get the shared folder</span></span>

<span data-ttu-id="01da4-117">Получение папки контактов, которой Григорий поделился с Иваном.</span><span class="sxs-lookup"><span data-stu-id="01da4-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="01da4-118">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0), представляющий общую папку контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="01da4-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="01da4-119">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану весь свой почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="01da4-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="01da4-120">Если Григорий не поделился своей папкой контактов с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Ивана в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="01da4-120">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="01da4-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="01da4-121">Next steps</span></span>

<span data-ttu-id="01da4-122">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="01da4-122">Find out more about:</span></span>

- [<span data-ttu-id="01da4-123">Зачем выполнять интеграцию с личными контактами Outlook?</span><span class="sxs-lookup"><span data-stu-id="01da4-123">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="01da4-124">[API контактов](/graph/api/resources/contact?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="01da4-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>