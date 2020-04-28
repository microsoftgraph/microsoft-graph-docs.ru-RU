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
# <a name="trending-resource-type"></a><span data-ttu-id="02c1a-104">Тип ресурса трендов</span><span class="sxs-lookup"><span data-stu-id="02c1a-104">trending resource type</span></span>

<span data-ttu-id="02c1a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02c1a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c1a-106">Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя).</span><span class="sxs-lookup"><span data-stu-id="02c1a-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="02c1a-107">Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.</span><span class="sxs-lookup"><span data-stu-id="02c1a-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="02c1a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="02c1a-108">Methods</span></span>

| <span data-ttu-id="02c1a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="02c1a-109">Method</span></span>       | <span data-ttu-id="02c1a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="02c1a-110">Return Type</span></span>  |<span data-ttu-id="02c1a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02c1a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02c1a-112">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="02c1a-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="02c1a-113">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="02c1a-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="02c1a-114">Получение списка файлов трендов.</span><span class="sxs-lookup"><span data-stu-id="02c1a-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="02c1a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="02c1a-115">Properties</span></span>

| <span data-ttu-id="02c1a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c1a-116">Property</span></span>      | <span data-ttu-id="02c1a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="02c1a-117">Type</span></span>                              | <span data-ttu-id="02c1a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="02c1a-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="02c1a-119">id</span><span class="sxs-lookup"><span data-stu-id="02c1a-119">id</span></span>                    | <span data-ttu-id="02c1a-120">String</span><span class="sxs-lookup"><span data-stu-id="02c1a-120">String</span></span>                    | <span data-ttu-id="02c1a-121">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="02c1a-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="02c1a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02c1a-122">Read only.</span></span>        |
| <span data-ttu-id="02c1a-123">weight</span><span class="sxs-lookup"><span data-stu-id="02c1a-123">weight</span></span>                | <span data-ttu-id="02c1a-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="02c1a-124">Double</span></span>                    | <span data-ttu-id="02c1a-125">Значение, определяющее степень тенденции документа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="02c1a-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="02c1a-126">Чем больше это число, тем больше документ будет обходить пользователь (более релевантно).</span><span class="sxs-lookup"><span data-stu-id="02c1a-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="02c1a-127">Возвращенные документы сортируются по этому значению.</span><span class="sxs-lookup"><span data-stu-id="02c1a-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="02c1a-128">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="02c1a-128">resourceVisualization</span></span> | [<span data-ttu-id="02c1a-129">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="02c1a-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="02c1a-130">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="02c1a-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="02c1a-131">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="02c1a-131">resourceReference</span></span>     | [<span data-ttu-id="02c1a-132">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="02c1a-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="02c1a-133">Справочные свойства документа тенденций, такие как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="02c1a-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="02c1a-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02c1a-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="02c1a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02c1a-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="02c1a-136">Связи</span><span class="sxs-lookup"><span data-stu-id="02c1a-136">Relationships</span></span>

| <span data-ttu-id="02c1a-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c1a-137">Property</span></span>      | <span data-ttu-id="02c1a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="02c1a-138">Type</span></span>          | <span data-ttu-id="02c1a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="02c1a-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="02c1a-140">resource</span><span class="sxs-lookup"><span data-stu-id="02c1a-140">resource</span></span>      | <span data-ttu-id="02c1a-141">.</span><span class="sxs-lookup"><span data-stu-id="02c1a-141">entity</span></span>        | <span data-ttu-id="02c1a-142">Используется для навигации по документу трендов.</span><span class="sxs-lookup"><span data-stu-id="02c1a-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02c1a-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02c1a-143">JSON representation</span></span>

<span data-ttu-id="02c1a-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02c1a-144">Here is a JSON representation of the resource</span></span>

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
