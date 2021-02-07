---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d2363f2bc25ddf3356215910e14b3451fccf6fcf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130776"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="6738f-104">Тип ресурса mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-104">mailFolder resource type</span></span>

<span data-ttu-id="6738f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6738f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6738f-106">Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики".</span><span class="sxs-lookup"><span data-stu-id="6738f-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="6738f-107">Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="6738f-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="6738f-108">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="6738f-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="6738f-109">**Известные имена папок**</span><span class="sxs-lookup"><span data-stu-id="6738f-109">**Well-known folder names**</span></span>

<span data-ttu-id="6738f-110">Outlook создает определенные папки для пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6738f-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="6738f-111">Для удобства вместо значения **id** для доступа к папкам можно использовать известные имена папок из таблицы ниже.</span><span class="sxs-lookup"><span data-stu-id="6738f-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="6738f-112">Например, вы можете получить папку черновиков, использовав ее известное имя со следующим запросом.</span><span class="sxs-lookup"><span data-stu-id="6738f-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="6738f-113">Известные имена поддерживаются вне зависимости от языкового стандарта почтового ящика пользователя, поэтому указанный выше запрос всегда возвращает папку черновиков пользователя, независимо от ее имени.</span><span class="sxs-lookup"><span data-stu-id="6738f-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="6738f-114">Известное имя папки</span><span class="sxs-lookup"><span data-stu-id="6738f-114">Well-known folder name</span></span> | <span data-ttu-id="6738f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6738f-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="6738f-116">archive</span><span class="sxs-lookup"><span data-stu-id="6738f-116">archive</span></span> | <span data-ttu-id="6738f-117">Архивная папка, в которую отправляются сообщения при использовании функции архивации одним щелчком в клиентах Outlook, поддерживающих ее.</span><span class="sxs-lookup"><span data-stu-id="6738f-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="6738f-118">**Примечание.** Она отличается от функции архивного почтового ящика Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6738f-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="6738f-119">clutter</span><span class="sxs-lookup"><span data-stu-id="6738f-119">clutter</span></span> | <span data-ttu-id="6738f-120">Папка "Несрочные", в которую перемещаются сообщения низкой важности при использовании функции "Несрочные".</span><span class="sxs-lookup"><span data-stu-id="6738f-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="6738f-121">conflicts</span><span class="sxs-lookup"><span data-stu-id="6738f-121">conflicts</span></span> | <span data-ttu-id="6738f-122">Папка, содержащая конфликтующие элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6738f-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="6738f-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="6738f-123">conversationhistory</span></span> | <span data-ttu-id="6738f-124">Папка, в которой Skype сохраняет беседы при обмене мгновенными сообщениями (если Skype настроен для этого).</span><span class="sxs-lookup"><span data-stu-id="6738f-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="6738f-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="6738f-125">deleteditems</span></span> | <span data-ttu-id="6738f-126">Папка, в которую перемещаются элементы при их удалении.</span><span class="sxs-lookup"><span data-stu-id="6738f-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="6738f-127">drafts</span><span class="sxs-lookup"><span data-stu-id="6738f-127">drafts</span></span> | <span data-ttu-id="6738f-128">Папка, содержащая неотправленные сообщения.</span><span class="sxs-lookup"><span data-stu-id="6738f-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="6738f-129">inbox</span><span class="sxs-lookup"><span data-stu-id="6738f-129">inbox</span></span> | <span data-ttu-id="6738f-130">Папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6738f-130">The inbox folder.</span></span> |
| <span data-ttu-id="6738f-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="6738f-131">junkemail</span></span> | <span data-ttu-id="6738f-132">Папка нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="6738f-132">The junk email folder.</span></span> |
| <span data-ttu-id="6738f-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="6738f-133">localfailures</span></span> | <span data-ttu-id="6738f-134">Папка, содержащая элементы, существующие в локальном клиенте, но которые нельзя отправить на сервер.</span><span class="sxs-lookup"><span data-stu-id="6738f-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="6738f-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="6738f-135">msgfolderroot</span></span> | <span data-ttu-id="6738f-136">Папка "Корневой уровень хранилища".</span><span class="sxs-lookup"><span data-stu-id="6738f-136">The "Top of Information Store" folder.</span></span> <span data-ttu-id="6738f-137">Эта папка является родительской для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6738f-137">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="6738f-138">outbox</span><span class="sxs-lookup"><span data-stu-id="6738f-138">outbox</span></span> | <span data-ttu-id="6738f-139">Папка "Исходящие".</span><span class="sxs-lookup"><span data-stu-id="6738f-139">The outbox folder.</span></span> |
| <span data-ttu-id="6738f-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="6738f-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="6738f-141">Папка, содержащая обратимо удаленные элементы: удаленные из папки "Удаленные" или путем нажатия клавиш SHIFT+DELETE в Outlook.</span><span class="sxs-lookup"><span data-stu-id="6738f-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="6738f-142">Эта папка не отображается в почтовых клиентах Outlook, но пользователи могут взаимодействовать с ней с помощью функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6738f-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="6738f-143">scheduled</span><span class="sxs-lookup"><span data-stu-id="6738f-143">scheduled</span></span> | <span data-ttu-id="6738f-144">Папка, содержащая сообщения, запланированные для повторного отображения в папке "Входящие" с помощью функции "Расписание" в Outlook для iOS.</span><span class="sxs-lookup"><span data-stu-id="6738f-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="6738f-145">searchfolders</span><span class="sxs-lookup"><span data-stu-id="6738f-145">searchfolders</span></span> | <span data-ttu-id="6738f-146">Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6738f-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="6738f-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="6738f-147">sentitems</span></span> | <span data-ttu-id="6738f-148">Папка "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="6738f-148">The sent items folder.</span></span> |
| <span data-ttu-id="6738f-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="6738f-149">serverfailures</span></span> | <span data-ttu-id="6738f-150">Папка, содержащая элементы, существующие на сервере, но которые нельзя синхронизировать с локальным клиентом.</span><span class="sxs-lookup"><span data-stu-id="6738f-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="6738f-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="6738f-151">syncissues</span></span> | <span data-ttu-id="6738f-152">Папка, содержащая журналы синхронизации, созданные в Outlook.</span><span class="sxs-lookup"><span data-stu-id="6738f-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="6738f-153">Методы</span><span class="sxs-lookup"><span data-stu-id="6738f-153">Methods</span></span>

| <span data-ttu-id="6738f-154">Метод</span><span class="sxs-lookup"><span data-stu-id="6738f-154">Method</span></span> | <span data-ttu-id="6738f-155">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6738f-155">Return Type</span></span> | <span data-ttu-id="6738f-156">Описание</span><span class="sxs-lookup"><span data-stu-id="6738f-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="6738f-157">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-157">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="6738f-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-158">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="6738f-159">Чтение свойств и связей объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-159">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="6738f-160">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-160">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="6738f-161">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-161">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="6738f-162">Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.</span><span class="sxs-lookup"><span data-stu-id="6738f-162">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="6738f-163">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-163">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="6738f-164">Коллекция [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-164">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="6738f-p107">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="6738f-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="6738f-167">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="6738f-167">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="6738f-168">Message</span><span class="sxs-lookup"><span data-stu-id="6738f-168">Message</span></span>](message.md)| <span data-ttu-id="6738f-169">Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="6738f-169">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="6738f-170">Вывод списка сообщений</span><span class="sxs-lookup"><span data-stu-id="6738f-170">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="6738f-171">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-171">[Message](message.md) collection</span></span>| <span data-ttu-id="6738f-172">Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6738f-172">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="6738f-173">Обновление</span><span class="sxs-lookup"><span data-stu-id="6738f-173">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="6738f-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-174">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6738f-175">Обновление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-175">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="6738f-176">Удаление</span><span class="sxs-lookup"><span data-stu-id="6738f-176">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="6738f-177">Нет</span><span class="sxs-lookup"><span data-stu-id="6738f-177">None</span></span> |<span data-ttu-id="6738f-178">Удаление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-178">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="6738f-179">copy</span><span class="sxs-lookup"><span data-stu-id="6738f-179">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="6738f-180">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-180">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6738f-181">Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-181">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="6738f-182">delta</span><span class="sxs-lookup"><span data-stu-id="6738f-182">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="6738f-183">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-183">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="6738f-184">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="6738f-184">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="6738f-185">move</span><span class="sxs-lookup"><span data-stu-id="6738f-185">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="6738f-186">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-186">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6738f-187">Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-187">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="6738f-188">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="6738f-188">**Extended properties**</span></span>| | |
|[<span data-ttu-id="6738f-189">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="6738f-189">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="6738f-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-190">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="6738f-191">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-191">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="6738f-192">Получение элемента mailFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="6738f-192">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6738f-193">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-193">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6738f-194">Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6738f-194">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="6738f-195">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="6738f-195">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="6738f-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-196">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6738f-197">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-197">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="6738f-198">Получение элемента mailFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="6738f-198">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6738f-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6738f-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6738f-200">Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="6738f-200">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="6738f-201">Свойства</span><span class="sxs-lookup"><span data-stu-id="6738f-201">Properties</span></span>

| <span data-ttu-id="6738f-202">Свойство</span><span class="sxs-lookup"><span data-stu-id="6738f-202">Property</span></span> | <span data-ttu-id="6738f-203">Тип</span><span class="sxs-lookup"><span data-stu-id="6738f-203">Type</span></span> | <span data-ttu-id="6738f-204">Описание</span><span class="sxs-lookup"><span data-stu-id="6738f-204">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="6738f-205">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="6738f-205">childFolderCount</span></span>|<span data-ttu-id="6738f-206">Int32</span><span class="sxs-lookup"><span data-stu-id="6738f-206">Int32</span></span>|<span data-ttu-id="6738f-207">Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-207">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="6738f-208">displayName</span><span class="sxs-lookup"><span data-stu-id="6738f-208">displayName</span></span>|<span data-ttu-id="6738f-209">Строка</span><span class="sxs-lookup"><span data-stu-id="6738f-209">String</span></span>|<span data-ttu-id="6738f-210">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-210">The mailFolder's display name.</span></span>|
|<span data-ttu-id="6738f-211">id</span><span class="sxs-lookup"><span data-stu-id="6738f-211">id</span></span>|<span data-ttu-id="6738f-212">Строка</span><span class="sxs-lookup"><span data-stu-id="6738f-212">String</span></span>|<span data-ttu-id="6738f-213">Уникальный идентификатор элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-213">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="6738f-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="6738f-214">parentFolderId</span></span>|<span data-ttu-id="6738f-215">Строка</span><span class="sxs-lookup"><span data-stu-id="6738f-215">String</span></span>|<span data-ttu-id="6738f-216">Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-216">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="6738f-217">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="6738f-217">totalItemCount</span></span>|<span data-ttu-id="6738f-218">Int32</span><span class="sxs-lookup"><span data-stu-id="6738f-218">Int32</span></span>|<span data-ttu-id="6738f-219">Количество элементов в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-219">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="6738f-220">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="6738f-220">unreadItemCount</span></span>|<span data-ttu-id="6738f-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6738f-221">Int32</span></span>|<span data-ttu-id="6738f-222">Количество элементов, помеченных как непрочитанные, в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-222">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="6738f-223">**Эффективный доступ к сведениям о количестве элементов**</span><span class="sxs-lookup"><span data-stu-id="6738f-223">**Access item counts efficiently**</span></span>

<span data-ttu-id="6738f-224">Используя такие свойства папки, как `TotalItemCount` и `UnreadItemCount`, можно удобно вычислять количество прочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="6738f-224">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="6738f-225">Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.</span><span class="sxs-lookup"><span data-stu-id="6738f-225">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="6738f-226">Папки почты в Outlook могут содержать элементы нескольких типов, например, папка "Входящие" может содержать элементы приглашений на собрания, не связанные с почтовыми элементами.</span><span class="sxs-lookup"><span data-stu-id="6738f-226">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="6738f-227">Свойства `TotalItemCount` и `UnreadItemCount` включают элементы из папки почты вне зависимости от их типов.</span><span class="sxs-lookup"><span data-stu-id="6738f-227">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="6738f-228">Отношения</span><span class="sxs-lookup"><span data-stu-id="6738f-228">Relationships</span></span>

| <span data-ttu-id="6738f-229">Связь</span><span class="sxs-lookup"><span data-stu-id="6738f-229">Relationship</span></span> | <span data-ttu-id="6738f-230">Тип</span><span class="sxs-lookup"><span data-stu-id="6738f-230">Type</span></span> | <span data-ttu-id="6738f-231">Описание</span><span class="sxs-lookup"><span data-stu-id="6738f-231">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="6738f-232">childFolders</span><span class="sxs-lookup"><span data-stu-id="6738f-232">childFolders</span></span>|<span data-ttu-id="6738f-233">Коллекция объектов [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-233">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="6738f-234">Коллекция дочерних папок в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-234">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="6738f-235">messageRules</span><span class="sxs-lookup"><span data-stu-id="6738f-235">messageRules</span></span> | <span data-ttu-id="6738f-236">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-236">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="6738f-237">Коллекция правил, которые применяются к папке пользователя "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6738f-237">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="6738f-238">messages</span><span class="sxs-lookup"><span data-stu-id="6738f-238">messages</span></span>|<span data-ttu-id="6738f-239">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-239">[Message](message.md) collection</span></span>|<span data-ttu-id="6738f-240">Коллекция сообщений в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="6738f-240">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="6738f-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6738f-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="6738f-242">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6738f-p110">Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6738f-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6738f-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6738f-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="6738f-247">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="6738f-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6738f-p111">Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6738f-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6738f-251">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6738f-251">JSON representation</span></span>

<span data-ttu-id="6738f-252">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6738f-252">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6738f-253">См. также</span><span class="sxs-lookup"><span data-stu-id="6738f-253">See also</span></span>

- [<span data-ttu-id="6738f-254">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="6738f-254">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="6738f-255">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="6738f-255">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

