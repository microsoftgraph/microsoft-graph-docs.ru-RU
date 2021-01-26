---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 276153f9613f464cdf11f6dfdad307bb341f646d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982154"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="50f77-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="50f77-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="50f77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f77-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="50f77-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="50f77-105">Properties</span></span>

| <span data-ttu-id="50f77-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="50f77-106">Property</span></span>                 | <span data-ttu-id="50f77-107">Тип</span><span class="sxs-lookup"><span data-stu-id="50f77-107">Type</span></span>   | <span data-ttu-id="50f77-108">Описание</span><span class="sxs-lookup"><span data-stu-id="50f77-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="50f77-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="50f77-109">reportRefreshDate</span></span>        | <span data-ttu-id="50f77-110">Дата</span><span class="sxs-lookup"><span data-stu-id="50f77-110">Date</span></span>   | <span data-ttu-id="50f77-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="50f77-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="50f77-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="50f77-112">exchangeActive</span></span>           | <span data-ttu-id="50f77-113">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-113">Int64</span></span>  | <span data-ttu-id="50f77-114">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="50f77-114">The number of active users on Exchange.</span></span> <span data-ttu-id="50f77-115">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="50f77-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-116">exchangeInactive</span></span>         | <span data-ttu-id="50f77-117">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-117">Int64</span></span>  | <span data-ttu-id="50f77-118">Количество неактивных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="50f77-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="50f77-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="50f77-119">oneDriveActive</span></span>           | <span data-ttu-id="50f77-120">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-120">Int64</span></span>  | <span data-ttu-id="50f77-121">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="50f77-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="50f77-122">Любой пользователь, просматривавший или редактировал файлы, общие файлы внутри или извне или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="50f77-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-123">oneDriveInactive</span></span>         | <span data-ttu-id="50f77-124">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-124">Int64</span></span>  | <span data-ttu-id="50f77-125">Количество неактивных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="50f77-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="50f77-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="50f77-126">sharePointActive</span></span>         | <span data-ttu-id="50f77-127">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-127">Int64</span></span>  | <span data-ttu-id="50f77-128">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="50f77-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="50f77-129">Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне, синхронизированные файлы или просматривал страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="50f77-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-130">sharePointInactive</span></span>       | <span data-ttu-id="50f77-131">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-131">Int64</span></span>  | <span data-ttu-id="50f77-132">Количество неактивных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="50f77-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="50f77-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="50f77-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="50f77-134">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-134">Int64</span></span>  | <span data-ttu-id="50f77-135">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="50f77-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="50f77-136">Любой пользователь, который организовывал или принимал участие в конференциях или присоединялся к одноранговом сеансу, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="50f77-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="50f77-138">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-138">Int64</span></span>  | <span data-ttu-id="50f77-139">Количество неактивных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="50f77-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="50f77-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="50f77-140">yammerActive</span></span>             | <span data-ttu-id="50f77-141">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-141">Int64</span></span>  | <span data-ttu-id="50f77-142">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="50f77-142">The number of active users on Yammer.</span></span> <span data-ttu-id="50f77-143">Любой пользователь, который может размещать, читать или читать сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="50f77-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-144">yammerInactive</span></span>           | <span data-ttu-id="50f77-145">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-145">Int64</span></span>  | <span data-ttu-id="50f77-146">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="50f77-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="50f77-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="50f77-147">teamsActive</span></span>              | <span data-ttu-id="50f77-148">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-148">Int64</span></span>  | <span data-ttu-id="50f77-149">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="50f77-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="50f77-150">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах приватного чата или участвовал в собраниях или звонках, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="50f77-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="50f77-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="50f77-151">teamsInactive</span></span>            | <span data-ttu-id="50f77-152">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-152">Int64</span></span>  | <span data-ttu-id="50f77-153">Количество неактивных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="50f77-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="50f77-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="50f77-154">office365Active</span></span>          | <span data-ttu-id="50f77-155">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-155">Int64</span></span>  | <span data-ttu-id="50f77-156">Количество активных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="50f77-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="50f77-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="50f77-157">office365Inactive</span></span>        | <span data-ttu-id="50f77-158">Int64</span><span class="sxs-lookup"><span data-stu-id="50f77-158">Int64</span></span>  | <span data-ttu-id="50f77-159">Количество неактивных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="50f77-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="50f77-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="50f77-160">reportPeriod</span></span>             | <span data-ttu-id="50f77-161">String</span><span class="sxs-lookup"><span data-stu-id="50f77-161">String</span></span> | <span data-ttu-id="50f77-162">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="50f77-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="50f77-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50f77-163">JSON representation</span></span>

<span data-ttu-id="50f77-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50f77-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```


