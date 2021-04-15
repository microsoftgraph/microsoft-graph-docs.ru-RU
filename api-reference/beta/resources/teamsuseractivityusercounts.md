---
title: тип ресурса teamsUserActivityUserCounts
description: Представляет число ежедневных пользователей по типу действия.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766443"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="be3d1-103">тип ресурса teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="be3d1-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="be3d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be3d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3d1-105">Представляет число ежедневных пользователей по типу действия.</span><span class="sxs-lookup"><span data-stu-id="be3d1-105">Represents numbers of daily users by activity type.</span></span>

## <a name="properties"></a><span data-ttu-id="be3d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="be3d1-106">Properties</span></span>

| <span data-ttu-id="be3d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="be3d1-107">Property</span></span>            | <span data-ttu-id="be3d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="be3d1-108">Type</span></span>   | <span data-ttu-id="be3d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="be3d1-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="be3d1-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="be3d1-110">reportRefreshDate</span></span>   | <span data-ttu-id="be3d1-111">Дата</span><span class="sxs-lookup"><span data-stu-id="be3d1-111">Date</span></span>   | <span data-ttu-id="be3d1-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="be3d1-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="be3d1-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="be3d1-113">reportDate</span></span>          | <span data-ttu-id="be3d1-114">Дата</span><span class="sxs-lookup"><span data-stu-id="be3d1-114">Date</span></span>   | <span data-ttu-id="be3d1-115">Дата выполнения пользователями действий.</span><span class="sxs-lookup"><span data-stu-id="be3d1-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="be3d1-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="be3d1-116">teamChatMessages</span></span>    | <span data-ttu-id="be3d1-117">Int64</span><span class="sxs-lookup"><span data-stu-id="be3d1-117">Int64</span></span>  | <span data-ttu-id="be3d1-118">Количество пользователей, которые разместили сообщение в командном чате.</span><span class="sxs-lookup"><span data-stu-id="be3d1-118">The number of users who posted message in a team chat.</span></span>       |
| <span data-ttu-id="be3d1-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="be3d1-119">privateChatMessages</span></span> | <span data-ttu-id="be3d1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="be3d1-120">Int64</span></span>  | <span data-ttu-id="be3d1-121">Число пользователей, которые разместили сообщение в частном чате.</span><span class="sxs-lookup"><span data-stu-id="be3d1-121">The number of users who posted message in a private chat.</span></span>    |
| <span data-ttu-id="be3d1-122">calls</span><span class="sxs-lookup"><span data-stu-id="be3d1-122">calls</span></span>               | <span data-ttu-id="be3d1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="be3d1-123">Int64</span></span>  | <span data-ttu-id="be3d1-124">Число пользователей, которые участвовали в звонках 1:1.</span><span class="sxs-lookup"><span data-stu-id="be3d1-124">The number of users who participated in 1:1 calls.</span></span>           |
| <span data-ttu-id="be3d1-125">meetings</span><span class="sxs-lookup"><span data-stu-id="be3d1-125">meetings</span></span>            | <span data-ttu-id="be3d1-126">Int64</span><span class="sxs-lookup"><span data-stu-id="be3d1-126">Int64</span></span>  | <span data-ttu-id="be3d1-127">Количество пользователей, которые участвовали в собраниях в Интернете.</span><span class="sxs-lookup"><span data-stu-id="be3d1-127">The number of users who participated in online meetings.</span></span>     |
| <span data-ttu-id="be3d1-128">otherActions</span><span class="sxs-lookup"><span data-stu-id="be3d1-128">otherActions</span></span>        | <span data-ttu-id="be3d1-129">Int64</span><span class="sxs-lookup"><span data-stu-id="be3d1-129">Int64</span></span>  | <span data-ttu-id="be3d1-130">Число пользователей, которые были активными, но выполняли другие действия, чем выставленные типы действий, предлагаемые в отчете (отправка или ответ на сообщения канала и сообщения чата, планирование или участие в звонках и собраниях 1:1).</span><span class="sxs-lookup"><span data-stu-id="be3d1-130">The number of users who were active but performed other activities than exposed action types offered in the report (sending or replying to channel messages and chat messages, scheduling or participating in 1:1 calls and meetings).</span></span> <span data-ttu-id="be3d1-131">Примеры действий, когда пользователь меняет состояние Teams или сообщение о состоянии Teams или открывает сообщение сообщения канала, но не отвечает.</span><span class="sxs-lookup"><span data-stu-id="be3d1-131">Examples actions are when a user changes the Teams status or the Teams status message or opens a Channel Message post but does not reply.</span></span> |
| <span data-ttu-id="be3d1-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="be3d1-132">reportPeriod</span></span>        | <span data-ttu-id="be3d1-133">String</span><span class="sxs-lookup"><span data-stu-id="be3d1-133">String</span></span> | <span data-ttu-id="be3d1-134">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="be3d1-134">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="be3d1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be3d1-135">JSON representation</span></span>

<span data-ttu-id="be3d1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be3d1-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```


