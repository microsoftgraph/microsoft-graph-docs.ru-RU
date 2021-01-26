---
title: Тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 67c9b898da9a106685739ebbf78ccef6425c6617
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980740"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="3397a-103">Тип ресурса office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="3397a-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="3397a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3397a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3397a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3397a-105">Properties</span></span>

| <span data-ttu-id="3397a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3397a-106">Property</span></span>          | <span data-ttu-id="3397a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3397a-107">Type</span></span>   | <span data-ttu-id="3397a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3397a-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3397a-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3397a-109">reportRefreshDate</span></span> | <span data-ttu-id="3397a-110">Дата</span><span class="sxs-lookup"><span data-stu-id="3397a-110">Date</span></span>   | <span data-ttu-id="3397a-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="3397a-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="3397a-112">office365</span><span class="sxs-lookup"><span data-stu-id="3397a-112">office365</span></span>         | <span data-ttu-id="3397a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-113">Int64</span></span>  | <span data-ttu-id="3397a-114">Количество активных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3397a-114">The number of active users in Microsoft 365.</span></span> <span data-ttu-id="3397a-115">Это число включает всех активных пользователей в Exchange, OneDrive, SharePoint, Skype для бизнеса, Yammer и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3397a-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="3397a-116">Определение активного пользователя для каждого продукта можно найти в соответствующем описании свойства.</span><span class="sxs-lookup"><span data-stu-id="3397a-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="3397a-117">exchange</span><span class="sxs-lookup"><span data-stu-id="3397a-117">exchange</span></span>          | <span data-ttu-id="3397a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-118">Int64</span></span>  | <span data-ttu-id="3397a-119">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3397a-119">The number of active users in Exchange.</span></span> <span data-ttu-id="3397a-120">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="3397a-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="3397a-121">oneDrive</span></span>          | <span data-ttu-id="3397a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-122">Int64</span></span>  | <span data-ttu-id="3397a-123">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3397a-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="3397a-124">Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="3397a-125">sharePoint</span><span class="sxs-lookup"><span data-stu-id="3397a-125">sharePoint</span></span>        | <span data-ttu-id="3397a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-126">Int64</span></span>  | <span data-ttu-id="3397a-127">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3397a-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="3397a-128">Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне, синхронизированные файлы или просматривал страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="3397a-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="3397a-129">skypeForBusiness</span></span>  | <span data-ttu-id="3397a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-130">Int64</span></span>  | <span data-ttu-id="3397a-131">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3397a-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="3397a-132">Любой пользователь, который организовывал или принимал участие в конференциях или присоединялся к одноранговом сеансу, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="3397a-133">yammer</span><span class="sxs-lookup"><span data-stu-id="3397a-133">yammer</span></span>            | <span data-ttu-id="3397a-134">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-134">Int64</span></span>  | <span data-ttu-id="3397a-135">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="3397a-135">The number of active users in Yammer.</span></span> <span data-ttu-id="3397a-136">Любой пользователь, который может размещать, читать или читать сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="3397a-137">teams</span><span class="sxs-lookup"><span data-stu-id="3397a-137">teams</span></span>             | <span data-ttu-id="3397a-138">Int64</span><span class="sxs-lookup"><span data-stu-id="3397a-138">Int64</span></span>  | <span data-ttu-id="3397a-139">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3397a-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="3397a-140">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах приватного чата или участвовал в собраниях или звонках, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="3397a-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="3397a-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="3397a-141">reportDate</span></span>        | <span data-ttu-id="3397a-142">Дата</span><span class="sxs-lookup"><span data-stu-id="3397a-142">Date</span></span>   | <span data-ttu-id="3397a-143">Дата, когда было активно несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="3397a-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="3397a-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3397a-144">reportPeriod</span></span>      | <span data-ttu-id="3397a-145">String</span><span class="sxs-lookup"><span data-stu-id="3397a-145">String</span></span> | <span data-ttu-id="3397a-146">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="3397a-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3397a-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3397a-147">JSON representation</span></span>

<span data-ttu-id="3397a-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3397a-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


