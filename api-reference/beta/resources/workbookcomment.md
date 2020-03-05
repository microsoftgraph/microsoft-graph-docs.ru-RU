---
title: Тип ресурса Воркбуккоммент
description: Представляет комментарий в книге.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c2165f43c04ebbaf3274cc0ae912756bf250785a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519248"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="d42fe-103">Тип ресурса Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d42fe-103">workbookComment resource type</span></span>

<span data-ttu-id="d42fe-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d42fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d42fe-105">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="d42fe-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="d42fe-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d42fe-106">Methods</span></span>

| <span data-ttu-id="d42fe-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d42fe-107">Method</span></span>       | <span data-ttu-id="d42fe-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d42fe-108">Return Type</span></span> | <span data-ttu-id="d42fe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d42fe-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d42fe-110">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="d42fe-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="d42fe-111">Коллекция [воркбуккоммент](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="d42fe-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="d42fe-112">Получение коллекции объектов **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="d42fe-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="d42fe-113">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d42fe-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="d42fe-114">воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="d42fe-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="d42fe-115">Чтение свойств и связей объекта **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="d42fe-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="d42fe-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d42fe-116">Properties</span></span>

| <span data-ttu-id="d42fe-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d42fe-117">Property</span></span>     | <span data-ttu-id="d42fe-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d42fe-118">Type</span></span>        | <span data-ttu-id="d42fe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d42fe-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d42fe-120">content</span><span class="sxs-lookup"><span data-stu-id="d42fe-120">content</span></span>|<span data-ttu-id="d42fe-121">String</span><span class="sxs-lookup"><span data-stu-id="d42fe-121">String</span></span>|<span data-ttu-id="d42fe-122">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="d42fe-122">The content of the comment.</span></span>|
|<span data-ttu-id="d42fe-123">contentType</span><span class="sxs-lookup"><span data-stu-id="d42fe-123">contentType</span></span>|<span data-ttu-id="d42fe-124">String</span><span class="sxs-lookup"><span data-stu-id="d42fe-124">String</span></span>|<span data-ttu-id="d42fe-125">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="d42fe-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="d42fe-126">id</span><span class="sxs-lookup"><span data-stu-id="d42fe-126">id</span></span>|<span data-ttu-id="d42fe-127">Строка</span><span class="sxs-lookup"><span data-stu-id="d42fe-127">String</span></span>| <span data-ttu-id="d42fe-128">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="d42fe-128">Represents the comment identifier.</span></span> <span data-ttu-id="d42fe-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d42fe-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d42fe-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="d42fe-130">Relationships</span></span>

| <span data-ttu-id="d42fe-131">Связь</span><span class="sxs-lookup"><span data-stu-id="d42fe-131">Relationship</span></span> | <span data-ttu-id="d42fe-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d42fe-132">Type</span></span>        | <span data-ttu-id="d42fe-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d42fe-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d42fe-134">отвечать</span><span class="sxs-lookup"><span data-stu-id="d42fe-134">replies</span></span>|<span data-ttu-id="d42fe-135">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="d42fe-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="d42fe-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d42fe-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d42fe-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d42fe-138">JSON representation</span></span>

<span data-ttu-id="d42fe-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d42fe-139">The following is a JSON representation of the resource.</span></span>

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
