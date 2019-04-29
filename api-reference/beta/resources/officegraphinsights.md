---
title: Тип ресурса officeGraphInsights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 8a07cd10622886ad6e367d5311e750454e7bf90b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348972"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="66c49-104">Тип ресурса officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="66c49-104">officeGraphInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66c49-105">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="66c49-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="66c49-106">К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="66c49-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="66c49-107">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="66c49-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="66c49-108">[Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="66c49-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="66c49-109">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="66c49-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="66c49-110">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="66c49-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="66c49-111">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="66c49-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="66c49-112">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="66c49-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="66c49-113">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="66c49-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="66c49-114">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="66c49-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="66c49-115">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="66c49-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="66c49-116">Связи</span><span class="sxs-lookup"><span data-stu-id="66c49-116">Relationships</span></span>

| <span data-ttu-id="66c49-117">Отношение</span><span class="sxs-lookup"><span data-stu-id="66c49-117">Relationship</span></span>      | <span data-ttu-id="66c49-118">Тип</span><span class="sxs-lookup"><span data-stu-id="66c49-118">Type</span></span>          | <span data-ttu-id="66c49-119">Описание</span><span class="sxs-lookup"><span data-stu-id="66c49-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="66c49-120">trending</span><span class="sxs-lookup"><span data-stu-id="66c49-120">trending</span></span>      | <span data-ttu-id="66c49-121">Коллекция [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="66c49-121">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="66c49-122">Вычисляемая связь, определяющая популярные документы.</span><span class="sxs-lookup"><span data-stu-id="66c49-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="66c49-123">Популярные документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="66c49-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="66c49-124">used</span><span class="sxs-lookup"><span data-stu-id="66c49-124">used</span></span>      | <span data-ttu-id="66c49-125">Коллекция [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="66c49-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="66c49-126">Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="66c49-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="66c49-127">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="66c49-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="66c49-128">общие</span><span class="sxs-lookup"><span data-stu-id="66c49-128">shared</span></span>        | <span data-ttu-id="66c49-129">Коллекция [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="66c49-129">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="66c49-130">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="66c49-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="66c49-131">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="66c49-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="66c49-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66c49-132">JSON representation</span></span>

<span data-ttu-id="66c49-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66c49-133">Here is a JSON representation of the resource</span></span>
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
