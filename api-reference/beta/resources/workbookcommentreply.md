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
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="f06e4-103">Тип ресурса Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="f06e4-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="f06e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f06e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f06e4-105">Представляет ответ на комментарий Excel.</span><span class="sxs-lookup"><span data-stu-id="f06e4-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="f06e4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f06e4-106">Methods</span></span>

| <span data-ttu-id="f06e4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f06e4-107">Method</span></span>       | <span data-ttu-id="f06e4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f06e4-108">Return Type</span></span> | <span data-ttu-id="f06e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f06e4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f06e4-110">Список Воркбуккомментреплиес</span><span class="sxs-lookup"><span data-stu-id="f06e4-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="f06e4-111">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="f06e4-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="f06e4-112">Получение списка объектов воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="f06e4-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="f06e4-113">Получение Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="f06e4-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="f06e4-114">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="f06e4-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="f06e4-115">Чтение свойств и связей объекта Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="f06e4-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="f06e4-116">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="f06e4-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="f06e4-117">воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="f06e4-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="f06e4-118">Создание нового Воркбуккомментрепли.</span><span class="sxs-lookup"><span data-stu-id="f06e4-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="f06e4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f06e4-119">Properties</span></span>

| <span data-ttu-id="f06e4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f06e4-120">Property</span></span>     | <span data-ttu-id="f06e4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f06e4-121">Type</span></span>        | <span data-ttu-id="f06e4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f06e4-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f06e4-123">content</span><span class="sxs-lookup"><span data-stu-id="f06e4-123">content</span></span>|<span data-ttu-id="f06e4-124">String</span><span class="sxs-lookup"><span data-stu-id="f06e4-124">String</span></span>|<span data-ttu-id="f06e4-125">Содержимое комментария, на который дан ответ.</span><span class="sxs-lookup"><span data-stu-id="f06e4-125">The content of replied comment.</span></span>|
|<span data-ttu-id="f06e4-126">contentType</span><span class="sxs-lookup"><span data-stu-id="f06e4-126">contentType</span></span>|<span data-ttu-id="f06e4-127">String</span><span class="sxs-lookup"><span data-stu-id="f06e4-127">String</span></span>|<span data-ttu-id="f06e4-128">Указывает тип комментария для ответа.</span><span class="sxs-lookup"><span data-stu-id="f06e4-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="f06e4-129">id</span><span class="sxs-lookup"><span data-stu-id="f06e4-129">id</span></span>|<span data-ttu-id="f06e4-130">Строка</span><span class="sxs-lookup"><span data-stu-id="f06e4-130">String</span></span>|<span data-ttu-id="f06e4-131">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="f06e4-131">Represents the comment identifier.</span></span> <span data-ttu-id="f06e4-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f06e4-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f06e4-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="f06e4-133">Relationships</span></span>

<span data-ttu-id="f06e4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="f06e4-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f06e4-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f06e4-135">JSON representation</span></span>

<span data-ttu-id="f06e4-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f06e4-136">The following is a JSON representation of the resource.</span></span>

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
