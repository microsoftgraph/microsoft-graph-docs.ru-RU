---
title: Тип ресурса officeGraphInsights
description: Представляет базовый тип для itemInsights. officeGraphInsights предназначен для обратной совместимости с более ранними версиями API аналитики. Используйте только itemInsights при получении доступа к API аналитики.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ce1f51a3e0b53dc1ed108febf9a3b91055349ce5
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427328"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="da047-105">Тип ресурса officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="da047-105">officeGraphInsights resource type</span></span>

<span data-ttu-id="da047-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da047-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da047-107">Используйте [itemInsights](iteminsights.md) вместо **officeGraphInsights**, чтобы получить доступ к API аналитики.</span><span class="sxs-lookup"><span data-stu-id="da047-107">Use [itemInsights](iteminsights.md) in place of **officeGraphInsights** to access the insights API.</span></span>

<span data-ttu-id="da047-108">**officeGraphInsights** предназначен для обратной совместимости с более ранними версиями API аналитики.</span><span class="sxs-lookup"><span data-stu-id="da047-108">**officeGraphInsights** is for backward compatibility from earlier versions of the insights API.</span></span> <span data-ttu-id="da047-109">Это базовый тип для [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="da047-109">It is the base type for [itemInsights](iteminsights.md).</span></span>

<span data-ttu-id="da047-110">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="da047-110">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="da047-111">К примеру, вы можете выявить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="da047-111">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="da047-112">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="da047-112">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="da047-113">[Популярные](insights-trending.md) — возвращает документы из OneDrive для бизнеса и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="da047-113">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="da047-114">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="da047-114">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="da047-115">Включает документы, использованные пользователем в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="da047-115">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="da047-116">[Общие](insights-shared.md) — возвращает документы, к которым пользователю или пользователем предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="da047-116">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="da047-117">Общий доступ к документам можно предоставлять в виде по URL-ссылок, вложенных файлов, справочных вложений в OneDrive для бизнеса и файлам SharePoint, которые есть в сообщениях и собраниях Outlook.</span><span class="sxs-lookup"><span data-stu-id="da047-117">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="da047-118">Каждый объект аналитики возвращается со значением сложного типа (CVT) **resourceVisualization** и **resourceReference** сложного типа значений.</span><span class="sxs-lookup"><span data-stu-id="da047-118">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="da047-119">Сложный тип значений **resourceVisualization** содержит такие свойства, как **title** и **previewImageUrl**.</span><span class="sxs-lookup"><span data-stu-id="da047-119">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="da047-120">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="da047-120">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="da047-121">Связи</span><span class="sxs-lookup"><span data-stu-id="da047-121">Relationships</span></span>

| <span data-ttu-id="da047-122">Связь</span><span class="sxs-lookup"><span data-stu-id="da047-122">Relationship</span></span>      | <span data-ttu-id="da047-123">Тип</span><span class="sxs-lookup"><span data-stu-id="da047-123">Type</span></span>          | <span data-ttu-id="da047-124">Описание</span><span class="sxs-lookup"><span data-stu-id="da047-124">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="da047-125">trending</span><span class="sxs-lookup"><span data-stu-id="da047-125">trending</span></span>      | <span data-ttu-id="da047-126">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="da047-126">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="da047-127">Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="da047-127">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="da047-128">used</span><span class="sxs-lookup"><span data-stu-id="da047-128">used</span></span>      | <span data-ttu-id="da047-129">Коллекция объектов [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="da047-129">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="da047-130">Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="da047-130">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="da047-131">общие</span><span class="sxs-lookup"><span data-stu-id="da047-131">shared</span></span>        | <span data-ttu-id="da047-132">Коллекция объектов [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="da047-132">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="da047-133">Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="da047-133">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="da047-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da047-134">JSON representation</span></span>

<span data-ttu-id="da047-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da047-135">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```

