---
title: Тип ресурса Воркбуккоммент
description: Представляет комментарий в книге.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 11e0b1538f6d2b41a8b211e1a7cc4ac45d2703a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079642"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="d582b-103">Тип ресурса Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d582b-103">workbookComment resource type</span></span>

<span data-ttu-id="d582b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d582b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d582b-105">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="d582b-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="d582b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d582b-106">Methods</span></span>

| <span data-ttu-id="d582b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d582b-107">Method</span></span>       | <span data-ttu-id="d582b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d582b-108">Return Type</span></span> | <span data-ttu-id="d582b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d582b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d582b-110">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="d582b-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="d582b-111">Коллекция [воркбуккоммент](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="d582b-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="d582b-112">Получение коллекции объектов **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="d582b-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="d582b-113">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d582b-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="d582b-114">воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d582b-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="d582b-115">Чтение свойств и связей объекта **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="d582b-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="d582b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d582b-116">Properties</span></span>

| <span data-ttu-id="d582b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d582b-117">Property</span></span>     | <span data-ttu-id="d582b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d582b-118">Type</span></span>        | <span data-ttu-id="d582b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d582b-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d582b-120">content</span><span class="sxs-lookup"><span data-stu-id="d582b-120">content</span></span>|<span data-ttu-id="d582b-121">String</span><span class="sxs-lookup"><span data-stu-id="d582b-121">String</span></span>|<span data-ttu-id="d582b-122">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="d582b-122">The content of the comment.</span></span>|
|<span data-ttu-id="d582b-123">contentType</span><span class="sxs-lookup"><span data-stu-id="d582b-123">contentType</span></span>|<span data-ttu-id="d582b-124">String</span><span class="sxs-lookup"><span data-stu-id="d582b-124">String</span></span>|<span data-ttu-id="d582b-125">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="d582b-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="d582b-126">id</span><span class="sxs-lookup"><span data-stu-id="d582b-126">id</span></span>|<span data-ttu-id="d582b-127">String</span><span class="sxs-lookup"><span data-stu-id="d582b-127">String</span></span>| <span data-ttu-id="d582b-128">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="d582b-128">Represents the comment identifier.</span></span> <span data-ttu-id="d582b-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d582b-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d582b-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="d582b-130">Relationships</span></span>

| <span data-ttu-id="d582b-131">Связь</span><span class="sxs-lookup"><span data-stu-id="d582b-131">Relationship</span></span> | <span data-ttu-id="d582b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d582b-132">Type</span></span>        | <span data-ttu-id="d582b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d582b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d582b-134">отвечать</span><span class="sxs-lookup"><span data-stu-id="d582b-134">replies</span></span>|<span data-ttu-id="d582b-135">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="d582b-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="d582b-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d582b-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d582b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d582b-138">JSON representation</span></span>

<span data-ttu-id="d582b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d582b-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "",
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


