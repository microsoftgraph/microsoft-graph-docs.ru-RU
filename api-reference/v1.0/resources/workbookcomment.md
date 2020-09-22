---
title: Тип ресурса Воркбуккоммент
description: Определение типа ресурса Воркбуккоммент
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b89f7b1ed2ca1ca833d8d5bae72d74a58b714997
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015171"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="6e55a-103">Тип ресурса Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="6e55a-103">workbookComment resource type</span></span>

<span data-ttu-id="6e55a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e55a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e55a-105">Представляет комментарий в книге.</span><span class="sxs-lookup"><span data-stu-id="6e55a-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="6e55a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6e55a-106">Methods</span></span>

| <span data-ttu-id="6e55a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6e55a-107">Method</span></span>       | <span data-ttu-id="6e55a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e55a-108">Return Type</span></span> | <span data-ttu-id="6e55a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e55a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6e55a-110">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="6e55a-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="6e55a-111">Коллекция [воркбуккоммент](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="6e55a-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="6e55a-112">Получение коллекции объектов **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="6e55a-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="6e55a-113">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="6e55a-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="6e55a-114">воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="6e55a-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="6e55a-115">Чтение свойств и связей объекта **воркбуккоммент** .</span><span class="sxs-lookup"><span data-stu-id="6e55a-115">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6e55a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e55a-116">Properties</span></span>

| <span data-ttu-id="6e55a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e55a-117">Property</span></span>     | <span data-ttu-id="6e55a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6e55a-118">Type</span></span>        | <span data-ttu-id="6e55a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6e55a-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e55a-120">content</span><span class="sxs-lookup"><span data-stu-id="6e55a-120">content</span></span>|<span data-ttu-id="6e55a-121">String</span><span class="sxs-lookup"><span data-stu-id="6e55a-121">String</span></span>|<span data-ttu-id="6e55a-122">Содержимое комментария.</span><span class="sxs-lookup"><span data-stu-id="6e55a-122">The content of comment.</span></span>|
|<span data-ttu-id="6e55a-123">contentType</span><span class="sxs-lookup"><span data-stu-id="6e55a-123">contentType</span></span>|<span data-ttu-id="6e55a-124">String</span><span class="sxs-lookup"><span data-stu-id="6e55a-124">String</span></span>|<span data-ttu-id="6e55a-125">Указывает тип комментария.</span><span class="sxs-lookup"><span data-stu-id="6e55a-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="6e55a-126">id</span><span class="sxs-lookup"><span data-stu-id="6e55a-126">id</span></span>|<span data-ttu-id="6e55a-127">String</span><span class="sxs-lookup"><span data-stu-id="6e55a-127">String</span></span>| <span data-ttu-id="6e55a-128">Представляет идентификатор примечания.</span><span class="sxs-lookup"><span data-stu-id="6e55a-128">Represents the comment identifier.</span></span> <span data-ttu-id="6e55a-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e55a-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e55a-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e55a-130">Relationships</span></span>

| <span data-ttu-id="6e55a-131">Связь</span><span class="sxs-lookup"><span data-stu-id="6e55a-131">Relationship</span></span> | <span data-ttu-id="6e55a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6e55a-132">Type</span></span>        | <span data-ttu-id="6e55a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6e55a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e55a-134">отвечать</span><span class="sxs-lookup"><span data-stu-id="6e55a-134">replies</span></span>|<span data-ttu-id="6e55a-135">Коллекция [воркбуккомментрепли](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="6e55a-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="6e55a-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e55a-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e55a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e55a-138">JSON representation</span></span>

<span data-ttu-id="6e55a-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e55a-139">The following is a JSON representation of the resource.</span></span>

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

