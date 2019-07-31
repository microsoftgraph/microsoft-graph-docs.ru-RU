---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966554"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="c20c7-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c20c7-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c20c7-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c20c7-104">Properties</span></span>

| <span data-ttu-id="c20c7-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c20c7-105">Property</span></span>               | <span data-ttu-id="c20c7-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c20c7-106">Type</span></span>   | <span data-ttu-id="c20c7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c20c7-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c20c7-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c20c7-108">reportRefreshDate</span></span>      | <span data-ttu-id="c20c7-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c20c7-109">Date</span></span>   | <span data-ttu-id="c20c7-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="c20c7-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="c20c7-111">Ексчанжеемаилсрецеивед</span><span class="sxs-lookup"><span data-stu-id="c20c7-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="c20c7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c20c7-112">Int64</span></span>  | <span data-ttu-id="c20c7-113">Количество сообщений электронной почты, получаемых групповой почтовыми ящиками.</span><span class="sxs-lookup"><span data-stu-id="c20c7-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="c20c7-114">Яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="c20c7-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="c20c7-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c20c7-115">Int64</span></span>  | <span data-ttu-id="c20c7-116">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="c20c7-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="c20c7-117">Яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="c20c7-117">yammerMessagesRead</span></span>     | <span data-ttu-id="c20c7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c20c7-118">Int64</span></span>  | <span data-ttu-id="c20c7-119">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c20c7-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="c20c7-120">Яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="c20c7-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="c20c7-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c20c7-121">Int64</span></span>  | <span data-ttu-id="c20c7-122">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c20c7-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="c20c7-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="c20c7-123">reportDate</span></span>             | <span data-ttu-id="c20c7-124">Дата</span><span class="sxs-lookup"><span data-stu-id="c20c7-124">Date</span></span>   | <span data-ttu-id="c20c7-125">Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений.</span><span class="sxs-lookup"><span data-stu-id="c20c7-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="c20c7-126">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="c20c7-126">reportPeriod</span></span>           | <span data-ttu-id="c20c7-127">String</span><span class="sxs-lookup"><span data-stu-id="c20c7-127">String</span></span> | <span data-ttu-id="c20c7-128">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="c20c7-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c20c7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c20c7-129">JSON representation</span></span>

<span data-ttu-id="c20c7-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c20c7-130">The following is a JSON representation of the resource.</span></span>

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
