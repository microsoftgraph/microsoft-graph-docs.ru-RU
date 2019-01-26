---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573895"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="9eac5-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="9eac5-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9eac5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eac5-104">Properties</span></span>

| <span data-ttu-id="9eac5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eac5-105">Property</span></span>                 | <span data-ttu-id="9eac5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="9eac5-106">Type</span></span>   | <span data-ttu-id="9eac5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9eac5-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9eac5-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9eac5-108">reportRefreshDate</span></span>        | <span data-ttu-id="9eac5-109">Date</span><span class="sxs-lookup"><span data-stu-id="9eac5-109">Date</span></span>   | <span data-ttu-id="9eac5-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="9eac5-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="9eac5-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-111">exchangeActive</span></span>           | <span data-ttu-id="9eac5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-112">Int64</span></span>  | <span data-ttu-id="9eac5-113">Число активных пользователей на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="9eac5-113">The number of active users on Exchange.</span></span> <span data-ttu-id="9eac5-114">Любой пользователь, который можно читать и отправлять электронную почту считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-115">exchangeInactive</span></span>         | <span data-ttu-id="9eac5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-116">Int64</span></span>  | <span data-ttu-id="9eac5-117">Количество неактивных пользователей на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="9eac5-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="9eac5-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-118">oneDriveActive</span></span>           | <span data-ttu-id="9eac5-119">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-119">Int64</span></span>  | <span data-ttu-id="9eac5-120">Количество активных пользователей на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9eac5-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="9eac5-121">Любой пользователь, просматривать или изменять файлы, общих файлов во внутреннем или внешнем ресурсе или синхронизирован файлы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-122">oneDriveInactive</span></span>         | <span data-ttu-id="9eac5-123">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-123">Int64</span></span>  | <span data-ttu-id="9eac5-124">Количество неактивных пользователей на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9eac5-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="9eac5-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-125">sharePointActive</span></span>         | <span data-ttu-id="9eac5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-126">Int64</span></span>  | <span data-ttu-id="9eac5-127">Число активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9eac5-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="9eac5-128">Любой пользователь, просматривать или изменять файлы, общих файлов во внутренней сети или извне, синхронизированные файлы или просматривать страницы SharePoint считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-129">sharePointInactive</span></span>       | <span data-ttu-id="9eac5-130">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-130">Int64</span></span>  | <span data-ttu-id="9eac5-131">Количество неактивных пользователей на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9eac5-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="9eac5-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="9eac5-133">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-133">Int64</span></span>  | <span data-ttu-id="9eac5-134">Число активных пользователей в Скайп для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9eac5-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="9eac5-135">Любой пользователь, который организовал принявших участие в конференциях или в состав peer-to-peer sessions считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="9eac5-137">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-137">Int64</span></span>  | <span data-ttu-id="9eac5-138">Количество неактивных пользователей на Скайп для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9eac5-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="9eac5-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-139">yammerActive</span></span>             | <span data-ttu-id="9eac5-140">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-140">Int64</span></span>  | <span data-ttu-id="9eac5-141">Число активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="9eac5-141">The number of active users on Yammer.</span></span> <span data-ttu-id="9eac5-142">Любой пользователь, который можно публиковать, чтение или как сообщения считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-143">yammerInactive</span></span>           | <span data-ttu-id="9eac5-144">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-144">Int64</span></span>  | <span data-ttu-id="9eac5-145">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="9eac5-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="9eac5-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="9eac5-146">teamsActive</span></span>              | <span data-ttu-id="9eac5-147">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-147">Int64</span></span>  | <span data-ttu-id="9eac5-148">Число активных пользователей в группы Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9eac5-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="9eac5-149">Любой пользователь, который сообщений, помещенных в каналы группы, отправленных сообщений в сеансах частной беседы или являлся участником собрания или вызовы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9eac5-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="9eac5-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-150">teamsInactive</span></span>            | <span data-ttu-id="9eac5-151">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-151">Int64</span></span>  | <span data-ttu-id="9eac5-152">Количество неактивных пользователей на группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9eac5-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="9eac5-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="9eac5-153">office365Active</span></span>          | <span data-ttu-id="9eac5-154">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-154">Int64</span></span>  | <span data-ttu-id="9eac5-155">Число активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="9eac5-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="9eac5-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="9eac5-156">office365Inactive</span></span>        | <span data-ttu-id="9eac5-157">Int64</span><span class="sxs-lookup"><span data-stu-id="9eac5-157">Int64</span></span>  | <span data-ttu-id="9eac5-158">Количество неактивных пользователей на Office 365.</span><span class="sxs-lookup"><span data-stu-id="9eac5-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="9eac5-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9eac5-159">reportPeriod</span></span>             | <span data-ttu-id="9eac5-160">Строка</span><span class="sxs-lookup"><span data-stu-id="9eac5-160">String</span></span> | <span data-ttu-id="9eac5-161">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="9eac5-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="9eac5-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eac5-162">JSON representation</span></span>

<span data-ttu-id="9eac5-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eac5-163">The following is a JSON representation of the resource.</span></span>

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
