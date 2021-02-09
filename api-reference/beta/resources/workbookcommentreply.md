---
title: Тип ресурса workbookCommentReply
description: Определение типа ресурса workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dc25b02005e0f419fbb878005006f155f1f99e72
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159432"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="6ed26-103">Тип ресурса workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="6ed26-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="6ed26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ed26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ed26-105">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="6ed26-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="6ed26-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6ed26-106">Methods</span></span>

| <span data-ttu-id="6ed26-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6ed26-107">Method</span></span>       | <span data-ttu-id="6ed26-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6ed26-108">Return Type</span></span> | <span data-ttu-id="6ed26-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6ed26-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6ed26-110">Список workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="6ed26-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="6ed26-111">[Коллекция workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="6ed26-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="6ed26-112">Получить список объектов workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="6ed26-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="6ed26-113">Get workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="6ed26-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="6ed26-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="6ed26-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="6ed26-115">Чтение свойств и связей объекта workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="6ed26-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="6ed26-116">Создание workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="6ed26-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="6ed26-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="6ed26-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="6ed26-118">Создайте новую книгуCommentReply.</span><span class="sxs-lookup"><span data-stu-id="6ed26-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="6ed26-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ed26-119">Properties</span></span>

| <span data-ttu-id="6ed26-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ed26-120">Property</span></span>     | <span data-ttu-id="6ed26-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6ed26-121">Type</span></span>        | <span data-ttu-id="6ed26-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ed26-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6ed26-123">content</span><span class="sxs-lookup"><span data-stu-id="6ed26-123">content</span></span>|<span data-ttu-id="6ed26-124">String</span><span class="sxs-lookup"><span data-stu-id="6ed26-124">String</span></span>|<span data-ttu-id="6ed26-125">Содержимое ответного комментария.</span><span class="sxs-lookup"><span data-stu-id="6ed26-125">The content of replied comment.</span></span>|
|<span data-ttu-id="6ed26-126">contentType</span><span class="sxs-lookup"><span data-stu-id="6ed26-126">contentType</span></span>|<span data-ttu-id="6ed26-127">String</span><span class="sxs-lookup"><span data-stu-id="6ed26-127">String</span></span>|<span data-ttu-id="6ed26-128">Указывает тип ответного комментария.</span><span class="sxs-lookup"><span data-stu-id="6ed26-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="6ed26-129">id</span><span class="sxs-lookup"><span data-stu-id="6ed26-129">id</span></span>|<span data-ttu-id="6ed26-130">String</span><span class="sxs-lookup"><span data-stu-id="6ed26-130">String</span></span>|<span data-ttu-id="6ed26-131">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="6ed26-131">Represents the comment identifier.</span></span> <span data-ttu-id="6ed26-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ed26-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ed26-133">Связи</span><span class="sxs-lookup"><span data-stu-id="6ed26-133">Relationships</span></span>

<span data-ttu-id="6ed26-134">Нет</span><span class="sxs-lookup"><span data-stu-id="6ed26-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ed26-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ed26-135">JSON representation</span></span>

<span data-ttu-id="6ed26-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ed26-136">The following is a JSON representation of the resource.</span></span>

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


