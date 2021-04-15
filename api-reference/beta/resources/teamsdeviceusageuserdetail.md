---
title: тип ресурса teamsDeviceUsageUserDetail
description: Представляет сведения об использовании устройства Microsoft Teams пользователем.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766058"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7edcc-103">тип ресурса teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7edcc-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="7edcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7edcc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7edcc-105">Представляет сведения об использовании устройства Microsoft Teams пользователем.</span><span class="sxs-lookup"><span data-stu-id="7edcc-105">Represents details about Microsoft Teams device usage by user.</span></span>

## <a name="properties"></a><span data-ttu-id="7edcc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7edcc-106">Properties</span></span>

| <span data-ttu-id="7edcc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7edcc-107">Property</span></span>          | <span data-ttu-id="7edcc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7edcc-108">Type</span></span>    | <span data-ttu-id="7edcc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7edcc-109">Description</span></span>                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| <span data-ttu-id="7edcc-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7edcc-110">reportRefreshDate</span></span> | <span data-ttu-id="7edcc-111">Дата</span><span class="sxs-lookup"><span data-stu-id="7edcc-111">Date</span></span>    | <span data-ttu-id="7edcc-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="7edcc-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="7edcc-113">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7edcc-113">userPrincipalName</span></span> | <span data-ttu-id="7edcc-114">String</span><span class="sxs-lookup"><span data-stu-id="7edcc-114">String</span></span>  | <span data-ttu-id="7edcc-115">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="7edcc-115">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="7edcc-116">Это имя для входа через Интернет по стандарту RFC 822.</span><span class="sxs-lookup"><span data-stu-id="7edcc-116">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="7edcc-117">В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7edcc-117">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="7edcc-118">Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента.</span><span class="sxs-lookup"><span data-stu-id="7edcc-118">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="7edcc-119">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="7edcc-119">This property is required when a user is created.</span></span> |
| <span data-ttu-id="7edcc-120">isLicensed</span><span class="sxs-lookup"><span data-stu-id="7edcc-120">isLicensed</span></span>        | <span data-ttu-id="7edcc-121">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-121">Boolean</span></span> | <span data-ttu-id="7edcc-122">Назначена ли пользователю лицензия Teams.</span><span class="sxs-lookup"><span data-stu-id="7edcc-122">Whether the user has been assigned a Teams license.</span></span>          |
| <span data-ttu-id="7edcc-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7edcc-123">lastActivityDate</span></span>  | <span data-ttu-id="7edcc-124">Дата</span><span class="sxs-lookup"><span data-stu-id="7edcc-124">Date</span></span>    | <span data-ttu-id="7edcc-125">Последняя дата участия пользователя в действии Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7edcc-125">The last date that the user participated in a Microsoft Teams activity.</span></span> |
| <span data-ttu-id="7edcc-126">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7edcc-126">isDeleted</span></span>         | <span data-ttu-id="7edcc-127">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-127">Boolean</span></span> | <span data-ttu-id="7edcc-128">Был ли этот пользователь удален или удален.</span><span class="sxs-lookup"><span data-stu-id="7edcc-128">Whether this user has been deleted or soft deleted.</span></span>          |
| <span data-ttu-id="7edcc-129">deletedDate</span><span class="sxs-lookup"><span data-stu-id="7edcc-129">deletedDate</span></span>       | <span data-ttu-id="7edcc-130">Дата</span><span class="sxs-lookup"><span data-stu-id="7edcc-130">Date</span></span>    | <span data-ttu-id="7edcc-131">Дата, когда произошла операция удаления.</span><span class="sxs-lookup"><span data-stu-id="7edcc-131">The date when the delete operation happened.</span></span> <span data-ttu-id="7edcc-132">Значение по умолчанию — "null", если пользователь не удален.</span><span class="sxs-lookup"><span data-stu-id="7edcc-132">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="7edcc-133">usedWeb</span><span class="sxs-lookup"><span data-stu-id="7edcc-133">usedWeb</span></span>           | <span data-ttu-id="7edcc-134">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-134">Boolean</span></span> | <span data-ttu-id="7edcc-135">Был ли пользователь активен в веб-клиенте Teams на устройствах.</span><span class="sxs-lookup"><span data-stu-id="7edcc-135">Whether the user was active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="7edcc-136">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7edcc-136">usedWindowsPhone</span></span>  | <span data-ttu-id="7edcc-137">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-137">Boolean</span></span> | <span data-ttu-id="7edcc-138">Был ли пользователь активен в мобильном клиенте Teams для windows phone.</span><span class="sxs-lookup"><span data-stu-id="7edcc-138">Whether the user was active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="7edcc-139">usediOS</span><span class="sxs-lookup"><span data-stu-id="7edcc-139">usediOS</span></span>           | <span data-ttu-id="7edcc-140">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-140">Boolean</span></span> | <span data-ttu-id="7edcc-141">Был ли пользователь активен в мобильном клиенте Teams для iOS.</span><span class="sxs-lookup"><span data-stu-id="7edcc-141">Whether the user was active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="7edcc-142">usedMac</span><span class="sxs-lookup"><span data-stu-id="7edcc-142">usedMac</span></span>           | <span data-ttu-id="7edcc-143">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-143">Boolean</span></span> | <span data-ttu-id="7edcc-144">Был ли пользователь активен в настольном клиенте Teams на компьютере macOS.</span><span class="sxs-lookup"><span data-stu-id="7edcc-144">Whether the user was active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="7edcc-145">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7edcc-145">usedAndroidPhone</span></span>  | <span data-ttu-id="7edcc-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-146">Boolean</span></span> | <span data-ttu-id="7edcc-147">Был ли пользователь активен в мобильном клиенте Teams для Android.</span><span class="sxs-lookup"><span data-stu-id="7edcc-147">Whether the user was active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="7edcc-148">usedWindows</span><span class="sxs-lookup"><span data-stu-id="7edcc-148">usedWindows</span></span>       | <span data-ttu-id="7edcc-149">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-149">Boolean</span></span> | <span data-ttu-id="7edcc-150">Был ли пользователь активен в настольном клиенте Teams на компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="7edcc-150">Whether the user was active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="7edcc-151">usedChromeOS</span><span class="sxs-lookup"><span data-stu-id="7edcc-151">usedChromeOS</span></span>      | <span data-ttu-id="7edcc-152">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-152">Boolean</span></span> | <span data-ttu-id="7edcc-153">Был ли пользователь активен в настольном клиенте Teams на компьютере ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="7edcc-153">Whether the user was active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="7edcc-154">usedLinux</span><span class="sxs-lookup"><span data-stu-id="7edcc-154">usedLinux</span></span>         | <span data-ttu-id="7edcc-155">Логический</span><span class="sxs-lookup"><span data-stu-id="7edcc-155">Boolean</span></span> | <span data-ttu-id="7edcc-156">Был ли пользователь активен в настольном клиенте Teams на компьютере Linux.</span><span class="sxs-lookup"><span data-stu-id="7edcc-156">Whether the user was active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="7edcc-157">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7edcc-157">reportPeriod</span></span>      | <span data-ttu-id="7edcc-158">String</span><span class="sxs-lookup"><span data-stu-id="7edcc-158">String</span></span>  | <span data-ttu-id="7edcc-159">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="7edcc-159">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="7edcc-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7edcc-160">JSON representation</span></span>

<span data-ttu-id="7edcc-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7edcc-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


