---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66441a37b417cef13cbb09219a26a98250cbf610
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888489"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="41cbb-103">Тип перечисления managementAgentType</span><span class="sxs-lookup"><span data-stu-id="41cbb-103">managementAgentType enum type</span></span>

> <span data-ttu-id="41cbb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="41cbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41cbb-105">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="41cbb-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="41cbb-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="41cbb-106">Members</span></span>
|<span data-ttu-id="41cbb-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="41cbb-107">Member</span></span>|<span data-ttu-id="41cbb-108">Значение</span><span class="sxs-lookup"><span data-stu-id="41cbb-108">Value</span></span>|<span data-ttu-id="41cbb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="41cbb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41cbb-110">EAS</span><span class="sxs-lookup"><span data-stu-id="41cbb-110">eas</span></span>|<span data-ttu-id="41cbb-111">1</span><span class="sxs-lookup"><span data-stu-id="41cbb-111">1</span></span>|<span data-ttu-id="41cbb-112">Устройство управляется сервером Exchange server.</span><span class="sxs-lookup"><span data-stu-id="41cbb-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="41cbb-113">MDM</span><span class="sxs-lookup"><span data-stu-id="41cbb-113">mdm</span></span>|<span data-ttu-id="41cbb-114">2</span><span class="sxs-lookup"><span data-stu-id="41cbb-114">2</span></span>|<span data-ttu-id="41cbb-115">Устройство является управляемым путем MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="41cbb-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="41cbb-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="41cbb-116">easMdm</span></span>|<span data-ttu-id="41cbb-117">3</span><span class="sxs-lookup"><span data-stu-id="41cbb-117">3</span></span>|<span data-ttu-id="41cbb-118">Устройство управляется сервером Exchange server и Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="41cbb-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="41cbb-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="41cbb-119">intuneClient</span></span>|<span data-ttu-id="41cbb-120">4</span><span class="sxs-lookup"><span data-stu-id="41cbb-120">4</span></span>|<span data-ttu-id="41cbb-121">Управляемые клиентами Intune.</span><span class="sxs-lookup"><span data-stu-id="41cbb-121">Intune client managed.</span></span>|
|<span data-ttu-id="41cbb-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="41cbb-122">easIntuneClient</span></span>|<span data-ttu-id="41cbb-123">5</span><span class="sxs-lookup"><span data-stu-id="41cbb-123">5</span></span>|<span data-ttu-id="41cbb-124">Устройство является EAS и Intune двойной управляемые клиентами.</span><span class="sxs-lookup"><span data-stu-id="41cbb-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="41cbb-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="41cbb-125">configurationManagerClient</span></span>|<span data-ttu-id="41cbb-126">8</span><span class="sxs-lookup"><span data-stu-id="41cbb-126">8</span></span>|<span data-ttu-id="41cbb-127">Устройство является управляемым, диспетчер конфигураций.</span><span class="sxs-lookup"><span data-stu-id="41cbb-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="41cbb-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="41cbb-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="41cbb-129">10</span><span class="sxs-lookup"><span data-stu-id="41cbb-129">10</span></span>|<span data-ttu-id="41cbb-130">Устройство управляется Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="41cbb-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="41cbb-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="41cbb-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="41cbb-132">11</span><span class="sxs-lookup"><span data-stu-id="41cbb-132">11</span></span>|<span data-ttu-id="41cbb-133">Устройство является управляемым, диспетчер конфигураций, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="41cbb-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="41cbb-134">unknown</span><span class="sxs-lookup"><span data-stu-id="41cbb-134">unknown</span></span>|<span data-ttu-id="41cbb-135">16</span><span class="sxs-lookup"><span data-stu-id="41cbb-135">16</span></span>|<span data-ttu-id="41cbb-136">Тип агента управления UNKNOWN.</span><span class="sxs-lookup"><span data-stu-id="41cbb-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="41cbb-137">jamf</span><span class="sxs-lookup"><span data-stu-id="41cbb-137">jamf</span></span>|<span data-ttu-id="41cbb-138">32</span><span class="sxs-lookup"><span data-stu-id="41cbb-138">32</span></span>|<span data-ttu-id="41cbb-139">Атрибуты устройства полученные от Jamf.</span><span class="sxs-lookup"><span data-stu-id="41cbb-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="41cbb-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="41cbb-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="41cbb-141">64</span><span class="sxs-lookup"><span data-stu-id="41cbb-141">64</span></span>|<span data-ttu-id="41cbb-142">Устройство управляется CloudDPC компании Google.</span><span class="sxs-lookup"><span data-stu-id="41cbb-142">The device is managed by Google's CloudDPC.</span></span>|



