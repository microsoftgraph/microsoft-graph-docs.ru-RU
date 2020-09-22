---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 26c1862a05431f02149cb4ddbef9a8ab57449d37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015157"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="178ea-103">Тип ресурса Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="178ea-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="178ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="178ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="178ea-105">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="178ea-105">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="178ea-106">Методы</span><span class="sxs-lookup"><span data-stu-id="178ea-106">Methods</span></span>

| <span data-ttu-id="178ea-107">Метод</span><span class="sxs-lookup"><span data-stu-id="178ea-107">Method</span></span>       | <span data-ttu-id="178ea-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="178ea-108">Return Type</span></span> | <span data-ttu-id="178ea-109">Описание</span><span class="sxs-lookup"><span data-stu-id="178ea-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="178ea-110">Список Воркбуккомментреплиес</span><span class="sxs-lookup"><span data-stu-id="178ea-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="178ea-111">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="178ea-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="178ea-112">Получение списка объектов воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="178ea-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="178ea-113">Получение Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="178ea-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="178ea-114">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="178ea-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="178ea-115">Чтение свойств и связей объекта Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="178ea-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="178ea-116">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="178ea-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="178ea-117">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="178ea-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="178ea-118">Создание нового Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="178ea-118">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="178ea-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="178ea-119">Properties</span></span>

| <span data-ttu-id="178ea-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="178ea-120">Property</span></span>     | <span data-ttu-id="178ea-121">Тип</span><span class="sxs-lookup"><span data-stu-id="178ea-121">Type</span></span>        | <span data-ttu-id="178ea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="178ea-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="178ea-123">content</span><span class="sxs-lookup"><span data-stu-id="178ea-123">content</span></span>|<span data-ttu-id="178ea-124">String</span><span class="sxs-lookup"><span data-stu-id="178ea-124">String</span></span>|<span data-ttu-id="178ea-125">Содержимое ответа на комментарий.</span><span class="sxs-lookup"><span data-stu-id="178ea-125">The content of a comment reply.</span></span>|
|<span data-ttu-id="178ea-126">contentType</span><span class="sxs-lookup"><span data-stu-id="178ea-126">contentType</span></span>|<span data-ttu-id="178ea-127">String</span><span class="sxs-lookup"><span data-stu-id="178ea-127">String</span></span>|<span data-ttu-id="178ea-128">Указывает тип ответа на комментарий.</span><span class="sxs-lookup"><span data-stu-id="178ea-128">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="178ea-129">id</span><span class="sxs-lookup"><span data-stu-id="178ea-129">id</span></span>|<span data-ttu-id="178ea-130">String</span><span class="sxs-lookup"><span data-stu-id="178ea-130">String</span></span>|<span data-ttu-id="178ea-131">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="178ea-131">Represents the comment identifier.</span></span> <span data-ttu-id="178ea-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="178ea-132">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="178ea-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="178ea-133">Relationships</span></span>

<span data-ttu-id="178ea-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="178ea-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="178ea-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="178ea-135">JSON representation</span></span>

<span data-ttu-id="178ea-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="178ea-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

