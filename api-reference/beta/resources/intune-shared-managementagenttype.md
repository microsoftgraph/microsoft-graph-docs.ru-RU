---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 916e41c84b2c5ec740522c19b73f0c598f42184f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095102"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="877cd-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="877cd-103">managementAgentType enum type</span></span>

<span data-ttu-id="877cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="877cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="877cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="877cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="877cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="877cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="877cd-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="877cd-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="877cd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="877cd-108">Members</span></span>
|<span data-ttu-id="877cd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="877cd-109">Member</span></span>|<span data-ttu-id="877cd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="877cd-110">Value</span></span>|<span data-ttu-id="877cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="877cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="877cd-112">атрибутов</span><span class="sxs-lookup"><span data-stu-id="877cd-112">eas</span></span>|<span data-ttu-id="877cd-113">1 </span><span class="sxs-lookup"><span data-stu-id="877cd-113">1</span></span>|<span data-ttu-id="877cd-114">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="877cd-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="877cd-115">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="877cd-115">mdm</span></span>|<span data-ttu-id="877cd-116">2 </span><span class="sxs-lookup"><span data-stu-id="877cd-116">2</span></span>|<span data-ttu-id="877cd-117">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="877cd-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="877cd-118">еасмдм</span><span class="sxs-lookup"><span data-stu-id="877cd-118">easMdm</span></span>|<span data-ttu-id="877cd-119">4</span><span class="sxs-lookup"><span data-stu-id="877cd-119">3</span></span>|<span data-ttu-id="877cd-120">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="877cd-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="877cd-121">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="877cd-121">intuneClient</span></span>|<span data-ttu-id="877cd-122">4 </span><span class="sxs-lookup"><span data-stu-id="877cd-122">4</span></span>|<span data-ttu-id="877cd-123">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="877cd-123">Intune client managed.</span></span>|
|<span data-ttu-id="877cd-124">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="877cd-124">easIntuneClient</span></span>|<span data-ttu-id="877cd-125">5 </span><span class="sxs-lookup"><span data-stu-id="877cd-125">5</span></span>|<span data-ttu-id="877cd-126">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="877cd-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="877cd-127">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="877cd-127">configurationManagerClient</span></span>|<span data-ttu-id="877cd-128">8 </span><span class="sxs-lookup"><span data-stu-id="877cd-128">8</span></span>|<span data-ttu-id="877cd-129">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="877cd-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="877cd-130">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="877cd-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="877cd-131">10 </span><span class="sxs-lookup"><span data-stu-id="877cd-131">10</span></span>|<span data-ttu-id="877cd-132">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="877cd-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="877cd-133">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="877cd-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="877cd-134">11 </span><span class="sxs-lookup"><span data-stu-id="877cd-134">11</span></span>|<span data-ttu-id="877cd-135">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="877cd-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="877cd-136">unknown</span><span class="sxs-lookup"><span data-stu-id="877cd-136">unknown</span></span>|<span data-ttu-id="877cd-137">16 </span><span class="sxs-lookup"><span data-stu-id="877cd-137">16</span></span>|<span data-ttu-id="877cd-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="877cd-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="877cd-139">жамф</span><span class="sxs-lookup"><span data-stu-id="877cd-139">jamf</span></span>|<span data-ttu-id="877cd-140">32</span><span class="sxs-lookup"><span data-stu-id="877cd-140">32</span></span>|<span data-ttu-id="877cd-141">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="877cd-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="877cd-142">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="877cd-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="877cd-143">64</span><span class="sxs-lookup"><span data-stu-id="877cd-143">64</span></span>|<span data-ttu-id="877cd-144">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="877cd-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="877cd-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="877cd-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="877cd-146">258</span><span class="sxs-lookup"><span data-stu-id="877cd-146">258</span></span>|<span data-ttu-id="877cd-147">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="877cd-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="877cd-148">виндовсманажементклаудапи</span><span class="sxs-lookup"><span data-stu-id="877cd-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="877cd-149">512</span><span class="sxs-lookup"><span data-stu-id="877cd-149">512</span></span>|<span data-ttu-id="877cd-150">Это устройство управляется Cloud API управления Windows.</span><span class="sxs-lookup"><span data-stu-id="877cd-150">This device is managed by Windows Management Cloud API.</span></span>|






