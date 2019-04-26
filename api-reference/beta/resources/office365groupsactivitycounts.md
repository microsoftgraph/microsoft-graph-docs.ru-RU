---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581725"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="b658e-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b658e-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b658e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b658e-104">Properties</span></span>

| <span data-ttu-id="b658e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b658e-105">Property</span></span>               | <span data-ttu-id="b658e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b658e-106">Type</span></span>   | <span data-ttu-id="b658e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b658e-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b658e-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="b658e-108">reportRefreshDate</span></span>      | <span data-ttu-id="b658e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b658e-109">Date</span></span>   | <span data-ttu-id="b658e-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="b658e-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="b658e-111">Ексчанжеемаилсрецеивед</span><span class="sxs-lookup"><span data-stu-id="b658e-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="b658e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b658e-112">Int64</span></span>  | <span data-ttu-id="b658e-113">Количество сообщений электронной почты, получаемых групповой почтовыми ящиками.</span><span class="sxs-lookup"><span data-stu-id="b658e-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="b658e-114">Яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="b658e-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="b658e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b658e-115">Int64</span></span>  | <span data-ttu-id="b658e-116">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="b658e-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="b658e-117">Яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="b658e-117">yammerMessagesRead</span></span>     | <span data-ttu-id="b658e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b658e-118">Int64</span></span>  | <span data-ttu-id="b658e-119">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="b658e-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="b658e-120">Яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="b658e-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="b658e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b658e-121">Int64</span></span>  | <span data-ttu-id="b658e-122">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="b658e-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="b658e-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="b658e-123">reportDate</span></span>             | <span data-ttu-id="b658e-124">Дата</span><span class="sxs-lookup"><span data-stu-id="b658e-124">Date</span></span>   | <span data-ttu-id="b658e-125">Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений.</span><span class="sxs-lookup"><span data-stu-id="b658e-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="b658e-126">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="b658e-126">reportPeriod</span></span>           | <span data-ttu-id="b658e-127">String</span><span class="sxs-lookup"><span data-stu-id="b658e-127">String</span></span> | <span data-ttu-id="b658e-128">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="b658e-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b658e-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b658e-129">JSON representation</span></span>

<span data-ttu-id="b658e-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b658e-130">The following is a JSON representation of the resource.</span></span>

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
