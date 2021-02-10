---
title: Тип ресурса workbookCommentReply
description: Определение типа ресурса workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7c47a6eb7abf8bf675dd8be35db6a96e511dbbcf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158039"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="e1688-103">Тип ресурса workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="e1688-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="e1688-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1688-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1688-105">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="e1688-105">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="e1688-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e1688-106">Methods</span></span>

| <span data-ttu-id="e1688-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e1688-107">Method</span></span>       | <span data-ttu-id="e1688-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1688-108">Return Type</span></span> | <span data-ttu-id="e1688-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1688-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e1688-110">Список workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="e1688-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="e1688-111">[Коллекция workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="e1688-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="e1688-112">Получить список объектов workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="e1688-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="e1688-113">Get workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="e1688-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="e1688-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="e1688-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="e1688-115">Чтение свойств и связей объекта workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="e1688-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="e1688-116">Создание workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="e1688-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="e1688-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="e1688-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="e1688-118">Создайте новую книгуCommentReply.</span><span class="sxs-lookup"><span data-stu-id="e1688-118">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="e1688-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1688-119">Properties</span></span>

| <span data-ttu-id="e1688-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1688-120">Property</span></span>     | <span data-ttu-id="e1688-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e1688-121">Type</span></span>        | <span data-ttu-id="e1688-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1688-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1688-123">content</span><span class="sxs-lookup"><span data-stu-id="e1688-123">content</span></span>|<span data-ttu-id="e1688-124">String</span><span class="sxs-lookup"><span data-stu-id="e1688-124">String</span></span>|<span data-ttu-id="e1688-125">Содержимое ответа на комментарий.</span><span class="sxs-lookup"><span data-stu-id="e1688-125">The content of a comment reply.</span></span>|
|<span data-ttu-id="e1688-126">contentType</span><span class="sxs-lookup"><span data-stu-id="e1688-126">contentType</span></span>|<span data-ttu-id="e1688-127">String</span><span class="sxs-lookup"><span data-stu-id="e1688-127">String</span></span>|<span data-ttu-id="e1688-128">Указывает тип ответа на комментарий.</span><span class="sxs-lookup"><span data-stu-id="e1688-128">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="e1688-129">id</span><span class="sxs-lookup"><span data-stu-id="e1688-129">id</span></span>|<span data-ttu-id="e1688-130">String</span><span class="sxs-lookup"><span data-stu-id="e1688-130">String</span></span>|<span data-ttu-id="e1688-131">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="e1688-131">Represents the comment identifier.</span></span> <span data-ttu-id="e1688-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1688-132">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e1688-133">Связи</span><span class="sxs-lookup"><span data-stu-id="e1688-133">Relationships</span></span>

<span data-ttu-id="e1688-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e1688-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1688-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e1688-135">JSON representation</span></span>

<span data-ttu-id="e1688-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1688-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

