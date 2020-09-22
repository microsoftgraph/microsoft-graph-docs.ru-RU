---
title: Тип ресурса трендов
description: Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7a9c9cf9323aa24bd50c1f817a1293088e1a4373
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054772"
---
# <a name="trending-resource-type"></a><span data-ttu-id="c7d2e-104">Тип ресурса трендов</span><span class="sxs-lookup"><span data-stu-id="c7d2e-104">trending resource type</span></span>

<span data-ttu-id="c7d2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d2e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7d2e-106">Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя).</span><span class="sxs-lookup"><span data-stu-id="c7d2e-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="c7d2e-107">Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c7d2e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c7d2e-108">Methods</span></span>

| <span data-ttu-id="c7d2e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c7d2e-109">Method</span></span>       | <span data-ttu-id="c7d2e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7d2e-110">Return Type</span></span>  |<span data-ttu-id="c7d2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d2e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7d2e-112">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="c7d2e-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="c7d2e-113">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="c7d2e-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="c7d2e-114">Получение списка файлов трендов.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7d2e-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7d2e-115">Properties</span></span>

| <span data-ttu-id="c7d2e-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7d2e-116">Property</span></span>      | <span data-ttu-id="c7d2e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c7d2e-117">Type</span></span>                              | <span data-ttu-id="c7d2e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d2e-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="c7d2e-119">id</span><span class="sxs-lookup"><span data-stu-id="c7d2e-119">id</span></span>                    | <span data-ttu-id="c7d2e-120">String</span><span class="sxs-lookup"><span data-stu-id="c7d2e-120">String</span></span>                    | <span data-ttu-id="c7d2e-121">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="c7d2e-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-122">Read only.</span></span>        |
| <span data-ttu-id="c7d2e-123">weight</span><span class="sxs-lookup"><span data-stu-id="c7d2e-123">weight</span></span>                | <span data-ttu-id="c7d2e-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="c7d2e-124">Double</span></span>                    | <span data-ttu-id="c7d2e-125">Значение, определяющее степень тенденции документа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="c7d2e-126">Чем больше это число, тем больше документ будет обходить пользователь (более релевантно).</span><span class="sxs-lookup"><span data-stu-id="c7d2e-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="c7d2e-127">Возвращенные документы сортируются по этому значению.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="c7d2e-128">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="c7d2e-128">resourceVisualization</span></span> | [<span data-ttu-id="c7d2e-129">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="c7d2e-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="c7d2e-130">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="c7d2e-131">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="c7d2e-131">resourceReference</span></span>     | [<span data-ttu-id="c7d2e-132">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="c7d2e-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="c7d2e-133">Справочные свойства документа тенденций, такие как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="c7d2e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d2e-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="c7d2e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d2e-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="c7d2e-136">Связи</span><span class="sxs-lookup"><span data-stu-id="c7d2e-136">Relationships</span></span>

| <span data-ttu-id="c7d2e-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7d2e-137">Property</span></span>      | <span data-ttu-id="c7d2e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c7d2e-138">Type</span></span>          | <span data-ttu-id="c7d2e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d2e-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="c7d2e-140">resource</span><span class="sxs-lookup"><span data-stu-id="c7d2e-140">resource</span></span>      | <span data-ttu-id="c7d2e-141">.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-141">entity</span></span>        | <span data-ttu-id="c7d2e-142">Используется для навигации по документу трендов.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7d2e-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7d2e-143">JSON representation</span></span>

<span data-ttu-id="c7d2e-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7d2e-144">Here is a JSON representation of the resource</span></span>

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

