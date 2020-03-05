---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d080f283401d9486de53095d3ad25029edbb14b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519241"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="d7e03-103">Тип ресурса Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="d7e03-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="d7e03-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7e03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7e03-105">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="d7e03-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="d7e03-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d7e03-106">Methods</span></span>

| <span data-ttu-id="d7e03-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d7e03-107">Method</span></span>       | <span data-ttu-id="d7e03-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d7e03-108">Return Type</span></span> | <span data-ttu-id="d7e03-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e03-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d7e03-110">Список Воркбуккомментреплиес</span><span class="sxs-lookup"><span data-stu-id="d7e03-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="d7e03-111">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="d7e03-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="d7e03-112">Получение списка объектов воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="d7e03-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="d7e03-113">Получение Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="d7e03-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="d7e03-114">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="d7e03-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d7e03-115">Чтение свойств и связей объекта Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="d7e03-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="d7e03-116">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="d7e03-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="d7e03-117">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="d7e03-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d7e03-118">Создание нового Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="d7e03-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7e03-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7e03-119">Properties</span></span>

| <span data-ttu-id="d7e03-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7e03-120">Property</span></span>     | <span data-ttu-id="d7e03-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d7e03-121">Type</span></span>        | <span data-ttu-id="d7e03-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e03-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7e03-123">content</span><span class="sxs-lookup"><span data-stu-id="d7e03-123">content</span></span>|<span data-ttu-id="d7e03-124">String</span><span class="sxs-lookup"><span data-stu-id="d7e03-124">String</span></span>|<span data-ttu-id="d7e03-125">Содержимое комментария, на который дан ответ.</span><span class="sxs-lookup"><span data-stu-id="d7e03-125">The content of replied comment.</span></span>|
|<span data-ttu-id="d7e03-126">contentType</span><span class="sxs-lookup"><span data-stu-id="d7e03-126">contentType</span></span>|<span data-ttu-id="d7e03-127">String</span><span class="sxs-lookup"><span data-stu-id="d7e03-127">String</span></span>|<span data-ttu-id="d7e03-128">Указывает тип комментария для ответа.</span><span class="sxs-lookup"><span data-stu-id="d7e03-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="d7e03-129">id</span><span class="sxs-lookup"><span data-stu-id="d7e03-129">id</span></span>|<span data-ttu-id="d7e03-130">Строка</span><span class="sxs-lookup"><span data-stu-id="d7e03-130">String</span></span>|<span data-ttu-id="d7e03-131">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="d7e03-131">Represents the comment identifier.</span></span> <span data-ttu-id="d7e03-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7e03-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7e03-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7e03-133">Relationships</span></span>

<span data-ttu-id="d7e03-134">Нет</span><span class="sxs-lookup"><span data-stu-id="d7e03-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7e03-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7e03-135">JSON representation</span></span>

<span data-ttu-id="d7e03-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7e03-136">The following is a JSON representation of the resource.</span></span>

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
