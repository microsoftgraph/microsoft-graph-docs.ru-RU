---
title: Тип ресурса insights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640170"
---
# <a name="insights-resource-type"></a><span data-ttu-id="cc2e7-104">Тип ресурса insights</span><span class="sxs-lookup"><span data-stu-id="cc2e7-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc2e7-105">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="cc2e7-106">К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="cc2e7-107">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="cc2e7-108">[Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="cc2e7-109">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="cc2e7-110">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="cc2e7-111">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="cc2e7-112">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="cc2e7-113">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="cc2e7-114">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="cc2e7-115">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="cc2e7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="cc2e7-116">Relationships</span></span>

| <span data-ttu-id="cc2e7-117">Связь</span><span class="sxs-lookup"><span data-stu-id="cc2e7-117">Relationship</span></span>      | <span data-ttu-id="cc2e7-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cc2e7-118">Type</span></span>          | <span data-ttu-id="cc2e7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2e7-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="cc2e7-120">trending</span><span class="sxs-lookup"><span data-stu-id="cc2e7-120">trending</span></span>      | <span data-ttu-id="cc2e7-121">Коллекция [Trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="cc2e7-121">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="cc2e7-122">Вычисляемая связь, определяющая популярные документы.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="cc2e7-123">Популярные документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="cc2e7-124">used</span><span class="sxs-lookup"><span data-stu-id="cc2e7-124">used</span></span>      | <span data-ttu-id="cc2e7-125">Коллекция [Used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="cc2e7-125">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="cc2e7-126">Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="cc2e7-127">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="cc2e7-128">shared</span><span class="sxs-lookup"><span data-stu-id="cc2e7-128">shared</span></span>        | <span data-ttu-id="cc2e7-129">Коллекция [Shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="cc2e7-129">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="cc2e7-130">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="cc2e7-131">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="cc2e7-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc2e7-132">JSON representation</span></span>

<span data-ttu-id="cc2e7-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc2e7-133">Here is a JSON representation of the resource</span></span>
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
