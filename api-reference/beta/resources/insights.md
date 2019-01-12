---
title: Тип ресурса полезные сведения о
description: Полезные сведения о являются связи вычисляется с помощью расширенных аналитических и обучения методики компьютера. К примеру, могут определять документов OneDrive прибора вокруг пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938316"
---
# <a name="insights-resource-type"></a><span data-ttu-id="8ed21-104">Тип ресурса полезные сведения о</span><span class="sxs-lookup"><span data-stu-id="8ed21-104">insights resource type</span></span>

> <span data-ttu-id="8ed21-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ed21-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ed21-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ed21-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ed21-107">Полезные сведения о являются связи вычисляется с помощью расширенных аналитических и обучения методики компьютера.</span><span class="sxs-lookup"><span data-stu-id="8ed21-107">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="8ed21-108">К примеру, могут определять документов OneDrive прибора вокруг пользователей.</span><span class="sxs-lookup"><span data-stu-id="8ed21-108">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="8ed21-109">Полезные сведения о возвращаются следующие интерфейсы API:</span><span class="sxs-lookup"><span data-stu-id="8ed21-109">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="8ed21-110">[Тенденций](insights-trending.md) - возвращает документов из OneDrive и сайты SharePoint прибора вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ed21-110">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="8ed21-111">[Используется](insights-used.md) - возвращает документов просматривать и изменять пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ed21-111">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="8ed21-112">Содержит документы, используемые для пользователя в OneDrive для бизнеса, SharePoint, открывается в виде вложений электронной почты, а также как вложения ссылка из источников, например поле, общего банка данных и Google диска.</span><span class="sxs-lookup"><span data-stu-id="8ed21-112">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="8ed21-113">[Shared](insights-shared.md) - возвращает документы совместно с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ed21-113">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="8ed21-114">Документы могут совместно использоваться как вложения электронной почты или OneDrive для бизнеса ссылки в отправленных по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="8ed21-114">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="8ed21-115">Каждый insight возвращается вместе с `resourceVisualization` и `resourceReference` тип сложных значения (CVT).</span><span class="sxs-lookup"><span data-stu-id="8ed21-115">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="8ed21-116">ResourceVisualization CVT содержит свойства, такие как `title` и `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="8ed21-116">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="8ed21-117">Корпорация Майкрософт использует свойства визуализации для обработки файлов в каждый раз, как углубимся Office.</span><span class="sxs-lookup"><span data-stu-id="8ed21-117">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="8ed21-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8ed21-118">Relationships</span></span>

| <span data-ttu-id="8ed21-119">Связь</span><span class="sxs-lookup"><span data-stu-id="8ed21-119">Relationship</span></span>      | <span data-ttu-id="8ed21-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ed21-120">Type</span></span>          | <span data-ttu-id="8ed21-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ed21-121">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="8ed21-122">Анализ трендов</span><span class="sxs-lookup"><span data-stu-id="8ed21-122">trending</span></span>      | <span data-ttu-id="8ed21-123">Коллекция [тенденций](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="8ed21-123">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="8ed21-124">Идентификация документов тенденции вычисляемые отношения.</span><span class="sxs-lookup"><span data-stu-id="8ed21-124">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="8ed21-125">Тенденции документы могут храниться в OneDrive или на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed21-125">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="8ed21-126">used</span><span class="sxs-lookup"><span data-stu-id="8ed21-126">used</span></span>      | <span data-ttu-id="8ed21-127">[Используется](insights-used.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="8ed21-127">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="8ed21-128">Идентификация документов просматривать и изменять пользователем отношение вычисляется.</span><span class="sxs-lookup"><span data-stu-id="8ed21-128">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="8ed21-129">Содержит документы, используемые для пользователя в OneDrive для бизнеса, SharePoint, открывается в виде вложений электронной почты, а также как вложения ссылка из источников, например поле, общего банка данных и Google диска.</span><span class="sxs-lookup"><span data-stu-id="8ed21-129">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="8ed21-130">shared</span><span class="sxs-lookup"><span data-stu-id="8ed21-130">shared</span></span>        | <span data-ttu-id="8ed21-131">Семейства сайтов [Shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="8ed21-131">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="8ed21-132">Идентификация документов, совместно с пользователем вычисляемые отношения.</span><span class="sxs-lookup"><span data-stu-id="8ed21-132">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="8ed21-133">Документы могут совместно использоваться как вложения электронной почты или OneDrive для бизнеса ссылки в отправленных по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="8ed21-133">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="8ed21-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ed21-134">JSON representation</span></span>

<span data-ttu-id="8ed21-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ed21-135">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
