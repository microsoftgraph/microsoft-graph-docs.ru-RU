---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска. mailSearchFolder наследуется от mailFolder.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9e153999cfa647b2f8f13e350b3193b358b536cf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129711"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="5547b-104">Тип ресурса mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5547b-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="5547b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5547b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5547b-106">**MailSearchFolder** — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-106">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="5547b-107">**mailSearchFolder** наследуется от [mailFolder.](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5547b-107">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="5547b-108">Папки поиска можно создавать в любой папке в почтовом ящике пользователя Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5547b-108">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="5547b-109">Однако для того, чтобы папка поиска появлялася в Outlook, Outlook в Интернете или Outlook Live, ее необходимо создать в папке **WellKnownFolderName.SearchFolders.**</span><span class="sxs-lookup"><span data-stu-id="5547b-109">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="5547b-110">Жизненный цикл папки поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-110">Search folder lifecycle</span></span>

<span data-ttu-id="5547b-111">Exchange Online может удалить папки поиска, созданные приложением, по одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="5547b-111">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="5547b-112">Срок действия папок поиска истекает через 45 дней без использования.</span><span class="sxs-lookup"><span data-stu-id="5547b-112">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="5547b-113">Количество папок поиска, которые можно создать для одной из исходных папок, ограничивается.</span><span class="sxs-lookup"><span data-stu-id="5547b-113">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="5547b-114">При нарушении этого ограничения старые папки поиска удаляются для укладки новых.</span><span class="sxs-lookup"><span data-stu-id="5547b-114">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="5547b-115">При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать то же самое.</span><span class="sxs-lookup"><span data-stu-id="5547b-115">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="5547b-116">Методы</span><span class="sxs-lookup"><span data-stu-id="5547b-116">Methods</span></span>

| <span data-ttu-id="5547b-117">Метод</span><span class="sxs-lookup"><span data-stu-id="5547b-117">Method</span></span> | <span data-ttu-id="5547b-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5547b-118">Return Type</span></span>  | <span data-ttu-id="5547b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5547b-119">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="5547b-120">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-120">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="5547b-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5547b-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5547b-122">Создайте папку поиска в почтовом ящике этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5547b-122">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="5547b-123">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-123">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="5547b-124">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5547b-124">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="5547b-125">Список всех папок в почтовом ящике этого пользователя, включая папки поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-125">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="5547b-126">Получить папку поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-126">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="5547b-127">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5547b-127">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5547b-128">Получите указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-128">Get the specified search folder.</span></span> |
| [<span data-ttu-id="5547b-129">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-129">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="5547b-130">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5547b-130">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5547b-131">Обновим указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-131">Update the specified search folder.</span></span> |
| [<span data-ttu-id="5547b-132">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-132">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="5547b-133">Нет</span><span class="sxs-lookup"><span data-stu-id="5547b-133">None</span></span> | <span data-ttu-id="5547b-134">Удалите указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-134">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="5547b-135">Список всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="5547b-135">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="5547b-136">Коллекция объектов [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="5547b-136">[message](message.md) collection</span></span> | <span data-ttu-id="5547b-137">Список всех сообщений в указанной папке поиска.</span><span class="sxs-lookup"><span data-stu-id="5547b-137">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="5547b-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="5547b-138">Properties</span></span>

| <span data-ttu-id="5547b-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="5547b-139">Property</span></span> | <span data-ttu-id="5547b-140">Тип</span><span class="sxs-lookup"><span data-stu-id="5547b-140">Type</span></span> | <span data-ttu-id="5547b-141">Описание</span><span class="sxs-lookup"><span data-stu-id="5547b-141">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5547b-142">isSupported</span><span class="sxs-lookup"><span data-stu-id="5547b-142">isSupported</span></span> | <span data-ttu-id="5547b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5547b-143">Boolean</span></span> | <span data-ttu-id="5547b-144">Указывает, можно ли редактировать папку поиска с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="5547b-144">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="5547b-145">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="5547b-145">includeNestedFolders</span></span> | <span data-ttu-id="5547b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5547b-146">Boolean</span></span> | <span data-ttu-id="5547b-147">Указывает, как должна проходить иерархия папок почтового ящика в поиске.</span><span class="sxs-lookup"><span data-stu-id="5547b-147">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="5547b-148">`true`означает, что следует глубоко искать, чтобы включить в иерархию каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="5547b-148">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="5547b-149">`false`означает неглубокий поиск только каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="5547b-149">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="5547b-150">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="5547b-150">sourceFolderIds</span></span> | <span data-ttu-id="5547b-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5547b-151">String collection</span></span> | <span data-ttu-id="5547b-152">Папки почтового ящика, которые необходимо миновать.</span><span class="sxs-lookup"><span data-stu-id="5547b-152">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5547b-153">filterQuery</span><span class="sxs-lookup"><span data-stu-id="5547b-153">filterQuery</span></span> | <span data-ttu-id="5547b-154">String</span><span class="sxs-lookup"><span data-stu-id="5547b-154">String</span></span> | <span data-ttu-id="5547b-155">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="5547b-155">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5547b-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5547b-156">JSON representation</span></span>

<span data-ttu-id="5547b-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5547b-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

