---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 34783f2c586e192d62cdeb0018b82e2df100c958
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466245"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="b387d-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="b387d-103">managementAgentType enum type</span></span>

<span data-ttu-id="b387d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b387d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b387d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b387d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b387d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b387d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b387d-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="b387d-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="b387d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b387d-108">Members</span></span>
|<span data-ttu-id="b387d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b387d-109">Member</span></span>|<span data-ttu-id="b387d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b387d-110">Value</span></span>|<span data-ttu-id="b387d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b387d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b387d-112">атрибутов</span><span class="sxs-lookup"><span data-stu-id="b387d-112">eas</span></span>|<span data-ttu-id="b387d-113">1,1</span><span class="sxs-lookup"><span data-stu-id="b387d-113">1</span></span>|<span data-ttu-id="b387d-114">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="b387d-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="b387d-115">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="b387d-115">mdm</span></span>|<span data-ttu-id="b387d-116">2</span><span class="sxs-lookup"><span data-stu-id="b387d-116">2</span></span>|<span data-ttu-id="b387d-117">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="b387d-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="b387d-118">еасмдм</span><span class="sxs-lookup"><span data-stu-id="b387d-118">easMdm</span></span>|<span data-ttu-id="b387d-119">4</span><span class="sxs-lookup"><span data-stu-id="b387d-119">3</span></span>|<span data-ttu-id="b387d-120">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="b387d-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="b387d-121">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="b387d-121">intuneClient</span></span>|<span data-ttu-id="b387d-122">4 </span><span class="sxs-lookup"><span data-stu-id="b387d-122">4</span></span>|<span data-ttu-id="b387d-123">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="b387d-123">Intune client managed.</span></span>|
|<span data-ttu-id="b387d-124">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="b387d-124">easIntuneClient</span></span>|<span data-ttu-id="b387d-125">5 </span><span class="sxs-lookup"><span data-stu-id="b387d-125">5</span></span>|<span data-ttu-id="b387d-126">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="b387d-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="b387d-127">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="b387d-127">configurationManagerClient</span></span>|<span data-ttu-id="b387d-128">8 </span><span class="sxs-lookup"><span data-stu-id="b387d-128">8</span></span>|<span data-ttu-id="b387d-129">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="b387d-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="b387d-130">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="b387d-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="b387d-131">10 </span><span class="sxs-lookup"><span data-stu-id="b387d-131">10</span></span>|<span data-ttu-id="b387d-132">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="b387d-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="b387d-133">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="b387d-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="b387d-134">-11:00</span><span class="sxs-lookup"><span data-stu-id="b387d-134">11</span></span>|<span data-ttu-id="b387d-135">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="b387d-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="b387d-136">unknown</span><span class="sxs-lookup"><span data-stu-id="b387d-136">unknown</span></span>|<span data-ttu-id="b387d-137">16 </span><span class="sxs-lookup"><span data-stu-id="b387d-137">16</span></span>|<span data-ttu-id="b387d-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="b387d-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="b387d-139">жамф</span><span class="sxs-lookup"><span data-stu-id="b387d-139">jamf</span></span>|<span data-ttu-id="b387d-140">32</span><span class="sxs-lookup"><span data-stu-id="b387d-140">32</span></span>|<span data-ttu-id="b387d-141">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="b387d-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="b387d-142">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="b387d-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="b387d-143">64</span><span class="sxs-lookup"><span data-stu-id="b387d-143">64</span></span>|<span data-ttu-id="b387d-144">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="b387d-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="b387d-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="b387d-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="b387d-146">258</span><span class="sxs-lookup"><span data-stu-id="b387d-146">258</span></span>|<span data-ttu-id="b387d-147">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="b387d-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="b387d-148">виндовсманажементклаудапи</span><span class="sxs-lookup"><span data-stu-id="b387d-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="b387d-149">512</span><span class="sxs-lookup"><span data-stu-id="b387d-149">512</span></span>|<span data-ttu-id="b387d-150">Это устройство управляется Cloud API управления Windows.</span><span class="sxs-lookup"><span data-stu-id="b387d-150">This device is managed by Windows Management Cloud API.</span></span>|



