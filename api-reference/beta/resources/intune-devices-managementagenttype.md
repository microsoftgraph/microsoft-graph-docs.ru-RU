---
title: Тип перечисления managementAgentType
description: Тип агента управления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401007"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="82762-103">Тип перечисления managementAgentType</span><span class="sxs-lookup"><span data-stu-id="82762-103">managementAgentType enum type</span></span>

> <span data-ttu-id="82762-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82762-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82762-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82762-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82762-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82762-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82762-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="82762-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="82762-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="82762-108">Members</span></span>
|<span data-ttu-id="82762-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="82762-109">Member</span></span>|<span data-ttu-id="82762-110">Значение</span><span class="sxs-lookup"><span data-stu-id="82762-110">Value</span></span>|<span data-ttu-id="82762-111">Описание</span><span class="sxs-lookup"><span data-stu-id="82762-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82762-112">EAS</span><span class="sxs-lookup"><span data-stu-id="82762-112">eas</span></span>|<span data-ttu-id="82762-113">1</span><span class="sxs-lookup"><span data-stu-id="82762-113">1</span></span>|<span data-ttu-id="82762-114">Устройство управляется сервером Exchange server.</span><span class="sxs-lookup"><span data-stu-id="82762-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="82762-115">MDM</span><span class="sxs-lookup"><span data-stu-id="82762-115">mdm</span></span>|<span data-ttu-id="82762-116">2</span><span class="sxs-lookup"><span data-stu-id="82762-116">2</span></span>|<span data-ttu-id="82762-117">Устройство является управляемым путем MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="82762-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="82762-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="82762-118">easMdm</span></span>|<span data-ttu-id="82762-119">3</span><span class="sxs-lookup"><span data-stu-id="82762-119">3</span></span>|<span data-ttu-id="82762-120">Устройство управляется сервером Exchange server и Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="82762-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="82762-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="82762-121">intuneClient</span></span>|<span data-ttu-id="82762-122">4</span><span class="sxs-lookup"><span data-stu-id="82762-122">4</span></span>|<span data-ttu-id="82762-123">Управляемые клиентами Intune.</span><span class="sxs-lookup"><span data-stu-id="82762-123">Intune client managed.</span></span>|
|<span data-ttu-id="82762-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="82762-124">easIntuneClient</span></span>|<span data-ttu-id="82762-125">5</span><span class="sxs-lookup"><span data-stu-id="82762-125">5</span></span>|<span data-ttu-id="82762-126">Устройство является EAS и Intune двойной управляемые клиентами.</span><span class="sxs-lookup"><span data-stu-id="82762-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="82762-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="82762-127">configurationManagerClient</span></span>|<span data-ttu-id="82762-128">8</span><span class="sxs-lookup"><span data-stu-id="82762-128">8</span></span>|<span data-ttu-id="82762-129">Устройство является управляемым, диспетчер конфигураций.</span><span class="sxs-lookup"><span data-stu-id="82762-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="82762-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="82762-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="82762-131">10</span><span class="sxs-lookup"><span data-stu-id="82762-131">10</span></span>|<span data-ttu-id="82762-132">Устройство управляется Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="82762-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="82762-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="82762-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="82762-134">11</span><span class="sxs-lookup"><span data-stu-id="82762-134">11</span></span>|<span data-ttu-id="82762-135">Устройство является управляемым, диспетчер конфигураций, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="82762-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="82762-136">unknown</span><span class="sxs-lookup"><span data-stu-id="82762-136">unknown</span></span>|<span data-ttu-id="82762-137">16</span><span class="sxs-lookup"><span data-stu-id="82762-137">16</span></span>|<span data-ttu-id="82762-138">Тип агента управления UNKNOWN.</span><span class="sxs-lookup"><span data-stu-id="82762-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="82762-139">jamf</span><span class="sxs-lookup"><span data-stu-id="82762-139">jamf</span></span>|<span data-ttu-id="82762-140">32</span><span class="sxs-lookup"><span data-stu-id="82762-140">32</span></span>|<span data-ttu-id="82762-141">Атрибуты устройства полученные от Jamf.</span><span class="sxs-lookup"><span data-stu-id="82762-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="82762-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="82762-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="82762-143">64</span><span class="sxs-lookup"><span data-stu-id="82762-143">64</span></span>|<span data-ttu-id="82762-144">Устройство управляется CloudDPC компании Google.</span><span class="sxs-lookup"><span data-stu-id="82762-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="82762-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="82762-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="82762-146">258</span><span class="sxs-lookup"><span data-stu-id="82762-146">258</span></span>|<span data-ttu-id="82762-147">Это устройство управляется Microsoft 365 через Intune.</span><span class="sxs-lookup"><span data-stu-id="82762-147">This device is managed by Microsoft 365 through Intune.</span></span>|




