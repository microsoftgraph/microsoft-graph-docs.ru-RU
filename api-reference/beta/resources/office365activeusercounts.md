---
title: Тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 4841377ba8b9aa5a94ca97b50847517be5b2f0cc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898074"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="a57d3-103">Тип ресурса office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a57d3-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="a57d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a57d3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a57d3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a57d3-105">Properties</span></span>

| <span data-ttu-id="a57d3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a57d3-106">Property</span></span>          | <span data-ttu-id="a57d3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a57d3-107">Type</span></span>   | <span data-ttu-id="a57d3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a57d3-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a57d3-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="a57d3-109">reportRefreshDate</span></span> | <span data-ttu-id="a57d3-110">Дата</span><span class="sxs-lookup"><span data-stu-id="a57d3-110">Date</span></span>   | <span data-ttu-id="a57d3-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="a57d3-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="a57d3-112">Office365</span><span class="sxs-lookup"><span data-stu-id="a57d3-112">office365</span></span>         | <span data-ttu-id="a57d3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-113">Int64</span></span>  | <span data-ttu-id="a57d3-114">Количество активных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a57d3-114">The number of active users in Microsoft 365.</span></span> <span data-ttu-id="a57d3-115">Это число включает все активные пользователи в Exchange, OneDrive, SharePoint, Skype для бизнеса, Yammer и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a57d3-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="a57d3-116">Определение активных пользователей для каждого продукта можно найти в описании соответствующего свойства.</span><span class="sxs-lookup"><span data-stu-id="a57d3-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="a57d3-117">теплообменник</span><span class="sxs-lookup"><span data-stu-id="a57d3-117">exchange</span></span>          | <span data-ttu-id="a57d3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-118">Int64</span></span>  | <span data-ttu-id="a57d3-119">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a57d3-119">The number of active users in Exchange.</span></span> <span data-ttu-id="a57d3-120">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="a57d3-121">oneDrive</span></span>          | <span data-ttu-id="a57d3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-122">Int64</span></span>  | <span data-ttu-id="a57d3-123">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a57d3-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="a57d3-124">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-125">sharePoint</span><span class="sxs-lookup"><span data-stu-id="a57d3-125">sharePoint</span></span>        | <span data-ttu-id="a57d3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-126">Int64</span></span>  | <span data-ttu-id="a57d3-127">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a57d3-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="a57d3-128">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="a57d3-129">skypeForBusiness</span></span>  | <span data-ttu-id="a57d3-130">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-130">Int64</span></span>  | <span data-ttu-id="a57d3-131">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a57d3-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="a57d3-132">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-133">Yammer</span><span class="sxs-lookup"><span data-stu-id="a57d3-133">yammer</span></span>            | <span data-ttu-id="a57d3-134">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-134">Int64</span></span>  | <span data-ttu-id="a57d3-135">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="a57d3-135">The number of active users in Yammer.</span></span> <span data-ttu-id="a57d3-136">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-137">Teams</span><span class="sxs-lookup"><span data-stu-id="a57d3-137">teams</span></span>             | <span data-ttu-id="a57d3-138">Int64</span><span class="sxs-lookup"><span data-stu-id="a57d3-138">Int64</span></span>  | <span data-ttu-id="a57d3-139">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a57d3-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="a57d3-140">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="a57d3-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="a57d3-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="a57d3-141">reportDate</span></span>        | <span data-ttu-id="a57d3-142">Дата</span><span class="sxs-lookup"><span data-stu-id="a57d3-142">Date</span></span>   | <span data-ttu-id="a57d3-143">Дата, когда число пользователей было активно.</span><span class="sxs-lookup"><span data-stu-id="a57d3-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="a57d3-144">репортпериод</span><span class="sxs-lookup"><span data-stu-id="a57d3-144">reportPeriod</span></span>      | <span data-ttu-id="a57d3-145">String</span><span class="sxs-lookup"><span data-stu-id="a57d3-145">String</span></span> | <span data-ttu-id="a57d3-146">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="a57d3-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a57d3-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a57d3-147">JSON representation</span></span>

<span data-ttu-id="a57d3-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a57d3-148">The following is a JSON representation of the resource.</span></span>

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
