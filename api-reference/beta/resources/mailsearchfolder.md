---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8d2e9892f72c3106eafd8d48e06a32a826e68a5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971827"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="09435-104">Тип ресурса Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="09435-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="09435-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09435-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09435-106">**Маилсеарчфолдер** — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-106">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="09435-107">**маилсеарчфолдер** наследуется от [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="09435-107">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="09435-108">Папки поиска можно создавать в любой папке почтового ящика Exchange Online пользователя.</span><span class="sxs-lookup"><span data-stu-id="09435-108">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="09435-109">Однако для отображения папки поиска в Outlook, Outlook для Интернета или Outlook Live необходимо создать папку в папке **веллкновнфолдернаме. SearchFolders** .</span><span class="sxs-lookup"><span data-stu-id="09435-109">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="09435-110">Жизненный цикл папок поиска</span><span class="sxs-lookup"><span data-stu-id="09435-110">Search folder lifecycle</span></span>

<span data-ttu-id="09435-111">Папки поиска, созданные приложением, могут быть удалены в Exchange Online по одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="09435-111">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="09435-112">Срок действия папок поиска истечет через 45 дней без использования.</span><span class="sxs-lookup"><span data-stu-id="09435-112">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="09435-113">Количество папок поиска, которые могут быть созданы для каждой исходной папки, ограничено.</span><span class="sxs-lookup"><span data-stu-id="09435-113">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="09435-114">При нарушении этого ограничения старые папки поиска удаляются, чтобы сделать новые.</span><span class="sxs-lookup"><span data-stu-id="09435-114">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="09435-115">При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать тот же ресурс.</span><span class="sxs-lookup"><span data-stu-id="09435-115">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="09435-116">Методы</span><span class="sxs-lookup"><span data-stu-id="09435-116">Methods</span></span>

| <span data-ttu-id="09435-117">Метод</span><span class="sxs-lookup"><span data-stu-id="09435-117">Method</span></span> | <span data-ttu-id="09435-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="09435-118">Return Type</span></span>  | <span data-ttu-id="09435-119">Описание</span><span class="sxs-lookup"><span data-stu-id="09435-119">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="09435-120">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="09435-120">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="09435-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="09435-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="09435-122">Создайте папку поиска в почтовом ящике этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="09435-122">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="09435-123">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="09435-123">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="09435-124">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="09435-124">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="09435-125">Перечислите все папки в почтовом ящике этого пользователя, в том числе папки поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-125">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="09435-126">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="09435-126">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="09435-127">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="09435-127">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="09435-128">Получение указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-128">Get the specified search folder.</span></span> |
| [<span data-ttu-id="09435-129">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="09435-129">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="09435-130">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="09435-130">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="09435-131">Обновление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-131">Update the specified search folder.</span></span> |
| [<span data-ttu-id="09435-132">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="09435-132">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="09435-133">Нет</span><span class="sxs-lookup"><span data-stu-id="09435-133">None</span></span> | <span data-ttu-id="09435-134">Удаление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-134">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="09435-135">Перечисление всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="09435-135">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="09435-136">Коллекция [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="09435-136">[message](message.md) collection</span></span> | <span data-ttu-id="09435-137">Перечисление всех сообщений в указанной папке поиска.</span><span class="sxs-lookup"><span data-stu-id="09435-137">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="09435-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="09435-138">Properties</span></span>

| <span data-ttu-id="09435-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="09435-139">Property</span></span> | <span data-ttu-id="09435-140">Тип</span><span class="sxs-lookup"><span data-stu-id="09435-140">Type</span></span> | <span data-ttu-id="09435-141">Описание</span><span class="sxs-lookup"><span data-stu-id="09435-141">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="09435-142">Поддержка</span><span class="sxs-lookup"><span data-stu-id="09435-142">isSupported</span></span> | <span data-ttu-id="09435-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="09435-143">Boolean</span></span> | <span data-ttu-id="09435-144">Указывает, является ли папка поиска редактируемой с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="09435-144">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="09435-145">инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="09435-145">includeNestedFolders</span></span> | <span data-ttu-id="09435-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="09435-146">Boolean</span></span> | <span data-ttu-id="09435-147">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="09435-147">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="09435-148">`true` означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="09435-148">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="09435-149">`false` означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="09435-149">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="09435-150">саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="09435-150">sourceFolderIds</span></span> | <span data-ttu-id="09435-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09435-151">String collection</span></span> | <span data-ttu-id="09435-152">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="09435-152">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="09435-153">филтеркуери</span><span class="sxs-lookup"><span data-stu-id="09435-153">filterQuery</span></span> | <span data-ttu-id="09435-154">String</span><span class="sxs-lookup"><span data-stu-id="09435-154">String</span></span> | <span data-ttu-id="09435-155">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="09435-155">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09435-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09435-156">JSON representation</span></span>

<span data-ttu-id="09435-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09435-157">The following is a JSON representation of the resource.</span></span>

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


