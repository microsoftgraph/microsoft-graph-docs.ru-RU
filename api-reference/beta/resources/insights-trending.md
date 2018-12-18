---
title: тенденции тип ресурса
description: Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.
author: simonhult
ms.openlocfilehash: ae3c3a876dba6c22a629cce5db8e5b4baa5fb5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348001"
---
# <a name="trending-resource-type"></a><span data-ttu-id="ce0be-104">тенденции тип ресурса</span><span class="sxs-lookup"><span data-stu-id="ce0be-104">trending resource type</span></span>

> <span data-ttu-id="ce0be-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce0be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce0be-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce0be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce0be-107">Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя).</span><span class="sxs-lookup"><span data-stu-id="ce0be-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="ce0be-108">Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce0be-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="ce0be-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ce0be-109">Methods</span></span>

| <span data-ttu-id="ce0be-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ce0be-110">Method</span></span>       | <span data-ttu-id="ce0be-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce0be-111">Return Type</span></span>  |<span data-ttu-id="ce0be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0be-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce0be-113">Список подписок</span><span class="sxs-lookup"><span data-stu-id="ce0be-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="ce0be-114">[insights_trending](insights-trending.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ce0be-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="ce0be-115">Ознакомьтесь со списком тенденции файлы.</span><span class="sxs-lookup"><span data-stu-id="ce0be-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce0be-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce0be-116">Properties</span></span>

| <span data-ttu-id="ce0be-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce0be-117">Property</span></span>      | <span data-ttu-id="ce0be-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ce0be-118">Type</span></span>                              | <span data-ttu-id="ce0be-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0be-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="ce0be-120">id</span><span class="sxs-lookup"><span data-stu-id="ce0be-120">id</span></span>                    | <span data-ttu-id="ce0be-121">Строка</span><span class="sxs-lookup"><span data-stu-id="ce0be-121">String</span></span>                    | <span data-ttu-id="ce0be-122">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="ce0be-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="ce0be-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce0be-123">Read only.</span></span>        |
| <span data-ttu-id="ce0be-124">weight</span><span class="sxs-lookup"><span data-stu-id="ce0be-124">weight</span></span>                | <span data-ttu-id="ce0be-125">Double</span><span class="sxs-lookup"><span data-stu-id="ce0be-125">Double</span></span>                    | <span data-ttu-id="ce0be-126">Значение, указывающее, какой объем документ в настоящее время прибора.</span><span class="sxs-lookup"><span data-stu-id="ce0be-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="ce0be-127">Чем больше число, тем больше документ — это в настоящее время прибора вокруг пользователя (более качественных это).</span><span class="sxs-lookup"><span data-stu-id="ce0be-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="ce0be-128">Возвращенный документы сортируются по это значение.</span><span class="sxs-lookup"><span data-stu-id="ce0be-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="ce0be-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ce0be-129">resourceVisualization</span></span> | [<span data-ttu-id="ce0be-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ce0be-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="ce0be-131">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="ce0be-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="ce0be-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ce0be-132">resourceReference</span></span>     | [<span data-ttu-id="ce0be-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ce0be-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="ce0be-134">Справочник по свойства тенденции документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="ce0be-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce0be-135">Связи</span><span class="sxs-lookup"><span data-stu-id="ce0be-135">Relationships</span></span>

| <span data-ttu-id="ce0be-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce0be-136">Property</span></span>      | <span data-ttu-id="ce0be-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ce0be-137">Type</span></span>          | <span data-ttu-id="ce0be-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0be-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="ce0be-139">resource</span><span class="sxs-lookup"><span data-stu-id="ce0be-139">resource</span></span>      | <span data-ttu-id="ce0be-140">Entity</span><span class="sxs-lookup"><span data-stu-id="ce0be-140">Entity</span></span>        | <span data-ttu-id="ce0be-141">Используется для перемещения по тенденции документа.</span><span class="sxs-lookup"><span data-stu-id="ce0be-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce0be-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce0be-142">JSON representation</span></span>

<span data-ttu-id="ce0be-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce0be-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```