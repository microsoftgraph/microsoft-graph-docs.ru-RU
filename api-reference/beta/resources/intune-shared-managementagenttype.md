---
title: тип enum managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8cd60cb8eb1b8ed4ac7bcd8fd321e0dbfdda084
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666340"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="40aae-103">тип enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="40aae-103">managementAgentType enum type</span></span>

<span data-ttu-id="40aae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40aae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40aae-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40aae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40aae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40aae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40aae-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="40aae-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="40aae-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="40aae-108">Members</span></span>
|<span data-ttu-id="40aae-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="40aae-109">Member</span></span>|<span data-ttu-id="40aae-110">Значение</span><span class="sxs-lookup"><span data-stu-id="40aae-110">Value</span></span>|<span data-ttu-id="40aae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="40aae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40aae-112">eas</span><span class="sxs-lookup"><span data-stu-id="40aae-112">eas</span></span>|<span data-ttu-id="40aae-113">1</span><span class="sxs-lookup"><span data-stu-id="40aae-113">1</span></span>|<span data-ttu-id="40aae-114">Устройство управляется Exchange сервером.</span><span class="sxs-lookup"><span data-stu-id="40aae-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="40aae-115">mdm</span><span class="sxs-lookup"><span data-stu-id="40aae-115">mdm</span></span>|<span data-ttu-id="40aae-116">2</span><span class="sxs-lookup"><span data-stu-id="40aae-116">2</span></span>|<span data-ttu-id="40aae-117">Устройство управляется intune MDM.</span><span class="sxs-lookup"><span data-stu-id="40aae-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="40aae-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="40aae-118">easMdm</span></span>|<span data-ttu-id="40aae-119">3</span><span class="sxs-lookup"><span data-stu-id="40aae-119">3</span></span>|<span data-ttu-id="40aae-120">Устройство управляется как сервером Exchange, так и MDM Intune.</span><span class="sxs-lookup"><span data-stu-id="40aae-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="40aae-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="40aae-121">intuneClient</span></span>|<span data-ttu-id="40aae-122">4 </span><span class="sxs-lookup"><span data-stu-id="40aae-122">4</span></span>|<span data-ttu-id="40aae-123">Клиент Intune управляется.</span><span class="sxs-lookup"><span data-stu-id="40aae-123">Intune client managed.</span></span>|
|<span data-ttu-id="40aae-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="40aae-124">easIntuneClient</span></span>|<span data-ttu-id="40aae-125">5 </span><span class="sxs-lookup"><span data-stu-id="40aae-125">5</span></span>|<span data-ttu-id="40aae-126">Устройство является двойным управляемым клиентом EAS и Intune.</span><span class="sxs-lookup"><span data-stu-id="40aae-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="40aae-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="40aae-127">configurationManagerClient</span></span>|<span data-ttu-id="40aae-128">8 </span><span class="sxs-lookup"><span data-stu-id="40aae-128">8</span></span>|<span data-ttu-id="40aae-129">Устройство управляется диспетчером конфигурации.</span><span class="sxs-lookup"><span data-stu-id="40aae-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="40aae-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="40aae-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="40aae-131">10 </span><span class="sxs-lookup"><span data-stu-id="40aae-131">10</span></span>|<span data-ttu-id="40aae-132">Устройство управляется диспетчером конфигурации и MDM.</span><span class="sxs-lookup"><span data-stu-id="40aae-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="40aae-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="40aae-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="40aae-134">11</span><span class="sxs-lookup"><span data-stu-id="40aae-134">11</span></span>|<span data-ttu-id="40aae-135">Устройство управляется диспетчером конфигурации, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="40aae-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="40aae-136">unknown</span><span class="sxs-lookup"><span data-stu-id="40aae-136">unknown</span></span>|<span data-ttu-id="40aae-137">16 </span><span class="sxs-lookup"><span data-stu-id="40aae-137">16</span></span>|<span data-ttu-id="40aae-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="40aae-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="40aae-139">jamf</span><span class="sxs-lookup"><span data-stu-id="40aae-139">jamf</span></span>|<span data-ttu-id="40aae-140">32</span><span class="sxs-lookup"><span data-stu-id="40aae-140">32</span></span>|<span data-ttu-id="40aae-141">Атрибуты устройства извлекаются из Jamf.</span><span class="sxs-lookup"><span data-stu-id="40aae-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="40aae-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="40aae-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="40aae-143">64</span><span class="sxs-lookup"><span data-stu-id="40aae-143">64</span></span>|<span data-ttu-id="40aae-144">Устройство управляется cloudDPC От Google.</span><span class="sxs-lookup"><span data-stu-id="40aae-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="40aae-145">Microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="40aae-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="40aae-146">258</span><span class="sxs-lookup"><span data-stu-id="40aae-146">258</span></span>|<span data-ttu-id="40aae-147">Это устройство управляется Microsoft 365 через Intune.</span><span class="sxs-lookup"><span data-stu-id="40aae-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="40aae-148">msSense</span><span class="sxs-lookup"><span data-stu-id="40aae-148">msSense</span></span>|<span data-ttu-id="40aae-149">1024</span><span class="sxs-lookup"><span data-stu-id="40aae-149">1024</span></span>|<span data-ttu-id="40aae-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="40aae-150">Not yet documented</span></span>|
|<span data-ttu-id="40aae-151">intuneAosp</span><span class="sxs-lookup"><span data-stu-id="40aae-151">intuneAosp</span></span>|<span data-ttu-id="40aae-152">2048</span><span class="sxs-lookup"><span data-stu-id="40aae-152">2048</span></span>|<span data-ttu-id="40aae-153">Это устройство управляется устройствами MDM intune для AOSP (Android Open Source Project)</span><span class="sxs-lookup"><span data-stu-id="40aae-153">This device is managed by Intune's MDM for AOSP (Android Open Source Project) devices</span></span>|
|<span data-ttu-id="40aae-154">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="40aae-154">windowsManagementCloudApi</span></span>|<span data-ttu-id="40aae-155">512</span><span class="sxs-lookup"><span data-stu-id="40aae-155">512</span></span>|<span data-ttu-id="40aae-156">Управление этим устройством Windows API облака управления.</span><span class="sxs-lookup"><span data-stu-id="40aae-156">This device is managed by Windows Management Cloud API.</span></span>|



