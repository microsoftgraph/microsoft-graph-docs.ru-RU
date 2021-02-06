---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска. mailSearchFolder наследуется от mailFolder.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6740d6bac12ca02938c24f6e36dc48b0ab3a316f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129851"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="74212-104">Тип ресурса mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="74212-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="74212-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74212-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74212-106">**MailSearchFolder** — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-106">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="74212-107">**mailSearchFolder** наследуется от [mailFolder.](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="74212-107">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="74212-108">Папки поиска можно создавать в любой папке в почтовом ящике пользователя Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="74212-108">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="74212-109">Однако чтобы папка поиска появлялись в Outlook, Outlook в Интернете или Outlook Live, ее необходимо создать в папке **WellKnownFolderName.SearchFolders.**</span><span class="sxs-lookup"><span data-stu-id="74212-109">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="74212-110">Жизненный цикл папки поиска</span><span class="sxs-lookup"><span data-stu-id="74212-110">Search folder lifecycle</span></span>

<span data-ttu-id="74212-111">Exchange Online может удалить папки поиска, созданные приложением, по одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="74212-111">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="74212-112">Срок действия папок поиска истекает через 45 дней без использования.</span><span class="sxs-lookup"><span data-stu-id="74212-112">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="74212-113">Количество папок поиска, которые можно создать для одной папки источника, ограничивается.</span><span class="sxs-lookup"><span data-stu-id="74212-113">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="74212-114">При нарушении этого ограничения старые папки поиска удаляются для укладки новых.</span><span class="sxs-lookup"><span data-stu-id="74212-114">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="74212-115">При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать то же самое.</span><span class="sxs-lookup"><span data-stu-id="74212-115">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="74212-116">Методы</span><span class="sxs-lookup"><span data-stu-id="74212-116">Methods</span></span>

| <span data-ttu-id="74212-117">Метод</span><span class="sxs-lookup"><span data-stu-id="74212-117">Method</span></span> | <span data-ttu-id="74212-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74212-118">Return Type</span></span>  | <span data-ttu-id="74212-119">Описание</span><span class="sxs-lookup"><span data-stu-id="74212-119">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="74212-120">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="74212-120">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="74212-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="74212-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="74212-122">Создайте папку поиска в почтовом ящике этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="74212-122">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="74212-123">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="74212-123">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="74212-124">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="74212-124">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="74212-125">Список всех папок в почтовом ящике этого пользователя, включая папки поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-125">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="74212-126">Получить папку поиска</span><span class="sxs-lookup"><span data-stu-id="74212-126">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="74212-127">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="74212-127">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="74212-128">Получите указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-128">Get the specified search folder.</span></span> |
| [<span data-ttu-id="74212-129">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="74212-129">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="74212-130">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="74212-130">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="74212-131">Обновим указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-131">Update the specified search folder.</span></span> |
| [<span data-ttu-id="74212-132">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="74212-132">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="74212-133">Нет</span><span class="sxs-lookup"><span data-stu-id="74212-133">None</span></span> | <span data-ttu-id="74212-134">Удалите указанную папку поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-134">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="74212-135">Список всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="74212-135">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="74212-136">Коллекция [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="74212-136">[message](message.md) collection</span></span> | <span data-ttu-id="74212-137">Список всех сообщений в указанной папке поиска.</span><span class="sxs-lookup"><span data-stu-id="74212-137">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="74212-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="74212-138">Properties</span></span>

| <span data-ttu-id="74212-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="74212-139">Property</span></span> | <span data-ttu-id="74212-140">Тип</span><span class="sxs-lookup"><span data-stu-id="74212-140">Type</span></span> | <span data-ttu-id="74212-141">Описание</span><span class="sxs-lookup"><span data-stu-id="74212-141">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="74212-142">isSupported</span><span class="sxs-lookup"><span data-stu-id="74212-142">isSupported</span></span> | <span data-ttu-id="74212-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="74212-143">Boolean</span></span> | <span data-ttu-id="74212-144">Указывает, можно ли редактировать папку поиска с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="74212-144">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="74212-145">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="74212-145">includeNestedFolders</span></span> | <span data-ttu-id="74212-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="74212-146">Boolean</span></span> | <span data-ttu-id="74212-147">Указывает, как должна проходить иерархия папок почтового ящика в поиске.</span><span class="sxs-lookup"><span data-stu-id="74212-147">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="74212-148">`true`означает, что следует глубоко искать, чтобы включить в иерархию каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="74212-148">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="74212-149">`false`означает неглубокий поиск только каждой папки, явно указанной в **sourceFolderIds.**</span><span class="sxs-lookup"><span data-stu-id="74212-149">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="74212-150">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="74212-150">sourceFolderIds</span></span> | <span data-ttu-id="74212-151">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="74212-151">String collection</span></span> | <span data-ttu-id="74212-152">Папки почтового ящика, которые необходимо миновать.</span><span class="sxs-lookup"><span data-stu-id="74212-152">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="74212-153">filterQuery</span><span class="sxs-lookup"><span data-stu-id="74212-153">filterQuery</span></span> | <span data-ttu-id="74212-154">Строка</span><span class="sxs-lookup"><span data-stu-id="74212-154">String</span></span> | <span data-ttu-id="74212-155">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="74212-155">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74212-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74212-156">JSON representation</span></span>

<span data-ttu-id="74212-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74212-157">The following is a JSON representation of the resource.</span></span>

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


