---
title: Тип ресурса itemInsights
description: Связи между пользователем и элементами, такими как документы в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. К примеру, вы можете определить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e5f0e525f95f988e7cb90c454285d2ecdb6b1072
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435000"
---
# <a name="iteminsights-resource-type"></a><span data-ttu-id="b95f0-104">Тип ресурса itemInsights</span><span class="sxs-lookup"><span data-stu-id="b95f0-104">itemInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b95f0-105">Связи между пользователем и элементами, такими как документы в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="b95f0-105">Relationships between a user and items such as OneDrive for Business documents, calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="b95f0-106">К примеру, вы можете определить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.</span><span class="sxs-lookup"><span data-stu-id="b95f0-106">You can, for example, identify OneDrive for Business documents trending around users.</span></span> <span data-ttu-id="b95f0-107">Производный от [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="b95f0-107">Derived from [officeGraphInsights](officegraphinsights.md).</span></span>

<span data-ttu-id="b95f0-108">Аналитика возвращается с помощью указанных ниже API.</span><span class="sxs-lookup"><span data-stu-id="b95f0-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="b95f0-109">[Популярные](insights-trending.md) — возвращает документы из OneDrive для бизнеса и сайтов SharePoint, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="b95f0-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="b95f0-110">[Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем.</span><span class="sxs-lookup"><span data-stu-id="b95f0-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="b95f0-111">Включает документы, использованные пользователем в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b95f0-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="b95f0-112">[Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="b95f0-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="b95f0-113">Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b95f0-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="b95f0-114">Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="b95f0-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="b95f0-115">Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="b95f0-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="b95f0-116">Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.</span><span class="sxs-lookup"><span data-stu-id="b95f0-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

### <a name="limiting-item-insights"></a><span data-ttu-id="b95f0-117">Ограничения для аналитики элементов</span><span class="sxs-lookup"><span data-stu-id="b95f0-117">Limiting item insights</span></span>

<span data-ttu-id="b95f0-118">Обновите [itemInsightsSettings](iteminsightssettings.md), чтобы отключить аналитику элементов для определенной группы Azure AD или всей организации.</span><span class="sxs-lookup"><span data-stu-id="b95f0-118">Update [itemInsightsSettings](iteminsightssettings.md) to disable item insights for a specific Azure AD group or an entire organization.</span></span> <span data-ttu-id="b95f0-119">Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="b95f0-119">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span>

## <a name="relationships"></a><span data-ttu-id="b95f0-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b95f0-120">Relationships</span></span>

| <span data-ttu-id="b95f0-121">Связь</span><span class="sxs-lookup"><span data-stu-id="b95f0-121">Relationship</span></span>      | <span data-ttu-id="b95f0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b95f0-122">Type</span></span>          | <span data-ttu-id="b95f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b95f0-123">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="b95f0-124">trending</span><span class="sxs-lookup"><span data-stu-id="b95f0-124">trending</span></span>      | <span data-ttu-id="b95f0-125">Коллекция объектов [trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="b95f0-125">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="b95f0-126">Вычисляемая связь, определяющая документы, популярные у пользователя.</span><span class="sxs-lookup"><span data-stu-id="b95f0-126">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="b95f0-127">Документы, популярные у пользователя, рассчитываются на основе действий пользователя в ближайшей сети людей и включают файлы, сохраненные в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b95f0-127">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="b95f0-128">Аналитика документов, популярных у пользователя, позволяет обнаружить потенциально полезное содержимое, к которому у пользователя есть доступ, но которое он еще не просматривал.</span><span class="sxs-lookup"><span data-stu-id="b95f0-128">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="b95f0-129">used</span><span class="sxs-lookup"><span data-stu-id="b95f0-129">used</span></span>      | <span data-ttu-id="b95f0-130">Коллекция объектов [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="b95f0-130">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="b95f0-131">Вычисляемая связь, определяющая последние документы, просмотренные и измененные пользователем, в том числе документы в OneDrive для бизнеса и SharePoint, упорядоченные по давности использования.</span><span class="sxs-lookup"><span data-stu-id="b95f0-131">Calculated relationship identifying the latest documents viewed and modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="b95f0-132">общие</span><span class="sxs-lookup"><span data-stu-id="b95f0-132">shared</span></span>        | <span data-ttu-id="b95f0-133">Коллекция объектов [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="b95f0-133">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="b95f0-134">Вычисляемая связь, определяющая документы, к которым предоставлен общий доступ пользователю или пользователем, включает вложенные файлы в сообщениях электронной почты и собраниях, а также URL-адреса и ссылочные вложения в файлах OneDrive для бизнеса и SharePoint, которые можно найти в сообщениях электронной почты, собраниях и беседах Teams.</span><span class="sxs-lookup"><span data-stu-id="b95f0-134">Calculated relationship identifying documents shared with or by the user, includes file attachments in emails and meetings, as well as URLs and Reference attachments to OneDrive for Business and SharePoint files found in emails, meetings, and Teams conversations.</span></span> <span data-ttu-id="b95f0-135">Упорядочено по давности общего доступа.</span><span class="sxs-lookup"><span data-stu-id="b95f0-135">Ordered by recency of share.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b95f0-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b95f0-136">JSON representation</span></span>

<span data-ttu-id="b95f0-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b95f0-137">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
