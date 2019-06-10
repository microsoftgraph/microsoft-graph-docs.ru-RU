---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7f522d6d947d190232d510662dfe2c6a70001fb2
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812924"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="cc502-104">Тип ресурса Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="cc502-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc502-105">**Маилсеарчфолдер** — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-105">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="cc502-106">**маилсеарчфолдер** наследуется от [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cc502-106">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="cc502-107">Папки поиска можно создавать в любой папке почтового ящика Exchange Online пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc502-107">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="cc502-108">Однако для отображения папки поиска в Outlook, Outlook для Интернета или Outlook Live необходимо создать папку в папке **веллкновнфолдернаме. SearchFolders** .</span><span class="sxs-lookup"><span data-stu-id="cc502-108">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="cc502-109">Жизненный цикл папок поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-109">Search folder lifecycle</span></span>

<span data-ttu-id="cc502-110">Папки поиска, созданные приложением, могут быть удалены в Exchange Online по одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="cc502-110">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="cc502-111">Срок действия папок поиска истечет через 45 дней без использования.</span><span class="sxs-lookup"><span data-stu-id="cc502-111">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="cc502-112">Количество папок поиска, которые могут быть созданы для каждой исходной папки, ограничено.</span><span class="sxs-lookup"><span data-stu-id="cc502-112">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="cc502-113">При нарушении этого ограничения старые папки поиска удаляются, чтобы сделать новые.</span><span class="sxs-lookup"><span data-stu-id="cc502-113">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="cc502-114">При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать тот же ресурс.</span><span class="sxs-lookup"><span data-stu-id="cc502-114">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="cc502-115">Методы</span><span class="sxs-lookup"><span data-stu-id="cc502-115">Methods</span></span>

| <span data-ttu-id="cc502-116">Метод</span><span class="sxs-lookup"><span data-stu-id="cc502-116">Method</span></span> | <span data-ttu-id="cc502-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc502-117">Return Type</span></span>  | <span data-ttu-id="cc502-118">Описание</span><span class="sxs-lookup"><span data-stu-id="cc502-118">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="cc502-119">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-119">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="cc502-120">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="cc502-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cc502-121">Создайте папку поиска в почтовом ящике этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc502-121">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="cc502-122">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-122">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="cc502-123">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="cc502-123">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="cc502-124">Перечислите все папки в почтовом ящике этого пользователя, в том числе папки поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-124">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="cc502-125">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-125">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="cc502-126">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="cc502-126">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cc502-127">Получение указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-127">Get the specified search folder.</span></span> |
| [<span data-ttu-id="cc502-128">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-128">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="cc502-129">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="cc502-129">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cc502-130">Обновление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-130">Update the specified search folder.</span></span> |
| [<span data-ttu-id="cc502-131">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-131">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="cc502-132">Нет</span><span class="sxs-lookup"><span data-stu-id="cc502-132">None</span></span> | <span data-ttu-id="cc502-133">Удаление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-133">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="cc502-134">Перечисление всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="cc502-134">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="cc502-135">Коллекция [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="cc502-135">[message](message.md) collection</span></span> | <span data-ttu-id="cc502-136">Перечисление всех сообщений в указанной папке поиска.</span><span class="sxs-lookup"><span data-stu-id="cc502-136">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc502-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc502-137">Properties</span></span>

| <span data-ttu-id="cc502-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc502-138">Property</span></span> | <span data-ttu-id="cc502-139">Тип</span><span class="sxs-lookup"><span data-stu-id="cc502-139">Type</span></span> | <span data-ttu-id="cc502-140">Описание</span><span class="sxs-lookup"><span data-stu-id="cc502-140">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="cc502-141">Поддержка</span><span class="sxs-lookup"><span data-stu-id="cc502-141">isSupported</span></span> | <span data-ttu-id="cc502-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc502-142">Boolean</span></span> | <span data-ttu-id="cc502-143">Указывает, является ли папка поиска редактируемой с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="cc502-143">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="cc502-144">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="cc502-144">includeNestedFolders</span></span> | <span data-ttu-id="cc502-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc502-145">Boolean</span></span> | <span data-ttu-id="cc502-146">Указывает, как должна проходить иерархия папок почтовых ящиков в поиске.</span><span class="sxs-lookup"><span data-stu-id="cc502-146">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="cc502-147">`true`означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="cc502-147">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="cc502-148">`false`означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**.</span><span class="sxs-lookup"><span data-stu-id="cc502-148">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="cc502-149">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="cc502-149">sourceFolderIds</span></span> | <span data-ttu-id="cc502-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc502-150">String collection</span></span> | <span data-ttu-id="cc502-151">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="cc502-151">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="cc502-152">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="cc502-152">filterQuery</span></span> | <span data-ttu-id="cc502-153">String</span><span class="sxs-lookup"><span data-stu-id="cc502-153">String</span></span> | <span data-ttu-id="cc502-154">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="cc502-154">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc502-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc502-155">JSON representation</span></span>

<span data-ttu-id="cc502-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc502-156">The following is a JSON representation of the resource.</span></span>

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
