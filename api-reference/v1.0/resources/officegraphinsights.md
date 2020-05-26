---
title: Тип ресурса officeGraphInsights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bfc058612b883ae51a1a674663c2704c4f4cde88
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226898"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="47506-104">Тип ресурса officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="47506-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="47506-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47506-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47506-106">Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="47506-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="47506-107">К примеру, вы можете выявить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="47506-107">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="47506-108">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="47506-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="47506-109">[Популярные](insights-trending.md) — возвращает документы из OneDrive для бизнеса и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="47506-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="47506-110">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="47506-110">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="47506-111">Включает документы, использованные пользователем в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="47506-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="47506-112">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен или пользователь предоставил общий доступ.</span><span class="sxs-lookup"><span data-stu-id="47506-112">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="47506-113">Общий доступ к документам можно предоставлять в виде по URL-ссылок, вложенных файлов, справочных вложений в OneDrive для бизнеса и файлам SharePoint, которые есть в сообщениях и собраниях Outlook.</span><span class="sxs-lookup"><span data-stu-id="47506-113">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="47506-114">Каждый объект аналитики возвращается со значением сложного типа (CVT) **resourceVisualization** и **resourceReference** сложного типа значений.</span><span class="sxs-lookup"><span data-stu-id="47506-114">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="47506-115">Сложный тип значенией **resourceVisualization** содержит такие свойства, как **title** и **previewImageUrl**.</span><span class="sxs-lookup"><span data-stu-id="47506-115">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="47506-116">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="47506-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="47506-117">Связи</span><span class="sxs-lookup"><span data-stu-id="47506-117">Relationships</span></span>

| <span data-ttu-id="47506-118">Связь</span><span class="sxs-lookup"><span data-stu-id="47506-118">Relationship</span></span>      | <span data-ttu-id="47506-119">Тип</span><span class="sxs-lookup"><span data-stu-id="47506-119">Type</span></span>          | <span data-ttu-id="47506-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47506-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="47506-121">trending</span><span class="sxs-lookup"><span data-stu-id="47506-121">trending</span></span>      | <span data-ttu-id="47506-122">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="47506-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="47506-123">Вычисляемая связь, определяющая документы, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="47506-123">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="47506-124">Документы, популярные у пользователя, рассчитываются на основе действий пользователя в ближайшей сети людей и включают файлы, сохраненные в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="47506-124">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="47506-125">Аналитика документов, популярных у пользователя, позволяет обнаружить потенциально полезное содержимое, к которому у пользователя есть доступ, но которое он еще не просматривал.</span><span class="sxs-lookup"><span data-stu-id="47506-125">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="47506-126">used</span><span class="sxs-lookup"><span data-stu-id="47506-126">used</span></span>      | <span data-ttu-id="47506-127">Коллекция объектов [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="47506-127">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="47506-128">Вычисление соотношения, определяющего последние документы, просмотренные или измененные пользователем, в том числе документы в OneDrive для бизнеса и SharePoint, упорядоченные по давности использования.</span><span class="sxs-lookup"><span data-stu-id="47506-128">Calculated relationship identifying the latest documents viewed or modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="47506-129">общие</span><span class="sxs-lookup"><span data-stu-id="47506-129">shared</span></span>        | <span data-ttu-id="47506-130">Коллекция объектов [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="47506-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="47506-131">Вычисляемая связь, определяющая документы, к которым пользователю предоставлен или пользователь предоставил общий доступ.</span><span class="sxs-lookup"><span data-stu-id="47506-131">Calculated relationship identifying documents shared with or by the user.</span></span> <span data-ttu-id="47506-132">Сюда включены URL-ссылки, вложенные файлы, справочные вложения в OneDrive для бизнеса и файлы SharePoint, которые есть в сообщениях и собраниях Outlook.</span><span class="sxs-lookup"><span data-stu-id="47506-132">This includes URLs, file attachments, and reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span> <span data-ttu-id="47506-133">Кроме того, сюда включены URL-ссылки и справочные вложения в беседах Teams.</span><span class="sxs-lookup"><span data-stu-id="47506-133">This also includes URLs and reference attachments to Teams conversations.</span></span> <span data-ttu-id="47506-134">Упорядочено по давности общего доступа.</span><span class="sxs-lookup"><span data-stu-id="47506-134">Ordered by recency of share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47506-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47506-135">JSON representation</span></span>

<span data-ttu-id="47506-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47506-136">Here is a JSON representation of the resource</span></span>
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
