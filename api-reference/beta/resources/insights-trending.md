---
title: Тип ресурса трендов
description: Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551311"
---
# <a name="trending-resource-type"></a><span data-ttu-id="cb26c-104">Тип ресурса трендов</span><span class="sxs-lookup"><span data-stu-id="cb26c-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb26c-105">Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя).</span><span class="sxs-lookup"><span data-stu-id="cb26c-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="cb26c-106">Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb26c-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cb26c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cb26c-107">Methods</span></span>

| <span data-ttu-id="cb26c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cb26c-108">Method</span></span>       | <span data-ttu-id="cb26c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb26c-109">Return Type</span></span>  |<span data-ttu-id="cb26c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cb26c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb26c-111">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="cb26c-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="cb26c-112">Коллекция [инсигхтс_трендинг](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="cb26c-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="cb26c-113">Получение списка файлов трендов.</span><span class="sxs-lookup"><span data-stu-id="cb26c-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb26c-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb26c-114">Properties</span></span>

| <span data-ttu-id="cb26c-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb26c-115">Property</span></span>      | <span data-ttu-id="cb26c-116">Тип</span><span class="sxs-lookup"><span data-stu-id="cb26c-116">Type</span></span>                              | <span data-ttu-id="cb26c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cb26c-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="cb26c-118">id</span><span class="sxs-lookup"><span data-stu-id="cb26c-118">id</span></span>                    | <span data-ttu-id="cb26c-119">String</span><span class="sxs-lookup"><span data-stu-id="cb26c-119">String</span></span>                    | <span data-ttu-id="cb26c-120">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="cb26c-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="cb26c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb26c-121">Read only.</span></span>        |
| <span data-ttu-id="cb26c-122">weight</span><span class="sxs-lookup"><span data-stu-id="cb26c-122">weight</span></span>                | <span data-ttu-id="cb26c-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="cb26c-123">Double</span></span>                    | <span data-ttu-id="cb26c-124">Значение, определяющее степень тенденции документа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="cb26c-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="cb26c-125">Чем больше это число, тем больше документ будет обходить пользователь (более релевантно).</span><span class="sxs-lookup"><span data-stu-id="cb26c-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="cb26c-126">Возвращенные документы сортируются по этому значению.</span><span class="sxs-lookup"><span data-stu-id="cb26c-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="cb26c-127">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="cb26c-127">resourceVisualization</span></span> | [<span data-ttu-id="cb26c-128">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="cb26c-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="cb26c-129">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="cb26c-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="cb26c-130">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="cb26c-130">resourceReference</span></span>     | [<span data-ttu-id="cb26c-131">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="cb26c-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="cb26c-132">Справочные свойства документа тенденций, такие как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="cb26c-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cb26c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="cb26c-133">Relationships</span></span>

| <span data-ttu-id="cb26c-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb26c-134">Property</span></span>      | <span data-ttu-id="cb26c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="cb26c-135">Type</span></span>          | <span data-ttu-id="cb26c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="cb26c-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="cb26c-137">resource</span><span class="sxs-lookup"><span data-stu-id="cb26c-137">resource</span></span>      | <span data-ttu-id="cb26c-138">Объект</span><span class="sxs-lookup"><span data-stu-id="cb26c-138">Entity</span></span>        | <span data-ttu-id="cb26c-139">Используется для навигации по документу трендов.</span><span class="sxs-lookup"><span data-stu-id="cb26c-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb26c-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb26c-140">JSON representation</span></span>

<span data-ttu-id="cb26c-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb26c-141">Here is a JSON representation of the resource</span></span>

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
