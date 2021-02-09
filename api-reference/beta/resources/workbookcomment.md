---
title: Тип ресурса workbookComment
description: Представляет комментарий в книге.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 920eff7126d3628e798e10a3e1cc9985d64d6602
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154238"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="95109-103">Тип ресурса workbookComment</span><span class="sxs-lookup"><span data-stu-id="95109-103">workbookComment resource type</span></span>

<span data-ttu-id="95109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95109-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95109-105">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="95109-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="95109-106">Методы</span><span class="sxs-lookup"><span data-stu-id="95109-106">Methods</span></span>

| <span data-ttu-id="95109-107">Метод</span><span class="sxs-lookup"><span data-stu-id="95109-107">Method</span></span>       | <span data-ttu-id="95109-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95109-108">Return Type</span></span> | <span data-ttu-id="95109-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95109-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="95109-110">Список workbookComments</span><span class="sxs-lookup"><span data-stu-id="95109-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="95109-111">[коллекция workbookComment](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="95109-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="95109-112">Получите **коллекцию объектов workbookComment.**</span><span class="sxs-lookup"><span data-stu-id="95109-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="95109-113">Get workbookComment</span><span class="sxs-lookup"><span data-stu-id="95109-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="95109-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="95109-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="95109-115">Чтение свойств и связей объекта **workbookComment.**</span><span class="sxs-lookup"><span data-stu-id="95109-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="95109-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="95109-116">Properties</span></span>

| <span data-ttu-id="95109-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="95109-117">Property</span></span>     | <span data-ttu-id="95109-118">Тип</span><span class="sxs-lookup"><span data-stu-id="95109-118">Type</span></span>        | <span data-ttu-id="95109-119">Описание</span><span class="sxs-lookup"><span data-stu-id="95109-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95109-120">content</span><span class="sxs-lookup"><span data-stu-id="95109-120">content</span></span>|<span data-ttu-id="95109-121">String</span><span class="sxs-lookup"><span data-stu-id="95109-121">String</span></span>|<span data-ttu-id="95109-122">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="95109-122">The content of the comment.</span></span>|
|<span data-ttu-id="95109-123">contentType</span><span class="sxs-lookup"><span data-stu-id="95109-123">contentType</span></span>|<span data-ttu-id="95109-124">String</span><span class="sxs-lookup"><span data-stu-id="95109-124">String</span></span>|<span data-ttu-id="95109-125">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="95109-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="95109-126">id</span><span class="sxs-lookup"><span data-stu-id="95109-126">id</span></span>|<span data-ttu-id="95109-127">String</span><span class="sxs-lookup"><span data-stu-id="95109-127">String</span></span>| <span data-ttu-id="95109-128">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="95109-128">Represents the comment identifier.</span></span> <span data-ttu-id="95109-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95109-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95109-130">Связи</span><span class="sxs-lookup"><span data-stu-id="95109-130">Relationships</span></span>

| <span data-ttu-id="95109-131">Связь</span><span class="sxs-lookup"><span data-stu-id="95109-131">Relationship</span></span> | <span data-ttu-id="95109-132">Тип</span><span class="sxs-lookup"><span data-stu-id="95109-132">Type</span></span>        | <span data-ttu-id="95109-133">Описание</span><span class="sxs-lookup"><span data-stu-id="95109-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95109-134">replies</span><span class="sxs-lookup"><span data-stu-id="95109-134">replies</span></span>|<span data-ttu-id="95109-135">[Коллекция workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="95109-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="95109-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="95109-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95109-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95109-138">JSON representation</span></span>

<span data-ttu-id="95109-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95109-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


