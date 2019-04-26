---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562607"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="a3333-104">Тип ресурса Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="a3333-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3333-105">Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="a3333-106">Маилсеарчфолдер наследуется от [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a3333-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a3333-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3333-107">Methods</span></span>

| <span data-ttu-id="a3333-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3333-108">Method</span></span> | <span data-ttu-id="a3333-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3333-109">Return Type</span></span>  | <span data-ttu-id="a3333-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3333-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="a3333-111">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="a3333-112">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="a3333-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="a3333-113">Создайте папку поиска в почтовом ящике этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3333-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="a3333-114">Список папок поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="a3333-115">Коллекция [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="a3333-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="a3333-116">ПереЧислите все папки в почтовом ящике этого пользователя, в том числе папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="a3333-117">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="a3333-118">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="a3333-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="a3333-119">Получение указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="a3333-120">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="a3333-121">Маилсеарчфолдер</span><span class="sxs-lookup"><span data-stu-id="a3333-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="a3333-122">Обновление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="a3333-123">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="a3333-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a3333-124">None</span></span> | <span data-ttu-id="a3333-125">Удаление указанной папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="a3333-126">ПереЧисление всех сообщений в папке поиска</span><span class="sxs-lookup"><span data-stu-id="a3333-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="a3333-127">Коллекция объектов [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="a3333-127">[message](message.md) collection</span></span> | <span data-ttu-id="a3333-128">ПереЧисление всех сообщений в указанной папке поиска.</span><span class="sxs-lookup"><span data-stu-id="a3333-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3333-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3333-129">Properties</span></span>

| <span data-ttu-id="a3333-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3333-130">Property</span></span> | <span data-ttu-id="a3333-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3333-131">Type</span></span> | <span data-ttu-id="a3333-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3333-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="a3333-133">Поддержка</span><span class="sxs-lookup"><span data-stu-id="a3333-133">isSupported</span></span> | <span data-ttu-id="a3333-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3333-134">Boolean</span></span> | <span data-ttu-id="a3333-135">Указывает, является ли папка поиска редактируемой с помощью REST API.</span><span class="sxs-lookup"><span data-stu-id="a3333-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="a3333-136">Инклуденестедфолдерс</span><span class="sxs-lookup"><span data-stu-id="a3333-136">includeNestedFolders</span></span> | <span data-ttu-id="a3333-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3333-137">Boolean</span></span> | <span data-ttu-id="a3333-138">Указывает, как должна проходить иерархия папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a3333-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="a3333-139">`true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск.</span><span class="sxs-lookup"><span data-stu-id="a3333-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="a3333-140">Саурцефолдеридс</span><span class="sxs-lookup"><span data-stu-id="a3333-140">sourceFolderIDs</span></span> | <span data-ttu-id="a3333-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3333-141">String collection</span></span> | <span data-ttu-id="a3333-142">Папки почтовых ящиков, которые должны быть mined.</span><span class="sxs-lookup"><span data-stu-id="a3333-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="a3333-143">Филтеркуери</span><span class="sxs-lookup"><span data-stu-id="a3333-143">filterQuery</span></span> | <span data-ttu-id="a3333-144">String</span><span class="sxs-lookup"><span data-stu-id="a3333-144">String</span></span> | <span data-ttu-id="a3333-145">Запрос OData для фильтрации сообщений.</span><span class="sxs-lookup"><span data-stu-id="a3333-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a3333-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3333-146">JSON representation</span></span>

<span data-ttu-id="a3333-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3333-147">The following is a JSON representation of the resource.</span></span>

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
