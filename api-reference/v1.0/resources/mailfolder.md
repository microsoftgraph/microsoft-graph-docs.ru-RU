---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dbcb35ad0b131f4e714acd7f178fbbb1109b913c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920116"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="f4853-104">Тип ресурса mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-104">mailFolder resource type</span></span>

<span data-ttu-id="f4853-105">Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики".</span><span class="sxs-lookup"><span data-stu-id="f4853-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="f4853-106">Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="f4853-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="f4853-107">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="f4853-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="f4853-108">**Имена папок хорошо известные**</span><span class="sxs-lookup"><span data-stu-id="f4853-108">**Well-known folder names**</span></span>

<span data-ttu-id="f4853-109">Outlook создает определенные папки для пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f4853-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="f4853-110">Вместо использования соответствующее значение **идентификатора** папки для удобства, можно использовать имена известных папок из приведенной ниже таблице при доступе к этих папок.</span><span class="sxs-lookup"><span data-stu-id="f4853-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="f4853-111">Например можно получить папке "Черновики", с помощью имени известных с помощью следующего запроса.</span><span class="sxs-lookup"><span data-stu-id="f4853-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="f4853-112">Хорошо известные имена работать независимо от языкового стандарта из почтового ящика пользователя выше запрос всегда будет возвращать Папка «Черновики» пользователя независимо от того, как с именем.</span><span class="sxs-lookup"><span data-stu-id="f4853-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="f4853-113">Имя хорошо известные папки</span><span class="sxs-lookup"><span data-stu-id="f4853-113">Well-known folder name</span></span> | <span data-ttu-id="f4853-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f4853-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="f4853-115">архив</span><span class="sxs-lookup"><span data-stu-id="f4853-115">archive</span></span> | <span data-ttu-id="f4853-116">Сообщения папки архива отправляются при использовании функции архивации One_Click в клиентах Outlook, которые поддерживают его.</span><span class="sxs-lookup"><span data-stu-id="f4853-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="f4853-117">**Примечание:** это не то же, что компонент архивного почтового ящика из Exchange online.</span><span class="sxs-lookup"><span data-stu-id="f4853-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="f4853-118">засорение</span><span class="sxs-lookup"><span data-stu-id="f4853-118">clutter</span></span> | <span data-ttu-id="f4853-119">Сообщения с низким приоритетом папки засорение перемещаются при использовании функции беспорядок.</span><span class="sxs-lookup"><span data-stu-id="f4853-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="f4853-120">конфликтов</span><span class="sxs-lookup"><span data-stu-id="f4853-120">conflicts</span></span> | <span data-ttu-id="f4853-121">Папка, содержащая конфликтующих элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f4853-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="f4853-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="f4853-122">conversationhistory</span></span> | <span data-ttu-id="f4853-123">Папка, где Скайп сохраняет мгновенные сообщения (если Скайп настроен для этого).</span><span class="sxs-lookup"><span data-stu-id="f4853-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="f4853-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="f4853-124">deleteditems</span></span> | <span data-ttu-id="f4853-125">Элементы папки перемещаются при удалении.</span><span class="sxs-lookup"><span data-stu-id="f4853-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="f4853-126">черновики</span><span class="sxs-lookup"><span data-stu-id="f4853-126">drafts</span></span> | <span data-ttu-id="f4853-127">Папка, содержащая неотправленные сообщения.</span><span class="sxs-lookup"><span data-stu-id="f4853-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="f4853-128">папки «Входящие»</span><span class="sxs-lookup"><span data-stu-id="f4853-128">inbox</span></span> | <span data-ttu-id="f4853-129">Папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="f4853-129">The inbox folder.</span></span> |
| <span data-ttu-id="f4853-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="f4853-130">junkemail</span></span> | <span data-ttu-id="f4853-131">В папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="f4853-131">The junk email folder.</span></span> |
| <span data-ttu-id="f4853-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="f4853-132">localfailures</span></span> | <span data-ttu-id="f4853-133">Папка, содержащая элементы, которые существуют на локальных клиентов, но не удалось загрузить на сервер.</span><span class="sxs-lookup"><span data-stu-id="f4853-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="f4853-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="f4853-134">msgfolderroot</span></span> | <span data-ttu-id="f4853-135">Папка «Хранилища».</span><span class="sxs-lookup"><span data-stu-id="f4853-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="f4853-136">Эта папка является родительской папки для папок, которые отображаются в обычном почтовых клиентах, таких как папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="f4853-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="f4853-137">Исходящие</span><span class="sxs-lookup"><span data-stu-id="f4853-137">outbox</span></span> | <span data-ttu-id="f4853-138">Папка "Исходящие".</span><span class="sxs-lookup"><span data-stu-id="f4853-138">The outbox folder.</span></span> |
| <span data-ttu-id="f4853-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="f4853-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="f4853-140">Папка, содержащая удаленные элементы: удален из папки «Удаленные», либо при нажатии клавиши shift + удаление в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f4853-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="f4853-141">Эта папка не отображается в любой клиент электронной почты Outlook, но конечные пользователи могут взаимодействовать с его посредством функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f4853-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="f4853-142">запланировано</span><span class="sxs-lookup"><span data-stu-id="f4853-142">scheduled</span></span> | <span data-ttu-id="f4853-143">Папка, содержащая сообщения, которые планируется снова появится в папке "Входящие", с помощью функции расписание в Outlook для операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="f4853-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="f4853-144">searchfolders</span><span class="sxs-lookup"><span data-stu-id="f4853-144">searchfolders</span></span> | <span data-ttu-id="f4853-145">Родительской папки для всех папок поиска, определенного в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4853-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="f4853-146">папки "Отправленные"</span><span class="sxs-lookup"><span data-stu-id="f4853-146">sentitems</span></span> | <span data-ttu-id="f4853-147">Папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="f4853-147">The sent items folder.</span></span> |
| <span data-ttu-id="f4853-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="f4853-148">serverfailures</span></span> | <span data-ttu-id="f4853-149">Папка, содержащая элементы, которые существуют на сервере, но не будет синхронизирована с локальных клиентских.</span><span class="sxs-lookup"><span data-stu-id="f4853-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="f4853-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="f4853-150">syncissues</span></span> | <span data-ttu-id="f4853-151">Папка, содержащая синхронизации журналов, созданных в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f4853-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="f4853-152">Методы</span><span class="sxs-lookup"><span data-stu-id="f4853-152">Methods</span></span>

| <span data-ttu-id="f4853-153">Метод</span><span class="sxs-lookup"><span data-stu-id="f4853-153">Method</span></span> | <span data-ttu-id="f4853-154">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4853-154">Return Type</span></span> | <span data-ttu-id="f4853-155">Описание</span><span class="sxs-lookup"><span data-stu-id="f4853-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="f4853-156">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="f4853-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="f4853-158">Чтение свойств и связей объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="f4853-159">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="f4853-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="f4853-161">Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.</span><span class="sxs-lookup"><span data-stu-id="f4853-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="f4853-162">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="f4853-163">Коллекция [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="f4853-p107">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="f4853-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="f4853-166">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="f4853-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="f4853-167">Message</span><span class="sxs-lookup"><span data-stu-id="f4853-167">Message</span></span>](message.md)| <span data-ttu-id="f4853-168">Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="f4853-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="f4853-169">Вывод списка сообщений</span><span class="sxs-lookup"><span data-stu-id="f4853-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="f4853-170">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-170">[Message](message.md) collection</span></span>| <span data-ttu-id="f4853-171">Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f4853-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="f4853-172">Обновление</span><span class="sxs-lookup"><span data-stu-id="f4853-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="f4853-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="f4853-174">Обновление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="f4853-175">Удаление</span><span class="sxs-lookup"><span data-stu-id="f4853-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="f4853-176">Нет</span><span class="sxs-lookup"><span data-stu-id="f4853-176">None</span></span> |<span data-ttu-id="f4853-177">Удаление указанного объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="f4853-178">copy</span><span class="sxs-lookup"><span data-stu-id="f4853-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="f4853-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="f4853-180">Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="f4853-181">delta</span><span class="sxs-lookup"><span data-stu-id="f4853-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="f4853-182">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="f4853-183">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="f4853-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="f4853-184">move</span><span class="sxs-lookup"><span data-stu-id="f4853-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="f4853-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="f4853-186">Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="f4853-187">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="f4853-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="f4853-188">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="f4853-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="f4853-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="f4853-190">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="f4853-191">Получение элемента mailFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="f4853-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f4853-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="f4853-193">Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f4853-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="f4853-194">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="f4853-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="f4853-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="f4853-196">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="f4853-197">Получение элемента mailFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="f4853-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f4853-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f4853-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="f4853-199">Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="f4853-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4853-200">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4853-200">Properties</span></span>

| <span data-ttu-id="f4853-201">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4853-201">Property</span></span> | <span data-ttu-id="f4853-202">Тип</span><span class="sxs-lookup"><span data-stu-id="f4853-202">Type</span></span> | <span data-ttu-id="f4853-203">Описание</span><span class="sxs-lookup"><span data-stu-id="f4853-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="f4853-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="f4853-204">childFolderCount</span></span>|<span data-ttu-id="f4853-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f4853-205">Int32</span></span>|<span data-ttu-id="f4853-206">Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="f4853-207">displayName</span><span class="sxs-lookup"><span data-stu-id="f4853-207">displayName</span></span>|<span data-ttu-id="f4853-208">String</span><span class="sxs-lookup"><span data-stu-id="f4853-208">String</span></span>|<span data-ttu-id="f4853-209">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="f4853-210">id</span><span class="sxs-lookup"><span data-stu-id="f4853-210">id</span></span>|<span data-ttu-id="f4853-211">String</span><span class="sxs-lookup"><span data-stu-id="f4853-211">String</span></span>|<span data-ttu-id="f4853-212">Уникальный идентификатор mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="f4853-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="f4853-213">parentFolderId</span></span>|<span data-ttu-id="f4853-214">Строка</span><span class="sxs-lookup"><span data-stu-id="f4853-214">String</span></span>|<span data-ttu-id="f4853-215">Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="f4853-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="f4853-216">totalItemCount</span></span>|<span data-ttu-id="f4853-217">Int32</span><span class="sxs-lookup"><span data-stu-id="f4853-217">Int32</span></span>|<span data-ttu-id="f4853-218">Количество элементов в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="f4853-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="f4853-219">unreadItemCount</span></span>|<span data-ttu-id="f4853-220">Int32</span><span class="sxs-lookup"><span data-stu-id="f4853-220">Int32</span></span>|<span data-ttu-id="f4853-221">Количество элементов, помеченных как непрочитанные, в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="f4853-222">**Эффективный доступ к сведениям о количестве элементов**</span><span class="sxs-lookup"><span data-stu-id="f4853-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="f4853-223">`TotalItemCount` И `UnreadItemCount` свойства папки позволяют легко создавать вычисления количества чтения элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="f4853-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="f4853-224">Они позволяют предотвратить запросов, который может привести к значительным задержка следующим образом:</span><span class="sxs-lookup"><span data-stu-id="f4853-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="f4853-225">Почтовые папки в Outlook может содержать несколько типов элементов, например, может содержать папки «Входящие» элементы запроса, которые отличаются от почтовых элементов собрания.</span><span class="sxs-lookup"><span data-stu-id="f4853-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="f4853-226">`TotalItemCount`и `UnreadItemCount` включать элементы в папке почты независимо от их типов элементов.</span><span class="sxs-lookup"><span data-stu-id="f4853-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4853-227">Связи</span><span class="sxs-lookup"><span data-stu-id="f4853-227">Relationships</span></span>

| <span data-ttu-id="f4853-228">Связь</span><span class="sxs-lookup"><span data-stu-id="f4853-228">Relationship</span></span> | <span data-ttu-id="f4853-229">Тип</span><span class="sxs-lookup"><span data-stu-id="f4853-229">Type</span></span> | <span data-ttu-id="f4853-230">Описание</span><span class="sxs-lookup"><span data-stu-id="f4853-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="f4853-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="f4853-231">childFolders</span></span>|<span data-ttu-id="f4853-232">Коллекция объектов [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="f4853-233">Коллекция дочерних папок в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="f4853-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="f4853-234">messageRules</span></span> | <span data-ttu-id="f4853-235">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="f4853-236">Коллекция правил, которые применяются к папке пользователя "Входящие".</span><span class="sxs-lookup"><span data-stu-id="f4853-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="f4853-237">messages</span><span class="sxs-lookup"><span data-stu-id="f4853-237">messages</span></span>|<span data-ttu-id="f4853-238">Коллекция объектов [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-238">[Message](message.md) collection</span></span>|<span data-ttu-id="f4853-239">Коллекция сообщений в элементе mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f4853-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="f4853-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f4853-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="f4853-241">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f4853-p110">Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f4853-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f4853-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f4853-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="f4853-246">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f4853-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f4853-p111">Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f4853-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4853-250">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4853-250">JSON representation</span></span>

<span data-ttu-id="f4853-251">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4853-251">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f4853-252">См. также</span><span class="sxs-lookup"><span data-stu-id="f4853-252">See also</span></span>

- [<span data-ttu-id="f4853-253">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="f4853-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="f4853-254">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="f4853-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
