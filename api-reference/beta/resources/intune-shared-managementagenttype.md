---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6b10c92a2c09505d1e3c5031f1d9046cfa56cb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769012"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7376c-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="7376c-103">managementAgentType enum type</span></span>

> <span data-ttu-id="7376c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7376c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7376c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7376c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7376c-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7376c-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="7376c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7376c-107">Members</span></span>
|<span data-ttu-id="7376c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7376c-108">Member</span></span>|<span data-ttu-id="7376c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7376c-109">Value</span></span>|<span data-ttu-id="7376c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7376c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7376c-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="7376c-111">eas</span></span>|<span data-ttu-id="7376c-112">1,1</span><span class="sxs-lookup"><span data-stu-id="7376c-112">1</span></span>|<span data-ttu-id="7376c-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7376c-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7376c-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="7376c-114">mdm</span></span>|<span data-ttu-id="7376c-115">2</span><span class="sxs-lookup"><span data-stu-id="7376c-115">2</span></span>|<span data-ttu-id="7376c-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7376c-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7376c-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="7376c-117">easMdm</span></span>|<span data-ttu-id="7376c-118">4</span><span class="sxs-lookup"><span data-stu-id="7376c-118">3</span></span>|<span data-ttu-id="7376c-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7376c-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7376c-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="7376c-120">intuneClient</span></span>|<span data-ttu-id="7376c-121">4 </span><span class="sxs-lookup"><span data-stu-id="7376c-121">4</span></span>|<span data-ttu-id="7376c-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7376c-122">Intune client managed.</span></span>|
|<span data-ttu-id="7376c-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="7376c-123">easIntuneClient</span></span>|<span data-ttu-id="7376c-124">5 </span><span class="sxs-lookup"><span data-stu-id="7376c-124">5</span></span>|<span data-ttu-id="7376c-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7376c-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7376c-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="7376c-126">configurationManagerClient</span></span>|<span data-ttu-id="7376c-127">8 </span><span class="sxs-lookup"><span data-stu-id="7376c-127">8</span></span>|<span data-ttu-id="7376c-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="7376c-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7376c-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="7376c-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="7376c-130">10 </span><span class="sxs-lookup"><span data-stu-id="7376c-130">10</span></span>|<span data-ttu-id="7376c-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="7376c-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7376c-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="7376c-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7376c-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="7376c-133">11</span></span>|<span data-ttu-id="7376c-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="7376c-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7376c-135">unknown</span><span class="sxs-lookup"><span data-stu-id="7376c-135">unknown</span></span>|<span data-ttu-id="7376c-136">16 </span><span class="sxs-lookup"><span data-stu-id="7376c-136">16</span></span>|<span data-ttu-id="7376c-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7376c-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="7376c-138">жамф</span><span class="sxs-lookup"><span data-stu-id="7376c-138">jamf</span></span>|<span data-ttu-id="7376c-139">32</span><span class="sxs-lookup"><span data-stu-id="7376c-139">32</span></span>|<span data-ttu-id="7376c-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="7376c-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7376c-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="7376c-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7376c-142">64</span><span class="sxs-lookup"><span data-stu-id="7376c-142">64</span></span>|<span data-ttu-id="7376c-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="7376c-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="7376c-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="7376c-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="7376c-145">258</span><span class="sxs-lookup"><span data-stu-id="7376c-145">258</span></span>|<span data-ttu-id="7376c-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="7376c-146">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="7376c-147">виндовсманажементклаудапи</span><span class="sxs-lookup"><span data-stu-id="7376c-147">windowsManagementCloudApi</span></span>|<span data-ttu-id="7376c-148">512</span><span class="sxs-lookup"><span data-stu-id="7376c-148">512</span></span>|<span data-ttu-id="7376c-149">Это устройство управляется Cloud API управления Windows.</span><span class="sxs-lookup"><span data-stu-id="7376c-149">This device is managed by Windows Management Cloud API.</span></span>|



