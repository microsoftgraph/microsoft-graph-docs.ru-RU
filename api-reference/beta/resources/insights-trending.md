---
title: тенденции тип ресурса
description: Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640373"
---
# <a name="trending-resource-type"></a><span data-ttu-id="8b377-104">тенденции тип ресурса</span><span class="sxs-lookup"><span data-stu-id="8b377-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b377-105">Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя).</span><span class="sxs-lookup"><span data-stu-id="8b377-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="8b377-106">Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b377-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="8b377-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8b377-107">Methods</span></span>

| <span data-ttu-id="8b377-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8b377-108">Method</span></span>       | <span data-ttu-id="8b377-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8b377-109">Return Type</span></span>  |<span data-ttu-id="8b377-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b377-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b377-111">Список подписок</span><span class="sxs-lookup"><span data-stu-id="8b377-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="8b377-112">[insights_trending](insights-trending.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8b377-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="8b377-113">Ознакомьтесь со списком тенденции файлы.</span><span class="sxs-lookup"><span data-stu-id="8b377-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b377-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b377-114">Properties</span></span>

| <span data-ttu-id="8b377-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b377-115">Property</span></span>      | <span data-ttu-id="8b377-116">Тип</span><span class="sxs-lookup"><span data-stu-id="8b377-116">Type</span></span>                              | <span data-ttu-id="8b377-117">Описание</span><span class="sxs-lookup"><span data-stu-id="8b377-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="8b377-118">id</span><span class="sxs-lookup"><span data-stu-id="8b377-118">id</span></span>                    | <span data-ttu-id="8b377-119">String</span><span class="sxs-lookup"><span data-stu-id="8b377-119">String</span></span>                    | <span data-ttu-id="8b377-120">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="8b377-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="8b377-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b377-121">Read only.</span></span>        |
| <span data-ttu-id="8b377-122">weight</span><span class="sxs-lookup"><span data-stu-id="8b377-122">weight</span></span>                | <span data-ttu-id="8b377-123">Double</span><span class="sxs-lookup"><span data-stu-id="8b377-123">Double</span></span>                    | <span data-ttu-id="8b377-124">Значение, указывающее, какой объем документ в настоящее время прибора.</span><span class="sxs-lookup"><span data-stu-id="8b377-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="8b377-125">Чем больше число, тем больше документ — это в настоящее время прибора вокруг пользователя (более качественных это).</span><span class="sxs-lookup"><span data-stu-id="8b377-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="8b377-126">Возвращенный документы сортируются по это значение.</span><span class="sxs-lookup"><span data-stu-id="8b377-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="8b377-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="8b377-127">resourceVisualization</span></span> | [<span data-ttu-id="8b377-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="8b377-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="8b377-129">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="8b377-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="8b377-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="8b377-130">resourceReference</span></span>     | [<span data-ttu-id="8b377-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="8b377-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="8b377-132">Справочник по свойства тенденции документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="8b377-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8b377-133">Связи</span><span class="sxs-lookup"><span data-stu-id="8b377-133">Relationships</span></span>

| <span data-ttu-id="8b377-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b377-134">Property</span></span>      | <span data-ttu-id="8b377-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8b377-135">Type</span></span>          | <span data-ttu-id="8b377-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8b377-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="8b377-137">resource</span><span class="sxs-lookup"><span data-stu-id="8b377-137">resource</span></span>      | <span data-ttu-id="8b377-138">Entity</span><span class="sxs-lookup"><span data-stu-id="8b377-138">Entity</span></span>        | <span data-ttu-id="8b377-139">Используется для перемещения по тенденции документа.</span><span class="sxs-lookup"><span data-stu-id="8b377-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b377-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b377-140">JSON representation</span></span>

<span data-ttu-id="8b377-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b377-141">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
