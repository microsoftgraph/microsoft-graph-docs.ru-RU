---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7e829929df46208ee321f56ae2d9f0144c320d4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036332"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="126bf-104">Тип ресурса mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-104">mailFolder resource type</span></span>

<span data-ttu-id="126bf-105">Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики".</span><span class="sxs-lookup"><span data-stu-id="126bf-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="126bf-106">Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="126bf-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="126bf-107">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="126bf-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="126bf-108">**Известные имена папок**</span><span class="sxs-lookup"><span data-stu-id="126bf-108">**Well-known folder names**</span></span>

<span data-ttu-id="126bf-109">Outlook создает определенные папки для пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="126bf-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="126bf-110">Для удобства вместо значения **id** для доступа к папкам можно использовать известные имена папок из таблицы ниже.</span><span class="sxs-lookup"><span data-stu-id="126bf-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="126bf-111">Например, вы можете получить папку черновиков, использовав ее известное имя со следующим запросом.</span><span class="sxs-lookup"><span data-stu-id="126bf-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="126bf-112">Известные имена поддерживаются вне зависимости от языкового стандарта почтового ящика пользователя, поэтому указанный выше запрос всегда возвращает папку черновиков пользователя, независимо от ее имени.</span><span class="sxs-lookup"><span data-stu-id="126bf-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="126bf-113">Известное имя папки</span><span class="sxs-lookup"><span data-stu-id="126bf-113">Well-known folder name</span></span> | <span data-ttu-id="126bf-114">Описание</span><span class="sxs-lookup"><span data-stu-id="126bf-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="126bf-115">archive</span><span class="sxs-lookup"><span data-stu-id="126bf-115">archive</span></span> | <span data-ttu-id="126bf-116">Архивная папка, в которую отправляются сообщения при использовании функции архивации одним щелчком в клиентах Outlook, поддерживающих ее.</span><span class="sxs-lookup"><span data-stu-id="126bf-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="126bf-117">**Примечание.** Она отличается от функции архивного почтового ящика Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="126bf-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="126bf-118">clutter</span><span class="sxs-lookup"><span data-stu-id="126bf-118">clutter</span></span> | <span data-ttu-id="126bf-119">Папка "Несрочные", в которую перемещаются сообщения низкой важности при использовании функции "Несрочные".</span><span class="sxs-lookup"><span data-stu-id="126bf-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="126bf-120">conflicts</span><span class="sxs-lookup"><span data-stu-id="126bf-120">conflicts</span></span> | <span data-ttu-id="126bf-121">Папка, содержащая конфликтующие элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="126bf-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="126bf-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="126bf-122">conversationhistory</span></span> | <span data-ttu-id="126bf-123">Папка, в которой Skype сохраняет беседы при обмене мгновенными сообщениями (если Skype настроен для этого).</span><span class="sxs-lookup"><span data-stu-id="126bf-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="126bf-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="126bf-124">deleteditems</span></span> | <span data-ttu-id="126bf-125">Папка, в которую перемещаются элементы при их удалении.</span><span class="sxs-lookup"><span data-stu-id="126bf-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="126bf-126">drafts</span><span class="sxs-lookup"><span data-stu-id="126bf-126">drafts</span></span> | <span data-ttu-id="126bf-127">Папка, содержащая неотправленные сообщения.</span><span class="sxs-lookup"><span data-stu-id="126bf-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="126bf-128">inbox</span><span class="sxs-lookup"><span data-stu-id="126bf-128">inbox</span></span> | <span data-ttu-id="126bf-129">Папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="126bf-129">The inbox folder.</span></span> |
| <span data-ttu-id="126bf-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="126bf-130">junkemail</span></span> | <span data-ttu-id="126bf-131">Папка нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="126bf-131">The junk email folder.</span></span> |
| <span data-ttu-id="126bf-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="126bf-132">localfailures</span></span> | <span data-ttu-id="126bf-133">Папка, содержащая элементы, существующие в локальном клиенте, но которые нельзя отправить на сервер.</span><span class="sxs-lookup"><span data-stu-id="126bf-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="126bf-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="126bf-134">msgfolderroot</span></span> | <span data-ttu-id="126bf-135">Папка "Корневой уровень хранилища".</span><span class="sxs-lookup"><span data-stu-id="126bf-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="126bf-136">Эта папка является родительской для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="126bf-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="126bf-137">outbox</span><span class="sxs-lookup"><span data-stu-id="126bf-137">outbox</span></span> | <span data-ttu-id="126bf-138">Папка "Исходящие".</span><span class="sxs-lookup"><span data-stu-id="126bf-138">The outbox folder.</span></span> |
| <span data-ttu-id="126bf-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="126bf-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="126bf-140">Папка, содержащая обратимо удаленные элементы: удаленные из папки "Удаленные" или путем нажатия клавиш SHIFT+DELETE в Outlook.</span><span class="sxs-lookup"><span data-stu-id="126bf-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="126bf-141">Эта папка не отображается в почтовых клиентах Outlook, но пользователи могут взаимодействовать с ней с помощью функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="126bf-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="126bf-142">scheduled</span><span class="sxs-lookup"><span data-stu-id="126bf-142">scheduled</span></span> | <span data-ttu-id="126bf-143">Папка, содержащая сообщения, запланированные для повторного отображения в папке "Входящие" с помощью функции "Расписание" в Outlook для iOS.</span><span class="sxs-lookup"><span data-stu-id="126bf-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="126bf-144">searchfolders</span><span class="sxs-lookup"><span data-stu-id="126bf-144">searchfolders</span></span> | <span data-ttu-id="126bf-145">Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="126bf-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="126bf-146">sentitems</span><span class="sxs-lookup"><span data-stu-id="126bf-146">sentitems</span></span> | <span data-ttu-id="126bf-147">Папка "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="126bf-147">The sent items folder.</span></span> |
| <span data-ttu-id="126bf-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="126bf-148">serverfailures</span></span> | <span data-ttu-id="126bf-149">Папка, содержащая элементы, существующие на сервере, но которые нельзя синхронизировать с локальным клиентом.</span><span class="sxs-lookup"><span data-stu-id="126bf-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="126bf-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="126bf-150">syncissues</span></span> | <span data-ttu-id="126bf-151">Папка, содержащая журналы синхронизации, созданные в Outlook.</span><span class="sxs-lookup"><span data-stu-id="126bf-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="126bf-152">Методы</span><span class="sxs-lookup"><span data-stu-id="126bf-152">Methods</span></span>

| <span data-ttu-id="126bf-153">Метод</span><span class="sxs-lookup"><span data-stu-id="126bf-153">Method</span></span> | <span data-ttu-id="126bf-154">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="126bf-154">Return Type</span></span> | <span data-ttu-id="126bf-155">Описание</span><span class="sxs-lookup"><span data-stu-id="126bf-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="126bf-156">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="126bf-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="126bf-158">Чтение свойств и связей объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="126bf-159">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="126bf-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="126bf-161">Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.</span><span class="sxs-lookup"><span data-stu-id="126bf-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="126bf-162">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="126bf-163">Коллекция [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="126bf-p107">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="126bf-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="126bf-166">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="126bf-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="126bf-167">Message</span><span class="sxs-lookup"><span data-stu-id="126bf-167">Message</span></span>](message.md)| <span data-ttu-id="126bf-168">Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="126bf-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="126bf-169">Вывод списка сообщений</span><span class="sxs-lookup"><span data-stu-id="126bf-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="126bf-170">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-170">[Message](message.md) collection</span></span>| <span data-ttu-id="126bf-171">Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="126bf-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="126bf-172">Обновление</span><span class="sxs-lookup"><span data-stu-id="126bf-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="126bf-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="126bf-174">Обновление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="126bf-175">Удаление</span><span class="sxs-lookup"><span data-stu-id="126bf-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="126bf-176">Нет</span><span class="sxs-lookup"><span data-stu-id="126bf-176">None</span></span> |<span data-ttu-id="126bf-177">Удаление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="126bf-178">copy</span><span class="sxs-lookup"><span data-stu-id="126bf-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="126bf-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="126bf-180">Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="126bf-181">delta</span><span class="sxs-lookup"><span data-stu-id="126bf-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="126bf-182">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="126bf-183">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="126bf-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="126bf-184">move</span><span class="sxs-lookup"><span data-stu-id="126bf-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="126bf-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="126bf-186">Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="126bf-187">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="126bf-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="126bf-188">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="126bf-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="126bf-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="126bf-190">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="126bf-191">Получение элемента mailFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="126bf-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="126bf-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="126bf-193">Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="126bf-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="126bf-194">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="126bf-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="126bf-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="126bf-196">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="126bf-197">Получение элемента mailFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="126bf-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="126bf-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="126bf-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="126bf-199">Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="126bf-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="126bf-200">Свойства</span><span class="sxs-lookup"><span data-stu-id="126bf-200">Properties</span></span>

| <span data-ttu-id="126bf-201">Свойство</span><span class="sxs-lookup"><span data-stu-id="126bf-201">Property</span></span> | <span data-ttu-id="126bf-202">Тип</span><span class="sxs-lookup"><span data-stu-id="126bf-202">Type</span></span> | <span data-ttu-id="126bf-203">Описание</span><span class="sxs-lookup"><span data-stu-id="126bf-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="126bf-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="126bf-204">childFolderCount</span></span>|<span data-ttu-id="126bf-205">Int32</span><span class="sxs-lookup"><span data-stu-id="126bf-205">Int32</span></span>|<span data-ttu-id="126bf-206">Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="126bf-207">displayName</span><span class="sxs-lookup"><span data-stu-id="126bf-207">displayName</span></span>|<span data-ttu-id="126bf-208">Строка</span><span class="sxs-lookup"><span data-stu-id="126bf-208">String</span></span>|<span data-ttu-id="126bf-209">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="126bf-210">id</span><span class="sxs-lookup"><span data-stu-id="126bf-210">id</span></span>|<span data-ttu-id="126bf-211">Строка</span><span class="sxs-lookup"><span data-stu-id="126bf-211">String</span></span>|<span data-ttu-id="126bf-212">Уникальный идентификатор элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="126bf-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="126bf-213">parentFolderId</span></span>|<span data-ttu-id="126bf-214">Строка</span><span class="sxs-lookup"><span data-stu-id="126bf-214">String</span></span>|<span data-ttu-id="126bf-215">Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="126bf-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="126bf-216">totalItemCount</span></span>|<span data-ttu-id="126bf-217">Int32</span><span class="sxs-lookup"><span data-stu-id="126bf-217">Int32</span></span>|<span data-ttu-id="126bf-218">Количество элементов в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="126bf-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="126bf-219">unreadItemCount</span></span>|<span data-ttu-id="126bf-220">Int32</span><span class="sxs-lookup"><span data-stu-id="126bf-220">Int32</span></span>|<span data-ttu-id="126bf-221">Количество элементов, помеченных как непрочитанные, в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="126bf-222">**Эффективный доступ к сведениям о количестве элементов**</span><span class="sxs-lookup"><span data-stu-id="126bf-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="126bf-223">Используя такие свойства папки, как `TotalItemCount` и `UnreadItemCount`, можно удобно вычислять количество прочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="126bf-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="126bf-224">Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.</span><span class="sxs-lookup"><span data-stu-id="126bf-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="126bf-225">Папки почты в Outlook могут содержать элементы нескольких типов, например, папка "Входящие" может содержать элементы приглашений на собрания, не связанные с почтовыми элементами.</span><span class="sxs-lookup"><span data-stu-id="126bf-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="126bf-226">Свойства `TotalItemCount` и `UnreadItemCount` включают элементы из папки почты вне зависимости от их типов.</span><span class="sxs-lookup"><span data-stu-id="126bf-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="126bf-227">Отношения</span><span class="sxs-lookup"><span data-stu-id="126bf-227">Relationships</span></span>

| <span data-ttu-id="126bf-228">Отношение</span><span class="sxs-lookup"><span data-stu-id="126bf-228">Relationship</span></span> | <span data-ttu-id="126bf-229">Тип</span><span class="sxs-lookup"><span data-stu-id="126bf-229">Type</span></span> | <span data-ttu-id="126bf-230">Описание</span><span class="sxs-lookup"><span data-stu-id="126bf-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="126bf-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="126bf-231">childFolders</span></span>|<span data-ttu-id="126bf-232">Коллекция объектов [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="126bf-233">Коллекция дочерних папок в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="126bf-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="126bf-234">messageRules</span></span> | <span data-ttu-id="126bf-235">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="126bf-236">Коллекция правил, которые применяются к папке пользователя "Входящие".</span><span class="sxs-lookup"><span data-stu-id="126bf-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="126bf-237">messages</span><span class="sxs-lookup"><span data-stu-id="126bf-237">messages</span></span>|<span data-ttu-id="126bf-238">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-238">[Message](message.md) collection</span></span>|<span data-ttu-id="126bf-239">Коллекция сообщений в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="126bf-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="126bf-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="126bf-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="126bf-241">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="126bf-p110">Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="126bf-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="126bf-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="126bf-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="126bf-246">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="126bf-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="126bf-p111">Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="126bf-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="126bf-250">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="126bf-250">JSON representation</span></span>

<span data-ttu-id="126bf-251">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="126bf-251">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="126bf-252">См. также</span><span class="sxs-lookup"><span data-stu-id="126bf-252">See also</span></span>

- [<span data-ttu-id="126bf-253">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="126bf-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="126bf-254">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="126bf-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
