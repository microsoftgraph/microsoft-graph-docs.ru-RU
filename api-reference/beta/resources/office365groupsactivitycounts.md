---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081598"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="2cf2b-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="2cf2b-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2cf2b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cf2b-104">Properties</span></span>

| <span data-ttu-id="2cf2b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cf2b-105">Property</span></span>               | <span data-ttu-id="2cf2b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2cf2b-106">Type</span></span>   | <span data-ttu-id="2cf2b-107">Description</span><span class="sxs-lookup"><span data-stu-id="2cf2b-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2cf2b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2cf2b-108">reportRefreshDate</span></span>      | <span data-ttu-id="2cf2b-109">Date</span><span class="sxs-lookup"><span data-stu-id="2cf2b-109">Date</span></span>   | <span data-ttu-id="2cf2b-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2cf2b-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="2cf2b-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="2cf2b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2cf2b-112">Int64</span></span>  | <span data-ttu-id="2cf2b-113">Количество почтовых ящиков групп, получаемые по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="2cf2b-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="2cf2b-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="2cf2b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2cf2b-115">Int64</span></span>  | <span data-ttu-id="2cf2b-116">Число сообщений, помещенных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="2cf2b-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="2cf2b-117">yammerMessagesRead</span></span>     | <span data-ttu-id="2cf2b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2cf2b-118">Int64</span></span>  | <span data-ttu-id="2cf2b-119">Количество сообщений, ознакомьтесь с разделом в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="2cf2b-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="2cf2b-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="2cf2b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="2cf2b-121">Int64</span></span>  | <span data-ttu-id="2cf2b-122">Количество сообщений, оцененных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="2cf2b-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="2cf2b-123">reportDate</span></span>             | <span data-ttu-id="2cf2b-124">Date</span><span class="sxs-lookup"><span data-stu-id="2cf2b-124">Date</span></span>   | <span data-ttu-id="2cf2b-125">Дата отправки целого ряда по электронной почте в почтовый ящик группы или учета количество сообщений, чтение или нравится, что в группе Yammer</span><span class="sxs-lookup"><span data-stu-id="2cf2b-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="2cf2b-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2cf2b-126">reportPeriod</span></span>           | <span data-ttu-id="2cf2b-127">String</span><span class="sxs-lookup"><span data-stu-id="2cf2b-127">String</span></span> | <span data-ttu-id="2cf2b-128">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2cf2b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cf2b-129">JSON representation</span></span>

<span data-ttu-id="2cf2b-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cf2b-130">The following is a JSON representation of the resource.</span></span>

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
