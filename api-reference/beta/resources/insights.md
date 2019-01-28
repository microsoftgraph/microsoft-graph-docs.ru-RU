---
title: Тип ресурса officeGraphInsights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: daded26bff88d611ea39754d98007fa3329d142b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572460"
---
# <a name="insights-resource-type"></a><span data-ttu-id="ca6ce-104">Тип ресурса insights</span><span class="sxs-lookup"><span data-stu-id="ca6ce-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca6ce-105">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="ca6ce-106">К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="ca6ce-107">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="ca6ce-108">[Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="ca6ce-109">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="ca6ce-110">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="ca6ce-111">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="ca6ce-112">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="ca6ce-113">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="ca6ce-114">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="ca6ce-115">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="ca6ce-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ca6ce-116">Relationships</span></span>

| <span data-ttu-id="ca6ce-117">Связь</span><span class="sxs-lookup"><span data-stu-id="ca6ce-117">Relationship</span></span>      | <span data-ttu-id="ca6ce-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ca6ce-118">Type</span></span>          | <span data-ttu-id="ca6ce-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ca6ce-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="ca6ce-120">trending</span><span class="sxs-lookup"><span data-stu-id="ca6ce-120">Trending</span></span>      | <span data-ttu-id="ca6ce-121">Коллекция [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="ca6ce-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="ca6ce-122">Вычисляемая связь, определяющая популярные документы.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="ca6ce-123">Популярные документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="ca6ce-124">used</span><span class="sxs-lookup"><span data-stu-id="ca6ce-124">used</span></span>      | <span data-ttu-id="ca6ce-125">Коллекция [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="ca6ce-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="ca6ce-126">Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="ca6ce-127">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="ca6ce-128">shared</span><span class="sxs-lookup"><span data-stu-id="ca6ce-128">shared</span></span>        | <span data-ttu-id="ca6ce-129">Коллекция [shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="ca6ce-129">[shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="ca6ce-130">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="ca6ce-131">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="ca6ce-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca6ce-132">JSON representation</span></span>

<span data-ttu-id="ca6ce-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca6ce-133">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
