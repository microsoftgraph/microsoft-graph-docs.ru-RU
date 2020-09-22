---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6c67de6592d32c15e7d64112ce9ac31b6a5d4c41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092428"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="c6de1-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c6de1-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="c6de1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6de1-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c6de1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6de1-105">Properties</span></span>

| <span data-ttu-id="c6de1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6de1-106">Property</span></span>               | <span data-ttu-id="c6de1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c6de1-107">Type</span></span>   | <span data-ttu-id="c6de1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c6de1-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c6de1-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c6de1-109">reportRefreshDate</span></span>      | <span data-ttu-id="c6de1-110">Дата</span><span class="sxs-lookup"><span data-stu-id="c6de1-110">Date</span></span>   | <span data-ttu-id="c6de1-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="c6de1-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="c6de1-112">ексчанжеемаилсрецеивед</span><span class="sxs-lookup"><span data-stu-id="c6de1-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="c6de1-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c6de1-113">Int64</span></span>  | <span data-ttu-id="c6de1-114">Количество сообщений электронной почты, получаемых групповой почтовыми ящиками.</span><span class="sxs-lookup"><span data-stu-id="c6de1-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="c6de1-115">яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="c6de1-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="c6de1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c6de1-116">Int64</span></span>  | <span data-ttu-id="c6de1-117">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="c6de1-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="c6de1-118">яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="c6de1-118">yammerMessagesRead</span></span>     | <span data-ttu-id="c6de1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c6de1-119">Int64</span></span>  | <span data-ttu-id="c6de1-120">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c6de1-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="c6de1-121">яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="c6de1-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="c6de1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c6de1-122">Int64</span></span>  | <span data-ttu-id="c6de1-123">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c6de1-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="c6de1-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="c6de1-124">reportDate</span></span>             | <span data-ttu-id="c6de1-125">Дата</span><span class="sxs-lookup"><span data-stu-id="c6de1-125">Date</span></span>   | <span data-ttu-id="c6de1-126">Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений.</span><span class="sxs-lookup"><span data-stu-id="c6de1-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="c6de1-127">репортпериод</span><span class="sxs-lookup"><span data-stu-id="c6de1-127">reportPeriod</span></span>           | <span data-ttu-id="c6de1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="c6de1-128">String</span></span> | <span data-ttu-id="c6de1-129">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="c6de1-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c6de1-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c6de1-130">JSON representation</span></span>

<span data-ttu-id="c6de1-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6de1-131">The following is a JSON representation of the resource.</span></span>

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


