---
title: тенденции тип ресурса
description: Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.
ms.openlocfilehash: 7d240c4358047ca9ba3d6b8340fbfb7d893a6a1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078829"
---
# <a name="trending-resource-type"></a><span data-ttu-id="3de1c-104">тенденции тип ресурса</span><span class="sxs-lookup"><span data-stu-id="3de1c-104">trending resource type</span></span>

> <span data-ttu-id="3de1c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3de1c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3de1c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de1c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3de1c-107">Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя).</span><span class="sxs-lookup"><span data-stu-id="3de1c-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="3de1c-108">Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="3de1c-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="3de1c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3de1c-109">Methods</span></span>

| <span data-ttu-id="3de1c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3de1c-110">Method</span></span>       | <span data-ttu-id="3de1c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3de1c-111">Return Type</span></span>  |<span data-ttu-id="3de1c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3de1c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3de1c-113">Список подписок</span><span class="sxs-lookup"><span data-stu-id="3de1c-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="3de1c-114">[insights_trending](insights-trending.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3de1c-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="3de1c-115">Ознакомьтесь со списком тенденции файлы.</span><span class="sxs-lookup"><span data-stu-id="3de1c-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="3de1c-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3de1c-116">Properties</span></span>

| <span data-ttu-id="3de1c-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de1c-117">Property</span></span>      | <span data-ttu-id="3de1c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3de1c-118">Type</span></span>                              | <span data-ttu-id="3de1c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3de1c-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="3de1c-120">id</span><span class="sxs-lookup"><span data-stu-id="3de1c-120">id</span></span>                    | <span data-ttu-id="3de1c-121">String</span><span class="sxs-lookup"><span data-stu-id="3de1c-121">String</span></span>                    | <span data-ttu-id="3de1c-122">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="3de1c-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="3de1c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3de1c-123">Read only.</span></span>        |
| <span data-ttu-id="3de1c-124">weight</span><span class="sxs-lookup"><span data-stu-id="3de1c-124">weight</span></span>                | <span data-ttu-id="3de1c-125">Double</span><span class="sxs-lookup"><span data-stu-id="3de1c-125">Double</span></span>                    | <span data-ttu-id="3de1c-126">Значение, указывающее, какой объем документ в настоящее время прибора.</span><span class="sxs-lookup"><span data-stu-id="3de1c-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="3de1c-127">Чем больше число, тем больше документ — это в настоящее время прибора вокруг пользователя (более качественных это).</span><span class="sxs-lookup"><span data-stu-id="3de1c-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="3de1c-128">Возвращенный документы сортируются по это значение.</span><span class="sxs-lookup"><span data-stu-id="3de1c-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="3de1c-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="3de1c-129">resourceVisualization</span></span> | [<span data-ttu-id="3de1c-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="3de1c-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="3de1c-131">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="3de1c-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="3de1c-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="3de1c-132">resourceReference</span></span>     | [<span data-ttu-id="3de1c-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="3de1c-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="3de1c-134">Справочник по свойства тенденции документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="3de1c-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3de1c-135">Связи</span><span class="sxs-lookup"><span data-stu-id="3de1c-135">Relationships</span></span>

| <span data-ttu-id="3de1c-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de1c-136">Property</span></span>      | <span data-ttu-id="3de1c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="3de1c-137">Type</span></span>          | <span data-ttu-id="3de1c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3de1c-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="3de1c-139">resource</span><span class="sxs-lookup"><span data-stu-id="3de1c-139">resource</span></span>      | <span data-ttu-id="3de1c-140">Объект</span><span class="sxs-lookup"><span data-stu-id="3de1c-140">Entity</span></span>        | <span data-ttu-id="3de1c-141">Используется для перемещения по тенденции документа.</span><span class="sxs-lookup"><span data-stu-id="3de1c-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3de1c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3de1c-142">JSON representation</span></span>

<span data-ttu-id="3de1c-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de1c-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```