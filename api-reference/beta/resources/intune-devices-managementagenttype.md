---
title: тип enum managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 331fd26e009fce708d13f4422c8eef0e6d19d0f8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612231"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="44e77-103">тип enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="44e77-103">managementAgentType enum type</span></span>

<span data-ttu-id="44e77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44e77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44e77-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44e77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44e77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44e77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44e77-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="44e77-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="44e77-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="44e77-108">Members</span></span>
|<span data-ttu-id="44e77-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="44e77-109">Member</span></span>|<span data-ttu-id="44e77-110">Значение</span><span class="sxs-lookup"><span data-stu-id="44e77-110">Value</span></span>|<span data-ttu-id="44e77-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44e77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e77-112">eas</span><span class="sxs-lookup"><span data-stu-id="44e77-112">eas</span></span>|<span data-ttu-id="44e77-113">1</span><span class="sxs-lookup"><span data-stu-id="44e77-113">1</span></span>|<span data-ttu-id="44e77-114">Устройство управляется сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="44e77-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="44e77-115">mdm</span><span class="sxs-lookup"><span data-stu-id="44e77-115">mdm</span></span>|<span data-ttu-id="44e77-116">2</span><span class="sxs-lookup"><span data-stu-id="44e77-116">2</span></span>|<span data-ttu-id="44e77-117">Устройство управляется intune MDM.</span><span class="sxs-lookup"><span data-stu-id="44e77-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="44e77-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="44e77-118">easMdm</span></span>|<span data-ttu-id="44e77-119">3</span><span class="sxs-lookup"><span data-stu-id="44e77-119">3</span></span>|<span data-ttu-id="44e77-120">Устройство управляется сервером Exchange и MDM Intune.</span><span class="sxs-lookup"><span data-stu-id="44e77-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="44e77-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="44e77-121">intuneClient</span></span>|<span data-ttu-id="44e77-122">4 </span><span class="sxs-lookup"><span data-stu-id="44e77-122">4</span></span>|<span data-ttu-id="44e77-123">Клиент Intune управляется.</span><span class="sxs-lookup"><span data-stu-id="44e77-123">Intune client managed.</span></span>|
|<span data-ttu-id="44e77-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="44e77-124">easIntuneClient</span></span>|<span data-ttu-id="44e77-125">5 </span><span class="sxs-lookup"><span data-stu-id="44e77-125">5</span></span>|<span data-ttu-id="44e77-126">Устройство является двойным управляемым клиентом EAS и Intune.</span><span class="sxs-lookup"><span data-stu-id="44e77-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="44e77-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="44e77-127">configurationManagerClient</span></span>|<span data-ttu-id="44e77-128">8 </span><span class="sxs-lookup"><span data-stu-id="44e77-128">8</span></span>|<span data-ttu-id="44e77-129">Устройство управляется диспетчером конфигурации.</span><span class="sxs-lookup"><span data-stu-id="44e77-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="44e77-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="44e77-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="44e77-131">10 </span><span class="sxs-lookup"><span data-stu-id="44e77-131">10</span></span>|<span data-ttu-id="44e77-132">Устройство управляется диспетчером конфигурации и MDM.</span><span class="sxs-lookup"><span data-stu-id="44e77-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="44e77-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="44e77-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="44e77-134">11</span><span class="sxs-lookup"><span data-stu-id="44e77-134">11</span></span>|<span data-ttu-id="44e77-135">Устройство управляется диспетчером конфигурации, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="44e77-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="44e77-136">unknown</span><span class="sxs-lookup"><span data-stu-id="44e77-136">unknown</span></span>|<span data-ttu-id="44e77-137">16 </span><span class="sxs-lookup"><span data-stu-id="44e77-137">16</span></span>|<span data-ttu-id="44e77-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="44e77-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="44e77-139">jamf</span><span class="sxs-lookup"><span data-stu-id="44e77-139">jamf</span></span>|<span data-ttu-id="44e77-140">32</span><span class="sxs-lookup"><span data-stu-id="44e77-140">32</span></span>|<span data-ttu-id="44e77-141">Атрибуты устройства извлекаются из Jamf.</span><span class="sxs-lookup"><span data-stu-id="44e77-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="44e77-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="44e77-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="44e77-143">64</span><span class="sxs-lookup"><span data-stu-id="44e77-143">64</span></span>|<span data-ttu-id="44e77-144">Устройство управляется cloudDPC От Google.</span><span class="sxs-lookup"><span data-stu-id="44e77-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="44e77-145">Microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="44e77-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="44e77-146">258</span><span class="sxs-lookup"><span data-stu-id="44e77-146">258</span></span>|<span data-ttu-id="44e77-147">Это устройство управляется Microsoft 365 через Intune.</span><span class="sxs-lookup"><span data-stu-id="44e77-147">This device is managed by Microsoft 365 through Intune.</span></span>|




