---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 282915b085107d5367a0b7f8bd8f4f3ea84b7c23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258943"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7ee64-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="7ee64-103">managementAgentType enum type</span></span>

<span data-ttu-id="7ee64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ee64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ee64-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ee64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ee64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ee64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ee64-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7ee64-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="7ee64-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7ee64-108">Members</span></span>
|<span data-ttu-id="7ee64-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7ee64-109">Member</span></span>|<span data-ttu-id="7ee64-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7ee64-110">Value</span></span>|<span data-ttu-id="7ee64-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7ee64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ee64-112">атрибутов</span><span class="sxs-lookup"><span data-stu-id="7ee64-112">eas</span></span>|<span data-ttu-id="7ee64-113">1,1</span><span class="sxs-lookup"><span data-stu-id="7ee64-113">1</span></span>|<span data-ttu-id="7ee64-114">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7ee64-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7ee64-115">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="7ee64-115">mdm</span></span>|<span data-ttu-id="7ee64-116">2</span><span class="sxs-lookup"><span data-stu-id="7ee64-116">2</span></span>|<span data-ttu-id="7ee64-117">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7ee64-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7ee64-118">еасмдм</span><span class="sxs-lookup"><span data-stu-id="7ee64-118">easMdm</span></span>|<span data-ttu-id="7ee64-119">4</span><span class="sxs-lookup"><span data-stu-id="7ee64-119">3</span></span>|<span data-ttu-id="7ee64-120">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7ee64-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7ee64-121">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="7ee64-121">intuneClient</span></span>|<span data-ttu-id="7ee64-122">4 </span><span class="sxs-lookup"><span data-stu-id="7ee64-122">4</span></span>|<span data-ttu-id="7ee64-123">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7ee64-123">Intune client managed.</span></span>|
|<span data-ttu-id="7ee64-124">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="7ee64-124">easIntuneClient</span></span>|<span data-ttu-id="7ee64-125">5 </span><span class="sxs-lookup"><span data-stu-id="7ee64-125">5</span></span>|<span data-ttu-id="7ee64-126">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7ee64-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7ee64-127">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="7ee64-127">configurationManagerClient</span></span>|<span data-ttu-id="7ee64-128">8 </span><span class="sxs-lookup"><span data-stu-id="7ee64-128">8</span></span>|<span data-ttu-id="7ee64-129">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="7ee64-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7ee64-130">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="7ee64-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="7ee64-131">10 </span><span class="sxs-lookup"><span data-stu-id="7ee64-131">10</span></span>|<span data-ttu-id="7ee64-132">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="7ee64-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7ee64-133">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="7ee64-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7ee64-134">11 </span><span class="sxs-lookup"><span data-stu-id="7ee64-134">11</span></span>|<span data-ttu-id="7ee64-135">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="7ee64-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7ee64-136">unknown</span><span class="sxs-lookup"><span data-stu-id="7ee64-136">unknown</span></span>|<span data-ttu-id="7ee64-137">16 </span><span class="sxs-lookup"><span data-stu-id="7ee64-137">16</span></span>|<span data-ttu-id="7ee64-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7ee64-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="7ee64-139">жамф</span><span class="sxs-lookup"><span data-stu-id="7ee64-139">jamf</span></span>|<span data-ttu-id="7ee64-140">32</span><span class="sxs-lookup"><span data-stu-id="7ee64-140">32</span></span>|<span data-ttu-id="7ee64-141">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="7ee64-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7ee64-142">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="7ee64-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7ee64-143">64</span><span class="sxs-lookup"><span data-stu-id="7ee64-143">64</span></span>|<span data-ttu-id="7ee64-144">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="7ee64-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="7ee64-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="7ee64-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="7ee64-146">258</span><span class="sxs-lookup"><span data-stu-id="7ee64-146">258</span></span>|<span data-ttu-id="7ee64-147">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="7ee64-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="7ee64-148">виндовсманажементклаудапи</span><span class="sxs-lookup"><span data-stu-id="7ee64-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="7ee64-149">512</span><span class="sxs-lookup"><span data-stu-id="7ee64-149">512</span></span>|<span data-ttu-id="7ee64-150">Это устройство управляется Cloud API управления Windows.</span><span class="sxs-lookup"><span data-stu-id="7ee64-150">This device is managed by Windows Management Cloud API.</span></span>|




