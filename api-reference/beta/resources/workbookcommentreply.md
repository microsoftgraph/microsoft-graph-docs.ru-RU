---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0a4dfc215eec435c67f1259a85e899db4dfb2b63
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775904"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="52ebb-103">Тип ресурса Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="52ebb-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="52ebb-104">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="52ebb-104">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="52ebb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="52ebb-105">Methods</span></span>

| <span data-ttu-id="52ebb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="52ebb-106">Method</span></span>       | <span data-ttu-id="52ebb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52ebb-107">Return Type</span></span> | <span data-ttu-id="52ebb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="52ebb-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52ebb-109">Список Воркбуккомментреплиес</span><span class="sxs-lookup"><span data-stu-id="52ebb-109">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="52ebb-110">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="52ebb-110">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="52ebb-111">Получение списка объектов воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="52ebb-111">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="52ebb-112">Получение Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="52ebb-112">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="52ebb-113">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="52ebb-113">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="52ebb-114">Чтение свойств и связей объекта Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="52ebb-114">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="52ebb-115">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="52ebb-115">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="52ebb-116">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="52ebb-116">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="52ebb-117">Создание нового Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="52ebb-117">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="52ebb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="52ebb-118">Properties</span></span>

| <span data-ttu-id="52ebb-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="52ebb-119">Property</span></span>     | <span data-ttu-id="52ebb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="52ebb-120">Type</span></span>        | <span data-ttu-id="52ebb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="52ebb-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52ebb-122">content</span><span class="sxs-lookup"><span data-stu-id="52ebb-122">content</span></span>|<span data-ttu-id="52ebb-123">String</span><span class="sxs-lookup"><span data-stu-id="52ebb-123">String</span></span>|<span data-ttu-id="52ebb-124">Содержимое комментария, на который дан ответ.</span><span class="sxs-lookup"><span data-stu-id="52ebb-124">The content of replied comment.</span></span>|
|<span data-ttu-id="52ebb-125">contentType</span><span class="sxs-lookup"><span data-stu-id="52ebb-125">contentType</span></span>|<span data-ttu-id="52ebb-126">String</span><span class="sxs-lookup"><span data-stu-id="52ebb-126">String</span></span>|<span data-ttu-id="52ebb-127">Указывает тип комментария для ответа.</span><span class="sxs-lookup"><span data-stu-id="52ebb-127">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="52ebb-128">id</span><span class="sxs-lookup"><span data-stu-id="52ebb-128">id</span></span>|<span data-ttu-id="52ebb-129">Строка</span><span class="sxs-lookup"><span data-stu-id="52ebb-129">String</span></span>|<span data-ttu-id="52ebb-130">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="52ebb-130">Represents the comment identifier.</span></span> <span data-ttu-id="52ebb-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52ebb-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ebb-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="52ebb-132">Relationships</span></span>

<span data-ttu-id="52ebb-133">Нет</span><span class="sxs-lookup"><span data-stu-id="52ebb-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52ebb-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52ebb-134">JSON representation</span></span>

<span data-ttu-id="52ebb-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52ebb-135">The following is a JSON representation of the resource.</span></span>

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
