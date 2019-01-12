---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска. mailSearchFolder наследует от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ba9ce248071e3d806383b4cd7e7550c1e3aa145
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920914"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="72f67-104">Тип ресурса mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="72f67-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="72f67-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72f67-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72f67-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72f67-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72f67-107">MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="72f67-108">mailSearchFolder наследует от [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="72f67-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="72f67-109">Методы</span><span class="sxs-lookup"><span data-stu-id="72f67-109">Methods</span></span>

| <span data-ttu-id="72f67-110">Метод</span><span class="sxs-lookup"><span data-stu-id="72f67-110">Method</span></span> | <span data-ttu-id="72f67-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72f67-111">Return Type</span></span>  | <span data-ttu-id="72f67-112">Описание</span><span class="sxs-lookup"><span data-stu-id="72f67-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="72f67-113">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="72f67-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="72f67-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="72f67-115">Создание папки поиска в этом почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="72f67-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="72f67-116">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="72f67-117">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="72f67-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="72f67-118">Список всех папок в этом почтовом ящике пользователя, включая папки поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="72f67-119">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="72f67-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="72f67-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="72f67-121">Получение папки поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="72f67-122">Изменение папки поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="72f67-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="72f67-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="72f67-124">Обновление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="72f67-125">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="72f67-126">Нет</span><span class="sxs-lookup"><span data-stu-id="72f67-126">None</span></span> | <span data-ttu-id="72f67-127">Удаление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="72f67-128">Список всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="72f67-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="72f67-129">Коллекция объектов [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="72f67-129">[message](message.md) collection</span></span> | <span data-ttu-id="72f67-130">Список всех сообщений в папке поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="72f67-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="72f67-131">Properties</span></span>

| <span data-ttu-id="72f67-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="72f67-132">Property</span></span> | <span data-ttu-id="72f67-133">Тип</span><span class="sxs-lookup"><span data-stu-id="72f67-133">Type</span></span> | <span data-ttu-id="72f67-134">Описание</span><span class="sxs-lookup"><span data-stu-id="72f67-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="72f67-135">isSupported</span><span class="sxs-lookup"><span data-stu-id="72f67-135">isSupported</span></span> | <span data-ttu-id="72f67-136">Логический</span><span class="sxs-lookup"><span data-stu-id="72f67-136">Boolean</span></span> | <span data-ttu-id="72f67-137">Указывает, является ли папки поиска редактирования с помощью API-интерфейсы REST.</span><span class="sxs-lookup"><span data-stu-id="72f67-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="72f67-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="72f67-138">includeNestedFolders</span></span> | <span data-ttu-id="72f67-139">Логический</span><span class="sxs-lookup"><span data-stu-id="72f67-139">Boolean</span></span> | <span data-ttu-id="72f67-140">Указывает, как должен выполняться иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="72f67-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="72f67-141">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="72f67-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="72f67-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="72f67-142">sourceFolderIDs</span></span> | <span data-ttu-id="72f67-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="72f67-143">String collection</span></span> | <span data-ttu-id="72f67-144">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="72f67-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="72f67-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="72f67-145">filterQuery</span></span> | <span data-ttu-id="72f67-146">Строка</span><span class="sxs-lookup"><span data-stu-id="72f67-146">String</span></span> | <span data-ttu-id="72f67-147">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="72f67-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72f67-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72f67-148">JSON representation</span></span>

<span data-ttu-id="72f67-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72f67-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
