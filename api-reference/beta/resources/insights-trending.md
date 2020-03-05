---
title: Тип ресурса трендов
description: Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c6fe9f81b9474ca8d1a4c2aeeb3fcc449499c82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495538"
---
# <a name="trending-resource-type"></a><span data-ttu-id="b83e4-104">Тип ресурса трендов</span><span class="sxs-lookup"><span data-stu-id="b83e4-104">trending resource type</span></span>

<span data-ttu-id="b83e4-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b83e4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b83e4-106">Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя).</span><span class="sxs-lookup"><span data-stu-id="b83e4-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="b83e4-107">Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.</span><span class="sxs-lookup"><span data-stu-id="b83e4-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="b83e4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b83e4-108">Methods</span></span>

| <span data-ttu-id="b83e4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b83e4-109">Method</span></span>       | <span data-ttu-id="b83e4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b83e4-110">Return Type</span></span>  |<span data-ttu-id="b83e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b83e4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b83e4-112">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="b83e4-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="b83e4-113">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="b83e4-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="b83e4-114">Получение списка файлов трендов.</span><span class="sxs-lookup"><span data-stu-id="b83e4-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="b83e4-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="b83e4-115">Properties</span></span>

| <span data-ttu-id="b83e4-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="b83e4-116">Property</span></span>      | <span data-ttu-id="b83e4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b83e4-117">Type</span></span>                              | <span data-ttu-id="b83e4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b83e4-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="b83e4-119">id</span><span class="sxs-lookup"><span data-stu-id="b83e4-119">id</span></span>                    | <span data-ttu-id="b83e4-120">String</span><span class="sxs-lookup"><span data-stu-id="b83e4-120">String</span></span>                    | <span data-ttu-id="b83e4-121">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="b83e4-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="b83e4-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b83e4-122">Read only.</span></span>        |
| <span data-ttu-id="b83e4-123">weight</span><span class="sxs-lookup"><span data-stu-id="b83e4-123">weight</span></span>                | <span data-ttu-id="b83e4-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b83e4-124">Double</span></span>                    | <span data-ttu-id="b83e4-125">Значение, определяющее степень тенденции документа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="b83e4-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="b83e4-126">Чем больше это число, тем больше документ будет обходить пользователь (более релевантно).</span><span class="sxs-lookup"><span data-stu-id="b83e4-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="b83e4-127">Возвращенные документы сортируются по этому значению.</span><span class="sxs-lookup"><span data-stu-id="b83e4-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="b83e4-128">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="b83e4-128">resourceVisualization</span></span> | [<span data-ttu-id="b83e4-129">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="b83e4-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="b83e4-130">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="b83e4-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="b83e4-131">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b83e4-131">resourceReference</span></span>     | [<span data-ttu-id="b83e4-132">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b83e4-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="b83e4-133">Справочные свойства документа тенденций, такие как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="b83e4-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="b83e4-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b83e4-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="b83e4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b83e4-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="b83e4-136">Связи</span><span class="sxs-lookup"><span data-stu-id="b83e4-136">Relationships</span></span>

| <span data-ttu-id="b83e4-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="b83e4-137">Property</span></span>      | <span data-ttu-id="b83e4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="b83e4-138">Type</span></span>          | <span data-ttu-id="b83e4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b83e4-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="b83e4-140">resource</span><span class="sxs-lookup"><span data-stu-id="b83e4-140">resource</span></span>      | <span data-ttu-id="b83e4-141">.</span><span class="sxs-lookup"><span data-stu-id="b83e4-141">entity</span></span>        | <span data-ttu-id="b83e4-142">Используется для навигации по документу трендов.</span><span class="sxs-lookup"><span data-stu-id="b83e4-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b83e4-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b83e4-143">JSON representation</span></span>

<span data-ttu-id="b83e4-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b83e4-144">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```
