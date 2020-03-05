---
title: Тип ресурса officeGraphInsights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8ac5019909a2f5ebe808be695ed7d516738c21e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447341"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="dca0a-104">Тип ресурса officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="dca0a-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="dca0a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca0a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dca0a-106">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="dca0a-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="dca0a-107">К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="dca0a-107">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="dca0a-108">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="dca0a-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="dca0a-109">[Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="dca0a-109">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="dca0a-110">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="dca0a-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="dca0a-111">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="dca0a-111">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="dca0a-112">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="dca0a-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="dca0a-113">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="dca0a-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="dca0a-114">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="dca0a-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="dca0a-115">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="dca0a-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="dca0a-116">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="dca0a-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="dca0a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="dca0a-117">Relationships</span></span>

| <span data-ttu-id="dca0a-118">Связь</span><span class="sxs-lookup"><span data-stu-id="dca0a-118">Relationship</span></span>      | <span data-ttu-id="dca0a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dca0a-119">Type</span></span>          | <span data-ttu-id="dca0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dca0a-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="dca0a-121">trending</span><span class="sxs-lookup"><span data-stu-id="dca0a-121">trending</span></span>      | <span data-ttu-id="dca0a-122">Коллекция [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="dca0a-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="dca0a-123">Вычисляемая связь, определяющая популярные документы.</span><span class="sxs-lookup"><span data-stu-id="dca0a-123">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="dca0a-124">Популярные документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dca0a-124">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="dca0a-125">used</span><span class="sxs-lookup"><span data-stu-id="dca0a-125">used</span></span>      | <span data-ttu-id="dca0a-126">Коллекция [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="dca0a-126">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="dca0a-127">Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="dca0a-127">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="dca0a-128">Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.</span><span class="sxs-lookup"><span data-stu-id="dca0a-128">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="dca0a-129">общие</span><span class="sxs-lookup"><span data-stu-id="dca0a-129">shared</span></span>        | <span data-ttu-id="dca0a-130">Коллекция [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="dca0a-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="dca0a-131">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="dca0a-131">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="dca0a-132">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="dca0a-132">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="dca0a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dca0a-133">JSON representation</span></span>

<span data-ttu-id="dca0a-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca0a-134">Here is a JSON representation of the resource</span></span>
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
