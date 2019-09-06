---
title: Тип ресурса Воркбуккоммент
description: Определение типа ресурса Воркбуккоммент
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2f081dd5bf3732b104ab20a28df0f61956b8490
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775757"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="a3186-103">Тип ресурса Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="a3186-103">workbookComment resource type</span></span>

<span data-ttu-id="a3186-104">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="a3186-104">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="a3186-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a3186-105">Methods</span></span>

| <span data-ttu-id="a3186-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a3186-106">Method</span></span>       | <span data-ttu-id="a3186-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3186-107">Return Type</span></span> | <span data-ttu-id="a3186-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a3186-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a3186-109">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="a3186-109">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="a3186-110">Коллекция [воркбуккоммент](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="a3186-110">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="a3186-111">Получение коллекции объектов **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="a3186-111">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="a3186-112">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="a3186-112">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="a3186-113">воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="a3186-113">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="a3186-114">Чтение свойств и связей объекта **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="a3186-114">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3186-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3186-115">Properties</span></span>

| <span data-ttu-id="a3186-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3186-116">Property</span></span>     | <span data-ttu-id="a3186-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a3186-117">Type</span></span>        | <span data-ttu-id="a3186-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a3186-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3186-119">content</span><span class="sxs-lookup"><span data-stu-id="a3186-119">content</span></span>|<span data-ttu-id="a3186-120">String</span><span class="sxs-lookup"><span data-stu-id="a3186-120">String</span></span>|<span data-ttu-id="a3186-121">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="a3186-121">The content of comment.</span></span>|
|<span data-ttu-id="a3186-122">contentType</span><span class="sxs-lookup"><span data-stu-id="a3186-122">contentType</span></span>|<span data-ttu-id="a3186-123">String</span><span class="sxs-lookup"><span data-stu-id="a3186-123">String</span></span>|<span data-ttu-id="a3186-124">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="a3186-124">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="a3186-125">id</span><span class="sxs-lookup"><span data-stu-id="a3186-125">id</span></span>|<span data-ttu-id="a3186-126">Строка</span><span class="sxs-lookup"><span data-stu-id="a3186-126">String</span></span>| <span data-ttu-id="a3186-127">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="a3186-127">Represents the comment identifier.</span></span> <span data-ttu-id="a3186-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3186-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3186-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="a3186-129">Relationships</span></span>

| <span data-ttu-id="a3186-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="a3186-130">Relationship</span></span> | <span data-ttu-id="a3186-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3186-131">Type</span></span>        | <span data-ttu-id="a3186-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3186-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3186-133">replies</span><span class="sxs-lookup"><span data-stu-id="a3186-133">replies</span></span>|<span data-ttu-id="a3186-134">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="a3186-134">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="a3186-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a3186-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3186-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3186-137">JSON representation</span></span>

<span data-ttu-id="a3186-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3186-138">The following is a JSON representation of the resource.</span></span>

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
