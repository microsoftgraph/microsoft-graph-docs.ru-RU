---
title: Тип ресурса officeGraphInsights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 807cb786577b9c9ddd512d9dcce9a03517170f5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966519"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="6672b-104">Тип ресурса officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="6672b-104">officeGraphInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6672b-105">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="6672b-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="6672b-106">К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="6672b-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="6672b-107">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="6672b-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="6672b-108">[Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="6672b-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="6672b-109">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="6672b-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="6672b-110">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="6672b-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="6672b-111">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="6672b-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="6672b-112">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6672b-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="6672b-113">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="6672b-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="6672b-114">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="6672b-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="6672b-115">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="6672b-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="6672b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="6672b-116">Relationships</span></span>

| <span data-ttu-id="6672b-117">Отношение</span><span class="sxs-lookup"><span data-stu-id="6672b-117">Relationship</span></span>      | <span data-ttu-id="6672b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6672b-118">Type</span></span>          | <span data-ttu-id="6672b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6672b-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="6672b-120">trending</span><span class="sxs-lookup"><span data-stu-id="6672b-120">trending</span></span>      | <span data-ttu-id="6672b-121">Коллекция [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="6672b-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="6672b-122">Вычисляемая связь, определяющая популярные документы.</span><span class="sxs-lookup"><span data-stu-id="6672b-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="6672b-123">Популярные документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6672b-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="6672b-124">used</span><span class="sxs-lookup"><span data-stu-id="6672b-124">used</span></span>      | <span data-ttu-id="6672b-125">Коллекция [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="6672b-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="6672b-126">Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="6672b-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="6672b-127">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="6672b-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="6672b-128">общие</span><span class="sxs-lookup"><span data-stu-id="6672b-128">shared</span></span>        | <span data-ttu-id="6672b-129">Коллекция [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="6672b-129">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="6672b-130">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="6672b-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="6672b-131">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6672b-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="6672b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6672b-132">JSON representation</span></span>

<span data-ttu-id="6672b-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6672b-133">Here is a JSON representation of the resource</span></span>
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
