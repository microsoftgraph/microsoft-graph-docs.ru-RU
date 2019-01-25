---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска. mailSearchFolder наследует от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520986"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="afe6b-104">Тип ресурса mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="afe6b-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe6b-105">MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="afe6b-106">mailSearchFolder наследует от [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="afe6b-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="afe6b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="afe6b-107">Methods</span></span>

| <span data-ttu-id="afe6b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="afe6b-108">Method</span></span> | <span data-ttu-id="afe6b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="afe6b-109">Return Type</span></span>  | <span data-ttu-id="afe6b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="afe6b-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="afe6b-111">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="afe6b-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="afe6b-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="afe6b-113">Создание папки поиска в этом почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="afe6b-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="afe6b-114">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="afe6b-115">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="afe6b-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="afe6b-116">Список всех папок в этом почтовом ящике пользователя, включая папки поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="afe6b-117">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="afe6b-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="afe6b-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="afe6b-119">Получение папки поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="afe6b-120">Изменение папки поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="afe6b-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="afe6b-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="afe6b-122">Обновление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="afe6b-123">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="afe6b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="afe6b-124">None</span></span> | <span data-ttu-id="afe6b-125">Удаление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="afe6b-126">Список всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="afe6b-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="afe6b-127">Коллекция объектов [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="afe6b-127">[message](message.md) collection</span></span> | <span data-ttu-id="afe6b-128">Список всех сообщений в папке поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="afe6b-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="afe6b-129">Properties</span></span>

| <span data-ttu-id="afe6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="afe6b-130">Property</span></span> | <span data-ttu-id="afe6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="afe6b-131">Type</span></span> | <span data-ttu-id="afe6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="afe6b-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="afe6b-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="afe6b-133">isSupported</span></span> | <span data-ttu-id="afe6b-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="afe6b-134">Boolean</span></span> | <span data-ttu-id="afe6b-135">Указывает, является ли папки поиска редактирования с помощью API-интерфейсы REST.</span><span class="sxs-lookup"><span data-stu-id="afe6b-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="afe6b-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="afe6b-136">includeNestedFolders</span></span> | <span data-ttu-id="afe6b-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="afe6b-137">Boolean</span></span> | <span data-ttu-id="afe6b-138">Указывает, как должен выполняться иерархии папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="afe6b-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="afe6b-139">`true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска.</span><span class="sxs-lookup"><span data-stu-id="afe6b-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="afe6b-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="afe6b-140">sourceFolderIDs</span></span> | <span data-ttu-id="afe6b-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="afe6b-141">String collection</span></span> | <span data-ttu-id="afe6b-142">Папки почтовых ящиков, которые должны быть получены.</span><span class="sxs-lookup"><span data-stu-id="afe6b-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="afe6b-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="afe6b-143">filterQuery</span></span> | <span data-ttu-id="afe6b-144">String</span><span class="sxs-lookup"><span data-stu-id="afe6b-144">String</span></span> | <span data-ttu-id="afe6b-145">Запросов OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="afe6b-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="afe6b-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afe6b-146">JSON representation</span></span>

<span data-ttu-id="afe6b-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afe6b-147">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
