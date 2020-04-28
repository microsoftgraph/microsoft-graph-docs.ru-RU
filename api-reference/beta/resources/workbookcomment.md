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
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="51269-103">Тип ресурса Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="51269-103">workbookComment resource type</span></span>

<span data-ttu-id="51269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51269-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51269-105">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="51269-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="51269-106">Методы</span><span class="sxs-lookup"><span data-stu-id="51269-106">Methods</span></span>

| <span data-ttu-id="51269-107">Метод</span><span class="sxs-lookup"><span data-stu-id="51269-107">Method</span></span>       | <span data-ttu-id="51269-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51269-108">Return Type</span></span> | <span data-ttu-id="51269-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51269-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="51269-110">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="51269-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="51269-111">Коллекция [воркбуккоммент](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="51269-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="51269-112">Получение коллекции объектов **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="51269-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="51269-113">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="51269-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="51269-114">воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="51269-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="51269-115">Чтение свойств и связей объекта **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="51269-115">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="51269-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="51269-116">Properties</span></span>

| <span data-ttu-id="51269-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="51269-117">Property</span></span>     | <span data-ttu-id="51269-118">Тип</span><span class="sxs-lookup"><span data-stu-id="51269-118">Type</span></span>        | <span data-ttu-id="51269-119">Описание</span><span class="sxs-lookup"><span data-stu-id="51269-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51269-120">content</span><span class="sxs-lookup"><span data-stu-id="51269-120">content</span></span>|<span data-ttu-id="51269-121">String</span><span class="sxs-lookup"><span data-stu-id="51269-121">String</span></span>|<span data-ttu-id="51269-122">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="51269-122">The content of the comment.</span></span>|
|<span data-ttu-id="51269-123">contentType</span><span class="sxs-lookup"><span data-stu-id="51269-123">contentType</span></span>|<span data-ttu-id="51269-124">String</span><span class="sxs-lookup"><span data-stu-id="51269-124">String</span></span>|<span data-ttu-id="51269-125">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="51269-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="51269-126">id</span><span class="sxs-lookup"><span data-stu-id="51269-126">id</span></span>|<span data-ttu-id="51269-127">Строка</span><span class="sxs-lookup"><span data-stu-id="51269-127">String</span></span>| <span data-ttu-id="51269-128">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="51269-128">Represents the comment identifier.</span></span> <span data-ttu-id="51269-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51269-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51269-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="51269-130">Relationships</span></span>

| <span data-ttu-id="51269-131">Связь</span><span class="sxs-lookup"><span data-stu-id="51269-131">Relationship</span></span> | <span data-ttu-id="51269-132">Тип</span><span class="sxs-lookup"><span data-stu-id="51269-132">Type</span></span>        | <span data-ttu-id="51269-133">Описание</span><span class="sxs-lookup"><span data-stu-id="51269-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51269-134">отвечать</span><span class="sxs-lookup"><span data-stu-id="51269-134">replies</span></span>|<span data-ttu-id="51269-135">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="51269-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="51269-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="51269-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51269-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51269-138">JSON representation</span></span>

<span data-ttu-id="51269-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51269-139">The following is a JSON representation of the resource.</span></span>

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
