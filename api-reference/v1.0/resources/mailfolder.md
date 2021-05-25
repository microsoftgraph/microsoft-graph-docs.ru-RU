---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a1ab83dfa3e3da64935a8c3976f12ffd1faf2e3c
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629387"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="92a07-104">Тип ресурса mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-104">mailFolder resource type</span></span>

<span data-ttu-id="92a07-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a07-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92a07-106">Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики".</span><span class="sxs-lookup"><span data-stu-id="92a07-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="92a07-107">Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="92a07-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="92a07-108">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="92a07-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="92a07-109">**Известные имена папок**</span><span class="sxs-lookup"><span data-stu-id="92a07-109">**Well-known folder names**</span></span>

<span data-ttu-id="92a07-110">Outlook создает определенные папки для пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="92a07-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="92a07-111">Для удобства вместо значения **id** для доступа к папкам можно использовать известные имена папок из таблицы ниже.</span><span class="sxs-lookup"><span data-stu-id="92a07-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="92a07-112">Например, вы можете получить папку черновиков, использовав ее известное имя со следующим запросом.</span><span class="sxs-lookup"><span data-stu-id="92a07-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="92a07-113">Известные имена поддерживаются вне зависимости от языкового стандарта почтового ящика пользователя, поэтому указанный выше запрос всегда возвращает папку черновиков пользователя, независимо от ее имени.</span><span class="sxs-lookup"><span data-stu-id="92a07-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="92a07-114">Известное имя папки</span><span class="sxs-lookup"><span data-stu-id="92a07-114">Well-known folder name</span></span> | <span data-ttu-id="92a07-115">Описание</span><span class="sxs-lookup"><span data-stu-id="92a07-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="92a07-116">archive</span><span class="sxs-lookup"><span data-stu-id="92a07-116">archive</span></span> | <span data-ttu-id="92a07-117">Архивная папка, в которую отправляются сообщения при использовании функции архивации одним щелчком в клиентах Outlook, поддерживающих ее.</span><span class="sxs-lookup"><span data-stu-id="92a07-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="92a07-118">**Примечание.** Она отличается от функции архивного почтового ящика Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="92a07-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="92a07-119">clutter</span><span class="sxs-lookup"><span data-stu-id="92a07-119">clutter</span></span> | <span data-ttu-id="92a07-120">Папка "Несрочные", в которую перемещаются сообщения низкой важности при использовании функции "Несрочные".</span><span class="sxs-lookup"><span data-stu-id="92a07-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="92a07-121">conflicts</span><span class="sxs-lookup"><span data-stu-id="92a07-121">conflicts</span></span> | <span data-ttu-id="92a07-122">Папка, содержащая конфликтующие элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="92a07-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="92a07-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="92a07-123">conversationhistory</span></span> | <span data-ttu-id="92a07-124">Папка, в которой Skype сохраняет беседы при обмене мгновенными сообщениями (если Skype настроен для этого).</span><span class="sxs-lookup"><span data-stu-id="92a07-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="92a07-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="92a07-125">deleteditems</span></span> | <span data-ttu-id="92a07-126">Папка, в которую перемещаются элементы при их удалении.</span><span class="sxs-lookup"><span data-stu-id="92a07-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="92a07-127">drafts</span><span class="sxs-lookup"><span data-stu-id="92a07-127">drafts</span></span> | <span data-ttu-id="92a07-128">Папка, содержащая неотправленные сообщения.</span><span class="sxs-lookup"><span data-stu-id="92a07-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="92a07-129">inbox</span><span class="sxs-lookup"><span data-stu-id="92a07-129">inbox</span></span> | <span data-ttu-id="92a07-130">Папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="92a07-130">The inbox folder.</span></span> |
| <span data-ttu-id="92a07-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="92a07-131">junkemail</span></span> | <span data-ttu-id="92a07-132">Папка нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="92a07-132">The junk email folder.</span></span> |
| <span data-ttu-id="92a07-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="92a07-133">localfailures</span></span> | <span data-ttu-id="92a07-134">Папка, содержащая элементы, существующие в локальном клиенте, но которые нельзя отправить на сервер.</span><span class="sxs-lookup"><span data-stu-id="92a07-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="92a07-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="92a07-135">msgfolderroot</span></span> | <span data-ttu-id="92a07-p105">Папка "Корневой уровень хранилища". Эта папка является родительской для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="92a07-p105">The "Top of Information Store" folder. This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="92a07-138">outbox</span><span class="sxs-lookup"><span data-stu-id="92a07-138">outbox</span></span> | <span data-ttu-id="92a07-139">Папка "Исходящие".</span><span class="sxs-lookup"><span data-stu-id="92a07-139">The outbox folder.</span></span> |
| <span data-ttu-id="92a07-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="92a07-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="92a07-141">Папка, содержащая обратимо удаленные элементы: удаленные из папки "Удаленные" или путем нажатия клавиш SHIFT+DELETE в Outlook.</span><span class="sxs-lookup"><span data-stu-id="92a07-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="92a07-142">Эта папка не отображается в почтовых клиентах Outlook, но пользователи могут взаимодействовать с ней с помощью функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="92a07-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="92a07-143">scheduled</span><span class="sxs-lookup"><span data-stu-id="92a07-143">scheduled</span></span> | <span data-ttu-id="92a07-144">Папка, содержащая сообщения, запланированные для повторного отображения в папке "Входящие" с помощью функции "Расписание" в Outlook для iOS.</span><span class="sxs-lookup"><span data-stu-id="92a07-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="92a07-145">searchfolders</span><span class="sxs-lookup"><span data-stu-id="92a07-145">searchfolders</span></span> | <span data-ttu-id="92a07-146">Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="92a07-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="92a07-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="92a07-147">sentitems</span></span> | <span data-ttu-id="92a07-148">Папка "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="92a07-148">The sent items folder.</span></span> |
| <span data-ttu-id="92a07-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="92a07-149">serverfailures</span></span> | <span data-ttu-id="92a07-150">Папка, содержащая элементы, существующие на сервере, но которые нельзя синхронизировать с локальным клиентом.</span><span class="sxs-lookup"><span data-stu-id="92a07-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="92a07-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="92a07-151">syncissues</span></span> | <span data-ttu-id="92a07-152">Папка, содержащая журналы синхронизации, созданные в Outlook.</span><span class="sxs-lookup"><span data-stu-id="92a07-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="92a07-153">Методы</span><span class="sxs-lookup"><span data-stu-id="92a07-153">Methods</span></span>

| <span data-ttu-id="92a07-154">Метод</span><span class="sxs-lookup"><span data-stu-id="92a07-154">Method</span></span> | <span data-ttu-id="92a07-155">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92a07-155">Return Type</span></span> | <span data-ttu-id="92a07-156">Описание</span><span class="sxs-lookup"><span data-stu-id="92a07-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="92a07-157">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-157">List mailFolders</span></span>](../api/user-list-mailfolders.md) | <span data-ttu-id="92a07-158">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-158">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="92a07-159">Получение всех папок почты в указанном почтовом ящике пользователя, включая все папки поиска почты.</span><span class="sxs-lookup"><span data-stu-id="92a07-159">Get all the mail folders in the specified user's mailbox, including any mail search folders.</span></span>|
|[<span data-ttu-id="92a07-160">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-160">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="92a07-161">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-161">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="92a07-162">Чтение свойств и связей объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-162">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="92a07-163">Создание объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-163">Create mailFolder</span></span>](../api/user-post-mailfolders.md) |[<span data-ttu-id="92a07-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-164">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="92a07-165">Создание папки почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="92a07-165">Create a new mail folder in the root folder of the user's mailbox.</span></span>|
|[<span data-ttu-id="92a07-166">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-166">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="92a07-167">Коллекция [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-167">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="92a07-p107">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="92a07-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="92a07-170">Создание объекта childFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-170">Create childFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="92a07-171">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-171">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="92a07-172">Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-172">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="92a07-173">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="92a07-173">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="92a07-174">Message</span><span class="sxs-lookup"><span data-stu-id="92a07-174">Message</span></span>](message.md)| <span data-ttu-id="92a07-175">Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="92a07-175">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="92a07-176">Вывод списка сообщений</span><span class="sxs-lookup"><span data-stu-id="92a07-176">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="92a07-177">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-177">[Message](message.md) collection</span></span>| <span data-ttu-id="92a07-178">Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="92a07-178">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="92a07-179">Обновление</span><span class="sxs-lookup"><span data-stu-id="92a07-179">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="92a07-180">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-180">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="92a07-181">Обновление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-181">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="92a07-182">Удаление</span><span class="sxs-lookup"><span data-stu-id="92a07-182">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="92a07-183">Нет</span><span class="sxs-lookup"><span data-stu-id="92a07-183">None</span></span> |<span data-ttu-id="92a07-184">Удаление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-184">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="92a07-185">copy</span><span class="sxs-lookup"><span data-stu-id="92a07-185">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="92a07-186">MailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-186">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="92a07-187">Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-187">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="92a07-188">delta</span><span class="sxs-lookup"><span data-stu-id="92a07-188">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="92a07-189">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-189">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="92a07-190">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="92a07-190">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="92a07-191">move</span><span class="sxs-lookup"><span data-stu-id="92a07-191">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="92a07-192">MailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-192">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="92a07-193">Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-193">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="92a07-194">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="92a07-194">**Extended properties**</span></span>| | |
|[<span data-ttu-id="92a07-195">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="92a07-195">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="92a07-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-196">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="92a07-197">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-197">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="92a07-198">Получение элемента mailFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="92a07-198">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="92a07-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="92a07-200">Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="92a07-200">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="92a07-201">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="92a07-201">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="92a07-202">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-202">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="92a07-203">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-203">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="92a07-204">Получение элемента mailFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="92a07-204">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="92a07-205">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92a07-205">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="92a07-206">Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="92a07-206">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="92a07-207">Свойства</span><span class="sxs-lookup"><span data-stu-id="92a07-207">Properties</span></span>

| <span data-ttu-id="92a07-208">Свойство</span><span class="sxs-lookup"><span data-stu-id="92a07-208">Property</span></span> | <span data-ttu-id="92a07-209">Тип</span><span class="sxs-lookup"><span data-stu-id="92a07-209">Type</span></span> | <span data-ttu-id="92a07-210">Описание</span><span class="sxs-lookup"><span data-stu-id="92a07-210">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="92a07-211">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="92a07-211">childFolderCount</span></span>|<span data-ttu-id="92a07-212">Int32</span><span class="sxs-lookup"><span data-stu-id="92a07-212">Int32</span></span>|<span data-ttu-id="92a07-213">Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-213">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="92a07-214">displayName</span><span class="sxs-lookup"><span data-stu-id="92a07-214">displayName</span></span>|<span data-ttu-id="92a07-215">Строка</span><span class="sxs-lookup"><span data-stu-id="92a07-215">String</span></span>|<span data-ttu-id="92a07-216">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-216">The mailFolder's display name.</span></span>|
|<span data-ttu-id="92a07-217">id</span><span class="sxs-lookup"><span data-stu-id="92a07-217">id</span></span>|<span data-ttu-id="92a07-218">Строка</span><span class="sxs-lookup"><span data-stu-id="92a07-218">String</span></span>|<span data-ttu-id="92a07-219">Уникальный идентификатор элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-219">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="92a07-220">isHidden</span><span class="sxs-lookup"><span data-stu-id="92a07-220">isHidden</span></span>|<span data-ttu-id="92a07-221">Логический</span><span class="sxs-lookup"><span data-stu-id="92a07-221">Boolean</span></span>|<span data-ttu-id="92a07-222">Указывает, скрыт ли объект mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-222">Indicates whether the mailFolder is hidden.</span></span> <span data-ttu-id="92a07-223">Это свойство можно установить только при создании папки.</span><span class="sxs-lookup"><span data-stu-id="92a07-223">This property can be set only when creating the folder.</span></span> <span data-ttu-id="92a07-224">Дополнительные сведения см. в разделе [Скрытые папки почты](#hidden-mail-folders).</span><span class="sxs-lookup"><span data-stu-id="92a07-224">Find more information in [Hidden mail folders](#hidden-mail-folders).</span></span>|
|<span data-ttu-id="92a07-225">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="92a07-225">parentFolderId</span></span>|<span data-ttu-id="92a07-226">Строка</span><span class="sxs-lookup"><span data-stu-id="92a07-226">String</span></span>|<span data-ttu-id="92a07-227">Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-227">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="92a07-228">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="92a07-228">totalItemCount</span></span>|<span data-ttu-id="92a07-229">Int32</span><span class="sxs-lookup"><span data-stu-id="92a07-229">Int32</span></span>|<span data-ttu-id="92a07-230">Количество элементов в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-230">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="92a07-231">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="92a07-231">unreadItemCount</span></span>|<span data-ttu-id="92a07-232">Int32</span><span class="sxs-lookup"><span data-stu-id="92a07-232">Int32</span></span>|<span data-ttu-id="92a07-233">Количество элементов, помеченных как непрочитанные, в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-233">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="92a07-234">**Эффективный доступ к сведениям о количестве элементов**</span><span class="sxs-lookup"><span data-stu-id="92a07-234">**Access item counts efficiently**</span></span>

<span data-ttu-id="92a07-235">Используя такие свойства папки, как `TotalItemCount` и `UnreadItemCount`, можно удобно вычислять количество прочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="92a07-235">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="92a07-236">Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.</span><span class="sxs-lookup"><span data-stu-id="92a07-236">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="92a07-237">Папки почты в Outlook могут содержать элементы нескольких типов, например, папка "Входящие" может содержать элементы приглашений на собрания, не связанные с почтовыми элементами.</span><span class="sxs-lookup"><span data-stu-id="92a07-237">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="92a07-238">Свойства `TotalItemCount` и `UnreadItemCount` включают элементы из папки почты вне зависимости от их типов.</span><span class="sxs-lookup"><span data-stu-id="92a07-238">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

### <a name="hidden-mail-folders"></a><span data-ttu-id="92a07-239">Скрытые папки почты</span><span class="sxs-lookup"><span data-stu-id="92a07-239">Hidden mail folders</span></span>
<span data-ttu-id="92a07-240">Значение свойства `isHidden` по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="92a07-240">The default value of the `isHidden` property is `false`.</span></span> <span data-ttu-id="92a07-241">Вы можете задать **isHidden** только один раз при [создании объекта mailFolder](../api/user-post-mailfolders.md).</span><span class="sxs-lookup"><span data-stu-id="92a07-241">You can set **isHidden** only once when [creating the mailFolder](../api/user-post-mailfolders.md).</span></span> <span data-ttu-id="92a07-242">Обновление свойства с помощью операции PATCH невозможно.</span><span class="sxs-lookup"><span data-stu-id="92a07-242">You cannot update the property using a PATCH operation.</span></span> <span data-ttu-id="92a07-243">Чтобы изменить свойство **isHidden** папки, удалите существующую папку и создайте новую с нужным значением.</span><span class="sxs-lookup"><span data-stu-id="92a07-243">To change the **isHidden** property of a folder, delete the existing folder and create a new one with the desired value.</span></span>

<span data-ttu-id="92a07-244">Скрытые папки почты поддерживают все операции, поддерживаемые обычной почтовой папкой.</span><span class="sxs-lookup"><span data-stu-id="92a07-244">Hidden mail folders support all operations that are supported by a regular mail folder.</span></span>

<span data-ttu-id="92a07-245">По умолчанию при [перечислении объектов mailFolder](../api/user-list-mailfolders.md) возвращаются только не скрытые папки почты.</span><span class="sxs-lookup"><span data-stu-id="92a07-245">By default, [listing mailFolders](../api/user-list-mailfolders.md) returns only mail folders that are not hidden.</span></span> <span data-ttu-id="92a07-246">Чтобы включить скрытые папки почты в отклик, используйте параметр запроса `includeHiddenFolders=true`.</span><span class="sxs-lookup"><span data-stu-id="92a07-246">To include hidden mail folders in the response, use the query parameter `includeHiddenFolders=true`.</span></span> <span data-ttu-id="92a07-247">Затем используйте свойство **isHidden**, чтобы определить, скрыта ли папка почты.</span><span class="sxs-lookup"><span data-stu-id="92a07-247">Then use the **isHidden** property to identify whether a mail folder is hidden.</span></span> 

## <a name="relationships"></a><span data-ttu-id="92a07-248">Связи</span><span class="sxs-lookup"><span data-stu-id="92a07-248">Relationships</span></span>

| <span data-ttu-id="92a07-249">Связь</span><span class="sxs-lookup"><span data-stu-id="92a07-249">Relationship</span></span> | <span data-ttu-id="92a07-250">Тип</span><span class="sxs-lookup"><span data-stu-id="92a07-250">Type</span></span> | <span data-ttu-id="92a07-251">Описание</span><span class="sxs-lookup"><span data-stu-id="92a07-251">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="92a07-252">childFolders</span><span class="sxs-lookup"><span data-stu-id="92a07-252">childFolders</span></span>|<span data-ttu-id="92a07-253">Коллекция объектов [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-253">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="92a07-254">Коллекция дочерних папок в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-254">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="92a07-255">messageRules</span><span class="sxs-lookup"><span data-stu-id="92a07-255">messageRules</span></span> | <span data-ttu-id="92a07-256">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-256">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="92a07-257">Коллекция правил, которые применяются к папке пользователя "Входящие".</span><span class="sxs-lookup"><span data-stu-id="92a07-257">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="92a07-258">messages</span><span class="sxs-lookup"><span data-stu-id="92a07-258">messages</span></span>|<span data-ttu-id="92a07-259">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-259">[Message](message.md) collection</span></span>|<span data-ttu-id="92a07-260">Коллекция сообщений в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="92a07-260">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="92a07-261">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="92a07-261">multiValueExtendedProperties</span></span>|<span data-ttu-id="92a07-262">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-262">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="92a07-p113">Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="92a07-p113">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="92a07-266">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="92a07-266">singleValueExtendedProperties</span></span>|<span data-ttu-id="92a07-267">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="92a07-267">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="92a07-p114">Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="92a07-p114">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92a07-271">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92a07-271">JSON representation</span></span>

<span data-ttu-id="92a07-272">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92a07-272">Here is a JSON representation of the resource</span></span>

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
  "isHidden": false,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="92a07-273">См. также</span><span class="sxs-lookup"><span data-stu-id="92a07-273">See also</span></span>

- [<span data-ttu-id="92a07-274">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="92a07-274">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="92a07-275">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="92a07-275">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

