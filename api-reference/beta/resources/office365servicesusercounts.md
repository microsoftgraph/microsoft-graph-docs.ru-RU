---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 18282aaa8dcd176a6eaa3a8176154670bfd6da9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808017"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="bf1d3-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="bf1d3-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bf1d3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf1d3-104">Properties</span></span>

| <span data-ttu-id="bf1d3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf1d3-105">Property</span></span>                 | <span data-ttu-id="bf1d3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bf1d3-106">Type</span></span>   | <span data-ttu-id="bf1d3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1d3-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="bf1d3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bf1d3-108">reportRefreshDate</span></span>        | <span data-ttu-id="bf1d3-109">Date</span><span class="sxs-lookup"><span data-stu-id="bf1d3-109">Date</span></span>   | <span data-ttu-id="bf1d3-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="bf1d3-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-111">exchangeActive</span></span>           | <span data-ttu-id="bf1d3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-112">Int64</span></span>  | <span data-ttu-id="bf1d3-113">Число активных пользователей на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-113">The number of active users on Exchange.</span></span> <span data-ttu-id="bf1d3-114">Любой пользователь, который можно читать и отправлять электронную почту считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-115">exchangeInactive</span></span>         | <span data-ttu-id="bf1d3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-116">Int64</span></span>  | <span data-ttu-id="bf1d3-117">Количество неактивных пользователей на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="bf1d3-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-118">oneDriveActive</span></span>           | <span data-ttu-id="bf1d3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-119">Int64</span></span>  | <span data-ttu-id="bf1d3-120">Количество активных пользователей на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="bf1d3-121">Любой пользователь, просматривать или изменять файлы, общих файлов во внутреннем или внешнем ресурсе или синхронизирован файлы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-122">oneDriveInactive</span></span>         | <span data-ttu-id="bf1d3-123">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-123">Int64</span></span>  | <span data-ttu-id="bf1d3-124">Количество неактивных пользователей на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="bf1d3-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-125">sharePointActive</span></span>         | <span data-ttu-id="bf1d3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-126">Int64</span></span>  | <span data-ttu-id="bf1d3-127">Число активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="bf1d3-128">Любой пользователь, просматривать или изменять файлы, общих файлов во внутренней сети или извне, синхронизированные файлы или просматривать страницы SharePoint считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-129">sharePointInactive</span></span>       | <span data-ttu-id="bf1d3-130">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-130">Int64</span></span>  | <span data-ttu-id="bf1d3-131">Количество неактивных пользователей на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="bf1d3-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="bf1d3-133">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-133">Int64</span></span>  | <span data-ttu-id="bf1d3-134">Число активных пользователей в Скайп для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="bf1d3-135">Любой пользователь, который организовал принявших участие в конференциях или в состав peer-to-peer sessions считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="bf1d3-137">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-137">Int64</span></span>  | <span data-ttu-id="bf1d3-138">Количество неактивных пользователей на Скайп для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="bf1d3-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-139">yammerActive</span></span>             | <span data-ttu-id="bf1d3-140">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-140">Int64</span></span>  | <span data-ttu-id="bf1d3-141">Число активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-141">The number of active users on Yammer.</span></span> <span data-ttu-id="bf1d3-142">Любой пользователь, который можно публиковать, чтение или как сообщения считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-143">yammerInactive</span></span>           | <span data-ttu-id="bf1d3-144">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-144">Int64</span></span>  | <span data-ttu-id="bf1d3-145">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="bf1d3-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-146">teamsActive</span></span>              | <span data-ttu-id="bf1d3-147">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-147">Int64</span></span>  | <span data-ttu-id="bf1d3-148">Число активных пользователей в группы.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-148">The number of active users on Teams.</span></span> <span data-ttu-id="bf1d3-149">Любой пользователь, который сообщений, помещенных в каналы группы, отправленных сообщений в сеансах частной беседы или являлся участником собрания или вызовы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="bf1d3-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="bf1d3-150">teamsInactive</span></span>            | <span data-ttu-id="bf1d3-151">Int64</span><span class="sxs-lookup"><span data-stu-id="bf1d3-151">Int64</span></span>  | <span data-ttu-id="bf1d3-152">Число активных пользователей в группы.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="bf1d3-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bf1d3-153">reportPeriod</span></span>             | <span data-ttu-id="bf1d3-154">Строка</span><span class="sxs-lookup"><span data-stu-id="bf1d3-154">String</span></span> | <span data-ttu-id="bf1d3-155">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="bf1d3-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf1d3-156">JSON representation</span></span>

<span data-ttu-id="bf1d3-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf1d3-157">The following is a JSON representation of the resource.</span></span>

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
  "reportPeriod": "String"
}
```
