---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f07743a592753daff2670478c6f2fe18207f6013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522458"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="3086f-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="3086f-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="3086f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3086f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3086f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3086f-105">Properties</span></span>

| <span data-ttu-id="3086f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3086f-106">Property</span></span>               | <span data-ttu-id="3086f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3086f-107">Type</span></span>   | <span data-ttu-id="3086f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3086f-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3086f-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="3086f-109">reportRefreshDate</span></span>      | <span data-ttu-id="3086f-110">Дата</span><span class="sxs-lookup"><span data-stu-id="3086f-110">Date</span></span>   | <span data-ttu-id="3086f-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="3086f-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="3086f-112">ексчанжеемаилсрецеивед</span><span class="sxs-lookup"><span data-stu-id="3086f-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="3086f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3086f-113">Int64</span></span>  | <span data-ttu-id="3086f-114">Количество сообщений электронной почты, получаемых групповой почтовыми ящиками.</span><span class="sxs-lookup"><span data-stu-id="3086f-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="3086f-115">яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="3086f-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="3086f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3086f-116">Int64</span></span>  | <span data-ttu-id="3086f-117">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="3086f-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="3086f-118">яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="3086f-118">yammerMessagesRead</span></span>     | <span data-ttu-id="3086f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3086f-119">Int64</span></span>  | <span data-ttu-id="3086f-120">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="3086f-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="3086f-121">яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="3086f-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="3086f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3086f-122">Int64</span></span>  | <span data-ttu-id="3086f-123">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="3086f-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="3086f-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="3086f-124">reportDate</span></span>             | <span data-ttu-id="3086f-125">Дата</span><span class="sxs-lookup"><span data-stu-id="3086f-125">Date</span></span>   | <span data-ttu-id="3086f-126">Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений.</span><span class="sxs-lookup"><span data-stu-id="3086f-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="3086f-127">репортпериод</span><span class="sxs-lookup"><span data-stu-id="3086f-127">reportPeriod</span></span>           | <span data-ttu-id="3086f-128">String</span><span class="sxs-lookup"><span data-stu-id="3086f-128">String</span></span> | <span data-ttu-id="3086f-129">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="3086f-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3086f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3086f-130">JSON representation</span></span>

<span data-ttu-id="3086f-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3086f-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
