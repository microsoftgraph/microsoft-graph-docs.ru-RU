---
title: тип enum managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a11300891ca4b12b15de26b5be929823b4a8ddf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751358"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="3504e-103">тип enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="3504e-103">managementAgentType enum type</span></span>

<span data-ttu-id="3504e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3504e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3504e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3504e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3504e-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="3504e-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="3504e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3504e-107">Members</span></span>
|<span data-ttu-id="3504e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3504e-108">Member</span></span>|<span data-ttu-id="3504e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3504e-109">Value</span></span>|<span data-ttu-id="3504e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3504e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3504e-111">eas</span><span class="sxs-lookup"><span data-stu-id="3504e-111">eas</span></span>|<span data-ttu-id="3504e-112">1</span><span class="sxs-lookup"><span data-stu-id="3504e-112">1</span></span>|<span data-ttu-id="3504e-113">Устройство управляется Exchange сервером.</span><span class="sxs-lookup"><span data-stu-id="3504e-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="3504e-114">mdm</span><span class="sxs-lookup"><span data-stu-id="3504e-114">mdm</span></span>|<span data-ttu-id="3504e-115">2</span><span class="sxs-lookup"><span data-stu-id="3504e-115">2</span></span>|<span data-ttu-id="3504e-116">Устройство управляется intune MDM.</span><span class="sxs-lookup"><span data-stu-id="3504e-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="3504e-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="3504e-117">easMdm</span></span>|<span data-ttu-id="3504e-118">3</span><span class="sxs-lookup"><span data-stu-id="3504e-118">3</span></span>|<span data-ttu-id="3504e-119">Устройство управляется как сервером Exchange, так и MDM Intune.</span><span class="sxs-lookup"><span data-stu-id="3504e-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="3504e-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="3504e-120">intuneClient</span></span>|<span data-ttu-id="3504e-121">4 </span><span class="sxs-lookup"><span data-stu-id="3504e-121">4</span></span>|<span data-ttu-id="3504e-122">Клиент Intune управляется.</span><span class="sxs-lookup"><span data-stu-id="3504e-122">Intune client managed.</span></span>|
|<span data-ttu-id="3504e-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="3504e-123">easIntuneClient</span></span>|<span data-ttu-id="3504e-124">5 </span><span class="sxs-lookup"><span data-stu-id="3504e-124">5</span></span>|<span data-ttu-id="3504e-125">Устройство является двойным управляемым клиентом EAS и Intune.</span><span class="sxs-lookup"><span data-stu-id="3504e-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="3504e-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="3504e-126">configurationManagerClient</span></span>|<span data-ttu-id="3504e-127">8 </span><span class="sxs-lookup"><span data-stu-id="3504e-127">8</span></span>|<span data-ttu-id="3504e-128">Устройство управляется диспетчером конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3504e-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="3504e-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="3504e-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="3504e-130">10 </span><span class="sxs-lookup"><span data-stu-id="3504e-130">10</span></span>|<span data-ttu-id="3504e-131">Устройство управляется диспетчером конфигурации и MDM.</span><span class="sxs-lookup"><span data-stu-id="3504e-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="3504e-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="3504e-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="3504e-133">11</span><span class="sxs-lookup"><span data-stu-id="3504e-133">11</span></span>|<span data-ttu-id="3504e-134">Устройство управляется диспетчером конфигурации, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="3504e-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="3504e-135">unknown</span><span class="sxs-lookup"><span data-stu-id="3504e-135">unknown</span></span>|<span data-ttu-id="3504e-136">16 </span><span class="sxs-lookup"><span data-stu-id="3504e-136">16</span></span>|<span data-ttu-id="3504e-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="3504e-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="3504e-138">jamf</span><span class="sxs-lookup"><span data-stu-id="3504e-138">jamf</span></span>|<span data-ttu-id="3504e-139">32</span><span class="sxs-lookup"><span data-stu-id="3504e-139">32</span></span>|<span data-ttu-id="3504e-140">Атрибуты устройства извлекаются из Jamf.</span><span class="sxs-lookup"><span data-stu-id="3504e-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="3504e-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="3504e-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="3504e-142">64</span><span class="sxs-lookup"><span data-stu-id="3504e-142">64</span></span>|<span data-ttu-id="3504e-143">Устройство управляется cloudDPC От Google.</span><span class="sxs-lookup"><span data-stu-id="3504e-143">The device is managed by Google's CloudDPC.</span></span>|




