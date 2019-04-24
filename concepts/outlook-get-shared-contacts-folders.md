---
title: Получение контактов Outlook из общей папки
description: Пользователи Outlook могут делиться папками и предоставлять права на чтение, создание, изменение или удаление отдельных папок контактов. Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86533a28c0af206458b63fd19f32f01c5b68710b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585442"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="97a66-104">Получение контактов Outlook из общей папки</span><span class="sxs-lookup"><span data-stu-id="97a66-104">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="97a66-105">Пользователи Outlook могут делиться папками и предоставлять права на чтение, создание, изменение или удаление отдельных папок контактов.</span><span class="sxs-lookup"><span data-stu-id="97a66-105">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="97a66-106">Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента и получать доступ к определенным папкам или ко всему почтовому ящику клиента. В Outlook это также называется "делегированием".</span><span class="sxs-lookup"><span data-stu-id="97a66-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="97a66-107">Что касается программного кода, Microsoft Graph поддерживает получение контактов из папок контактов, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="97a66-107">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="97a66-108">Поддержка также относится к папкам в делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="97a66-108">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="97a66-109">Допустим, Григорий поделился с Иваном пользовательской папкой контактов и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="97a66-109">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="97a66-110">Если Иван войдет в приложение и предоставит делегированные разрешения (Contacts.Read.Shared или Contacts.ReadWrite.Shared), то приложение сможет получать доступ к пользовательской папке контактов Григория и контактам из нее, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="97a66-110">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

> <span data-ttu-id="97a66-111">**Примечание.** Разрешения совместного доступа (Contacts.Read.Shared или Contacts.ReadWrite.Shared) позволяют читать или записывать контакты в общей или делегированной папке.</span><span class="sxs-lookup"><span data-stu-id="97a66-111">**Note** The sharing permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared) allow you to read or write contacts in a shared or delegated folder.</span></span> <span data-ttu-id="97a66-112">Они не поддерживают [подписку на уведомления об изменениях](webhooks.md) элементов в таких папках.</span><span class="sxs-lookup"><span data-stu-id="97a66-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="97a66-113">Чтобы настроить подписки на уведомления об изменениях контактов в общей, делегированной или любой другой папке контактов пользователя в клиенте, используйте разрешение приложения Contacts.Read.</span><span class="sxs-lookup"><span data-stu-id="97a66-113">To set up change notification subscriptions on contacts in a shared, delegated, or any other user's contact folder in the tenant, use the application permission, Contacts.Read.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="97a66-114">Получение контакта из общей папки</span><span class="sxs-lookup"><span data-stu-id="97a66-114">Get a contact in the shared folder</span></span>

<span data-ttu-id="97a66-115">Можно получить определенный контакт из пользовательской папки контактов, которой Григорий поделился с Иваном:</span><span class="sxs-lookup"><span data-stu-id="97a66-115">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="97a66-116">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0), указанный параметром `{id}`, из общей папки контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="97a66-116">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="97a66-117">Получение всех контактов из общей папки</span><span class="sxs-lookup"><span data-stu-id="97a66-117">Get all contacts in the shared folder</span></span>

<span data-ttu-id="97a66-118">Получение всех контактов из общей папки контактов Григория:</span><span class="sxs-lookup"><span data-stu-id="97a66-118">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="97a66-119">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0) из общей папки контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="97a66-119">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="97a66-120">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="97a66-120">Get the shared folder</span></span>

<span data-ttu-id="97a66-121">Получение папки контактов, которой Григорий поделился с Иваном.</span><span class="sxs-lookup"><span data-stu-id="97a66-121">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="97a66-122">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0), представляющий общую папку контактов Григория.</span><span class="sxs-lookup"><span data-stu-id="97a66-122">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="97a66-123">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану весь свой почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="97a66-123">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="97a66-124">Если Григорий не поделился своей папкой контактов с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Ивана в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="97a66-124">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="97a66-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="97a66-125">Next steps</span></span>

<span data-ttu-id="97a66-126">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="97a66-126">Find out more about:</span></span>

- [<span data-ttu-id="97a66-127">Зачем выполнять интеграцию с личными контактами Outlook?</span><span class="sxs-lookup"><span data-stu-id="97a66-127">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="97a66-128">[API контактов](/graph/api/resources/contact?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="97a66-128">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
