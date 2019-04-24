---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505461"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="59372-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="59372-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="59372-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="59372-104">Properties</span></span>

| <span data-ttu-id="59372-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="59372-105">Property</span></span>                 | <span data-ttu-id="59372-106">Тип</span><span class="sxs-lookup"><span data-stu-id="59372-106">Type</span></span>   | <span data-ttu-id="59372-107">Описание</span><span class="sxs-lookup"><span data-stu-id="59372-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="59372-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="59372-108">reportRefreshDate</span></span>        | <span data-ttu-id="59372-109">Дата</span><span class="sxs-lookup"><span data-stu-id="59372-109">Date</span></span>   | <span data-ttu-id="59372-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="59372-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="59372-111">Ексчанжеактиве</span><span class="sxs-lookup"><span data-stu-id="59372-111">exchangeActive</span></span>           | <span data-ttu-id="59372-112">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-112">Int64</span></span>  | <span data-ttu-id="59372-113">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="59372-113">The number of active users on Exchange.</span></span> <span data-ttu-id="59372-114">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="59372-115">Ексчанжеинактиве</span><span class="sxs-lookup"><span data-stu-id="59372-115">exchangeInactive</span></span>         | <span data-ttu-id="59372-116">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-116">Int64</span></span>  | <span data-ttu-id="59372-117">Количество неактивных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="59372-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="59372-118">Онедривеактиве</span><span class="sxs-lookup"><span data-stu-id="59372-118">oneDriveActive</span></span>           | <span data-ttu-id="59372-119">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-119">Int64</span></span>  | <span data-ttu-id="59372-120">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="59372-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="59372-121">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="59372-122">Онедривеинактиве</span><span class="sxs-lookup"><span data-stu-id="59372-122">oneDriveInactive</span></span>         | <span data-ttu-id="59372-123">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-123">Int64</span></span>  | <span data-ttu-id="59372-124">Количество неактивных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="59372-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="59372-125">Шарепоинтактиве</span><span class="sxs-lookup"><span data-stu-id="59372-125">sharePointActive</span></span>         | <span data-ttu-id="59372-126">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-126">Int64</span></span>  | <span data-ttu-id="59372-127">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="59372-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="59372-128">Любой пользователь, просматривающий или изМеняющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="59372-129">Шарепоинтинактиве</span><span class="sxs-lookup"><span data-stu-id="59372-129">sharePointInactive</span></span>       | <span data-ttu-id="59372-130">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-130">Int64</span></span>  | <span data-ttu-id="59372-131">Количество неактивных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="59372-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="59372-132">Скипефорбусинессактиве</span><span class="sxs-lookup"><span data-stu-id="59372-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="59372-133">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-133">Int64</span></span>  | <span data-ttu-id="59372-134">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="59372-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="59372-135">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="59372-136">Скипефорбусинессинактиве</span><span class="sxs-lookup"><span data-stu-id="59372-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="59372-137">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-137">Int64</span></span>  | <span data-ttu-id="59372-138">Количество неактивных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="59372-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="59372-139">Яммерактиве</span><span class="sxs-lookup"><span data-stu-id="59372-139">yammerActive</span></span>             | <span data-ttu-id="59372-140">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-140">Int64</span></span>  | <span data-ttu-id="59372-141">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="59372-141">The number of active users on Yammer.</span></span> <span data-ttu-id="59372-142">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="59372-143">Яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="59372-143">yammerInactive</span></span>           | <span data-ttu-id="59372-144">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-144">Int64</span></span>  | <span data-ttu-id="59372-145">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="59372-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="59372-146">Теамсактиве</span><span class="sxs-lookup"><span data-stu-id="59372-146">teamsActive</span></span>              | <span data-ttu-id="59372-147">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-147">Int64</span></span>  | <span data-ttu-id="59372-148">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="59372-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="59372-149">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="59372-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="59372-150">Теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="59372-150">teamsInactive</span></span>            | <span data-ttu-id="59372-151">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-151">Int64</span></span>  | <span data-ttu-id="59372-152">Количество неактивных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="59372-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="59372-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="59372-153">office365Active</span></span>          | <span data-ttu-id="59372-154">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-154">Int64</span></span>  | <span data-ttu-id="59372-155">Количество активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="59372-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="59372-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="59372-156">office365Inactive</span></span>        | <span data-ttu-id="59372-157">Int64</span><span class="sxs-lookup"><span data-stu-id="59372-157">Int64</span></span>  | <span data-ttu-id="59372-158">Количество неактивных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="59372-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="59372-159">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="59372-159">reportPeriod</span></span>             | <span data-ttu-id="59372-160">String</span><span class="sxs-lookup"><span data-stu-id="59372-160">String</span></span> | <span data-ttu-id="59372-161">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="59372-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="59372-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59372-162">JSON representation</span></span>

<span data-ttu-id="59372-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59372-163">The following is a JSON representation of the resource.</span></span>

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
