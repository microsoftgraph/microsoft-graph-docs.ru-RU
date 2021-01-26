---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a212028e4ba9d38ea38e99c835d89fe1fe7d850b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980698"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="66ec0-103">Тип ресурса office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="66ec0-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="66ec0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ec0-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="66ec0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="66ec0-105">Properties</span></span>

| <span data-ttu-id="66ec0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="66ec0-106">Property</span></span>               | <span data-ttu-id="66ec0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="66ec0-107">Type</span></span>   | <span data-ttu-id="66ec0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="66ec0-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="66ec0-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="66ec0-109">reportRefreshDate</span></span>      | <span data-ttu-id="66ec0-110">Дата</span><span class="sxs-lookup"><span data-stu-id="66ec0-110">Date</span></span>   | <span data-ttu-id="66ec0-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="66ec0-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="66ec0-112">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="66ec0-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="66ec0-113">Int64</span><span class="sxs-lookup"><span data-stu-id="66ec0-113">Int64</span></span>  | <span data-ttu-id="66ec0-114">Количество сообщений электронной почты, полученных почтовыми ящиками группы.</span><span class="sxs-lookup"><span data-stu-id="66ec0-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="66ec0-115">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="66ec0-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="66ec0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="66ec0-116">Int64</span></span>  | <span data-ttu-id="66ec0-117">Количество сообщений, которые были опубликованы в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="66ec0-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="66ec0-118">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="66ec0-118">yammerMessagesRead</span></span>     | <span data-ttu-id="66ec0-119">Int64</span><span class="sxs-lookup"><span data-stu-id="66ec0-119">Int64</span></span>  | <span data-ttu-id="66ec0-120">Количество сообщений, прочитано в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="66ec0-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="66ec0-121">yammerMessagesИмбл</span><span class="sxs-lookup"><span data-stu-id="66ec0-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="66ec0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="66ec0-122">Int64</span></span>  | <span data-ttu-id="66ec0-123">Количество сообщений, которые нравится в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="66ec0-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="66ec0-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="66ec0-124">reportDate</span></span>             | <span data-ttu-id="66ec0-125">Дата</span><span class="sxs-lookup"><span data-stu-id="66ec0-125">Date</span></span>   | <span data-ttu-id="66ec0-126">Дата отправки, чтения или отправки сообщений в почтовом ящике группы в группе Yammer</span><span class="sxs-lookup"><span data-stu-id="66ec0-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="66ec0-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="66ec0-127">reportPeriod</span></span>           | <span data-ttu-id="66ec0-128">String</span><span class="sxs-lookup"><span data-stu-id="66ec0-128">String</span></span> | <span data-ttu-id="66ec0-129">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="66ec0-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="66ec0-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66ec0-130">JSON representation</span></span>

<span data-ttu-id="66ec0-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66ec0-131">The following is a JSON representation of the resource.</span></span>

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


