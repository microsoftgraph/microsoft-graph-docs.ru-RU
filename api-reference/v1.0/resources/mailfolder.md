---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0de32560e154eaa732e596040525025ad0676926
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448020"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="7dda3-104">Тип ресурса mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-104">mailFolder resource type</span></span>

<span data-ttu-id="7dda3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dda3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7dda3-106">Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики".</span><span class="sxs-lookup"><span data-stu-id="7dda3-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="7dda3-107">Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="7dda3-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="7dda3-108">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="7dda3-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="7dda3-109">**Известные имена папок**</span><span class="sxs-lookup"><span data-stu-id="7dda3-109">**Well-known folder names**</span></span>

<span data-ttu-id="7dda3-110">Outlook создает определенные папки для пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7dda3-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="7dda3-111">Для удобства вместо значения **id** для доступа к папкам можно использовать известные имена папок из таблицы ниже.</span><span class="sxs-lookup"><span data-stu-id="7dda3-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="7dda3-112">Например, вы можете получить папку черновиков, использовав ее известное имя со следующим запросом.</span><span class="sxs-lookup"><span data-stu-id="7dda3-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="7dda3-113">Известные имена поддерживаются вне зависимости от языкового стандарта почтового ящика пользователя, поэтому указанный выше запрос всегда возвращает папку черновиков пользователя, независимо от ее имени.</span><span class="sxs-lookup"><span data-stu-id="7dda3-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="7dda3-114">Известное имя папки</span><span class="sxs-lookup"><span data-stu-id="7dda3-114">Well-known folder name</span></span> | <span data-ttu-id="7dda3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda3-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="7dda3-116">archive</span><span class="sxs-lookup"><span data-stu-id="7dda3-116">archive</span></span> | <span data-ttu-id="7dda3-117">Архивная папка, в которую отправляются сообщения при использовании функции архивации одним щелчком в клиентах Outlook, поддерживающих ее.</span><span class="sxs-lookup"><span data-stu-id="7dda3-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="7dda3-118">**Примечание.** Она отличается от функции архивного почтового ящика Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7dda3-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="7dda3-119">clutter</span><span class="sxs-lookup"><span data-stu-id="7dda3-119">clutter</span></span> | <span data-ttu-id="7dda3-120">Папка "Несрочные", в которую перемещаются сообщения низкой важности при использовании функции "Несрочные".</span><span class="sxs-lookup"><span data-stu-id="7dda3-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="7dda3-121">conflicts</span><span class="sxs-lookup"><span data-stu-id="7dda3-121">conflicts</span></span> | <span data-ttu-id="7dda3-122">Папка, содержащая конфликтующие элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7dda3-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="7dda3-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="7dda3-123">conversationhistory</span></span> | <span data-ttu-id="7dda3-124">Папка, в которой Skype сохраняет беседы при обмене мгновенными сообщениями (если Skype настроен для этого).</span><span class="sxs-lookup"><span data-stu-id="7dda3-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="7dda3-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="7dda3-125">deleteditems</span></span> | <span data-ttu-id="7dda3-126">Папка, в которую перемещаются элементы при их удалении.</span><span class="sxs-lookup"><span data-stu-id="7dda3-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="7dda3-127">drafts</span><span class="sxs-lookup"><span data-stu-id="7dda3-127">drafts</span></span> | <span data-ttu-id="7dda3-128">Папка, содержащая неотправленные сообщения.</span><span class="sxs-lookup"><span data-stu-id="7dda3-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="7dda3-129">inbox</span><span class="sxs-lookup"><span data-stu-id="7dda3-129">inbox</span></span> | <span data-ttu-id="7dda3-130">Папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7dda3-130">The inbox folder.</span></span> |
| <span data-ttu-id="7dda3-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="7dda3-131">junkemail</span></span> | <span data-ttu-id="7dda3-132">Папка нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="7dda3-132">The junk email folder.</span></span> |
| <span data-ttu-id="7dda3-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="7dda3-133">localfailures</span></span> | <span data-ttu-id="7dda3-134">Папка, содержащая элементы, существующие в локальном клиенте, но которые нельзя отправить на сервер.</span><span class="sxs-lookup"><span data-stu-id="7dda3-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="7dda3-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="7dda3-135">msgfolderroot</span></span> | <span data-ttu-id="7dda3-136">Папка "Корневой уровень хранилища".</span><span class="sxs-lookup"><span data-stu-id="7dda3-136">The "Top of Information Store" folder.</span></span> <span data-ttu-id="7dda3-137">Эта папка является родительской для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7dda3-137">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="7dda3-138">outbox</span><span class="sxs-lookup"><span data-stu-id="7dda3-138">outbox</span></span> | <span data-ttu-id="7dda3-139">Папка "Исходящие".</span><span class="sxs-lookup"><span data-stu-id="7dda3-139">The outbox folder.</span></span> |
| <span data-ttu-id="7dda3-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="7dda3-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="7dda3-141">Папка, содержащая обратимо удаленные элементы: удаленные из папки "Удаленные" или путем нажатия клавиш SHIFT+DELETE в Outlook.</span><span class="sxs-lookup"><span data-stu-id="7dda3-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="7dda3-142">Эта папка не отображается в почтовых клиентах Outlook, но пользователи могут взаимодействовать с ней с помощью функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="7dda3-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="7dda3-143">scheduled</span><span class="sxs-lookup"><span data-stu-id="7dda3-143">scheduled</span></span> | <span data-ttu-id="7dda3-144">Папка, содержащая сообщения, запланированные для повторного отображения в папке "Входящие" с помощью функции "Расписание" в Outlook для iOS.</span><span class="sxs-lookup"><span data-stu-id="7dda3-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="7dda3-145">searchfolders</span><span class="sxs-lookup"><span data-stu-id="7dda3-145">searchfolders</span></span> | <span data-ttu-id="7dda3-146">Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dda3-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="7dda3-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="7dda3-147">sentitems</span></span> | <span data-ttu-id="7dda3-148">Папка "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="7dda3-148">The sent items folder.</span></span> |
| <span data-ttu-id="7dda3-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="7dda3-149">serverfailures</span></span> | <span data-ttu-id="7dda3-150">Папка, содержащая элементы, существующие на сервере, но которые нельзя синхронизировать с локальным клиентом.</span><span class="sxs-lookup"><span data-stu-id="7dda3-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="7dda3-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="7dda3-151">syncissues</span></span> | <span data-ttu-id="7dda3-152">Папка, содержащая журналы синхронизации, созданные в Outlook.</span><span class="sxs-lookup"><span data-stu-id="7dda3-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="7dda3-153">Методы</span><span class="sxs-lookup"><span data-stu-id="7dda3-153">Methods</span></span>

| <span data-ttu-id="7dda3-154">Метод</span><span class="sxs-lookup"><span data-stu-id="7dda3-154">Method</span></span> | <span data-ttu-id="7dda3-155">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7dda3-155">Return Type</span></span> | <span data-ttu-id="7dda3-156">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda3-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="7dda3-157">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-157">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="7dda3-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-158">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="7dda3-159">Чтение свойств и связей объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-159">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="7dda3-160">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-160">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="7dda3-161">MailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-161">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="7dda3-162">Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.</span><span class="sxs-lookup"><span data-stu-id="7dda3-162">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="7dda3-163">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-163">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="7dda3-164">Коллекция [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-164">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="7dda3-p107">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="7dda3-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="7dda3-167">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="7dda3-167">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="7dda3-168">Message</span><span class="sxs-lookup"><span data-stu-id="7dda3-168">Message</span></span>](message.md)| <span data-ttu-id="7dda3-169">Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="7dda3-169">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="7dda3-170">Вывод списка сообщений</span><span class="sxs-lookup"><span data-stu-id="7dda3-170">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="7dda3-171">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-171">[Message](message.md) collection</span></span>| <span data-ttu-id="7dda3-172">Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7dda3-172">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="7dda3-173">Обновление</span><span class="sxs-lookup"><span data-stu-id="7dda3-173">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="7dda3-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-174">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="7dda3-175">Обновление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-175">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="7dda3-176">Удаление</span><span class="sxs-lookup"><span data-stu-id="7dda3-176">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="7dda3-177">Нет</span><span class="sxs-lookup"><span data-stu-id="7dda3-177">None</span></span> |<span data-ttu-id="7dda3-178">Удаление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-178">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="7dda3-179">copy</span><span class="sxs-lookup"><span data-stu-id="7dda3-179">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="7dda3-180">MailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-180">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="7dda3-181">Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-181">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="7dda3-182">delta</span><span class="sxs-lookup"><span data-stu-id="7dda3-182">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="7dda3-183">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-183">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="7dda3-184">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="7dda3-184">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="7dda3-185">move</span><span class="sxs-lookup"><span data-stu-id="7dda3-185">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="7dda3-186">MailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-186">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="7dda3-187">Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-187">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="7dda3-188">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="7dda3-188">**Extended properties**</span></span>| | |
|[<span data-ttu-id="7dda3-189">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="7dda3-189">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="7dda3-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-190">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="7dda3-191">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-191">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="7dda3-192">Получение элемента mailFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="7dda3-192">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7dda3-193">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-193">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="7dda3-194">Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7dda3-194">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="7dda3-195">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="7dda3-195">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="7dda3-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-196">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="7dda3-197">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-197">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="7dda3-198">Получение элемента mailFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="7dda3-198">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7dda3-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7dda3-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="7dda3-200">Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="7dda3-200">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="7dda3-201">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dda3-201">Properties</span></span>

| <span data-ttu-id="7dda3-202">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dda3-202">Property</span></span> | <span data-ttu-id="7dda3-203">Тип</span><span class="sxs-lookup"><span data-stu-id="7dda3-203">Type</span></span> | <span data-ttu-id="7dda3-204">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda3-204">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="7dda3-205">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="7dda3-205">childFolderCount</span></span>|<span data-ttu-id="7dda3-206">Int32</span><span class="sxs-lookup"><span data-stu-id="7dda3-206">Int32</span></span>|<span data-ttu-id="7dda3-207">Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-207">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="7dda3-208">displayName</span><span class="sxs-lookup"><span data-stu-id="7dda3-208">displayName</span></span>|<span data-ttu-id="7dda3-209">Строка</span><span class="sxs-lookup"><span data-stu-id="7dda3-209">String</span></span>|<span data-ttu-id="7dda3-210">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-210">The mailFolder's display name.</span></span>|
|<span data-ttu-id="7dda3-211">id</span><span class="sxs-lookup"><span data-stu-id="7dda3-211">id</span></span>|<span data-ttu-id="7dda3-212">Строка</span><span class="sxs-lookup"><span data-stu-id="7dda3-212">String</span></span>|<span data-ttu-id="7dda3-213">Уникальный идентификатор элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-213">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="7dda3-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="7dda3-214">parentFolderId</span></span>|<span data-ttu-id="7dda3-215">Строка</span><span class="sxs-lookup"><span data-stu-id="7dda3-215">String</span></span>|<span data-ttu-id="7dda3-216">Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-216">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="7dda3-217">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="7dda3-217">totalItemCount</span></span>|<span data-ttu-id="7dda3-218">Int32</span><span class="sxs-lookup"><span data-stu-id="7dda3-218">Int32</span></span>|<span data-ttu-id="7dda3-219">Количество элементов в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-219">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="7dda3-220">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="7dda3-220">unreadItemCount</span></span>|<span data-ttu-id="7dda3-221">Int32</span><span class="sxs-lookup"><span data-stu-id="7dda3-221">Int32</span></span>|<span data-ttu-id="7dda3-222">Количество элементов, помеченных как непрочитанные, в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-222">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="7dda3-223">**Эффективный доступ к сведениям о количестве элементов**</span><span class="sxs-lookup"><span data-stu-id="7dda3-223">**Access item counts efficiently**</span></span>

<span data-ttu-id="7dda3-224">Используя такие свойства папки, как `TotalItemCount` и `UnreadItemCount`, можно удобно вычислять количество прочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="7dda3-224">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="7dda3-225">Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.</span><span class="sxs-lookup"><span data-stu-id="7dda3-225">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="7dda3-226">Папки почты в Outlook могут содержать элементы нескольких типов, например, папка "Входящие" может содержать элементы приглашений на собрания, не связанные с почтовыми элементами.</span><span class="sxs-lookup"><span data-stu-id="7dda3-226">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="7dda3-227">Свойства `TotalItemCount` и `UnreadItemCount` включают элементы из папки почты вне зависимости от их типов.</span><span class="sxs-lookup"><span data-stu-id="7dda3-227">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="7dda3-228">Отношения</span><span class="sxs-lookup"><span data-stu-id="7dda3-228">Relationships</span></span>

| <span data-ttu-id="7dda3-229">Связь</span><span class="sxs-lookup"><span data-stu-id="7dda3-229">Relationship</span></span> | <span data-ttu-id="7dda3-230">Тип</span><span class="sxs-lookup"><span data-stu-id="7dda3-230">Type</span></span> | <span data-ttu-id="7dda3-231">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda3-231">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="7dda3-232">childFolders</span><span class="sxs-lookup"><span data-stu-id="7dda3-232">childFolders</span></span>|<span data-ttu-id="7dda3-233">Коллекция объектов [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-233">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="7dda3-234">Коллекция дочерних папок в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-234">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="7dda3-235">messageRules</span><span class="sxs-lookup"><span data-stu-id="7dda3-235">messageRules</span></span> | <span data-ttu-id="7dda3-236">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-236">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="7dda3-237">Коллекция правил, которые применяются к папке пользователя "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7dda3-237">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="7dda3-238">messages</span><span class="sxs-lookup"><span data-stu-id="7dda3-238">messages</span></span>|<span data-ttu-id="7dda3-239">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-239">[Message](message.md) collection</span></span>|<span data-ttu-id="7dda3-240">Коллекция сообщений в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="7dda3-240">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="7dda3-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7dda3-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="7dda3-242">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7dda3-p110">Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7dda3-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="7dda3-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7dda3-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="7dda3-247">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7dda3-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7dda3-p111">Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7dda3-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7dda3-251">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7dda3-251">JSON representation</span></span>

<span data-ttu-id="7dda3-252">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dda3-252">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="7dda3-253">См. также</span><span class="sxs-lookup"><span data-stu-id="7dda3-253">See also</span></span>

- [<span data-ttu-id="7dda3-254">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="7dda3-254">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="7dda3-255">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="7dda3-255">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
