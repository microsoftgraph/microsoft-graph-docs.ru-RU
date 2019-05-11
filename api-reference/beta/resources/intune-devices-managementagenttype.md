---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bb3c564366e2fa5c4be2c7c7ed75267a4d58275
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941928"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="c4f20-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="c4f20-103">managementAgentType enum type</span></span>

> <span data-ttu-id="c4f20-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4f20-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4f20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f20-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="c4f20-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="c4f20-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c4f20-107">Members</span></span>
|<span data-ttu-id="c4f20-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c4f20-108">Member</span></span>|<span data-ttu-id="c4f20-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c4f20-109">Value</span></span>|<span data-ttu-id="c4f20-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4f20-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="c4f20-111">eas</span></span>|<span data-ttu-id="c4f20-112">1,1</span><span class="sxs-lookup"><span data-stu-id="c4f20-112">1</span></span>|<span data-ttu-id="c4f20-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="c4f20-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="c4f20-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="c4f20-114">mdm</span></span>|<span data-ttu-id="c4f20-115">2</span><span class="sxs-lookup"><span data-stu-id="c4f20-115">2</span></span>|<span data-ttu-id="c4f20-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="c4f20-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="c4f20-117">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="c4f20-117">easMdm</span></span>|<span data-ttu-id="c4f20-118">4</span><span class="sxs-lookup"><span data-stu-id="c4f20-118">3</span></span>|<span data-ttu-id="c4f20-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="c4f20-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="c4f20-120">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="c4f20-120">intuneClient</span></span>|<span data-ttu-id="c4f20-121">SP4</span><span class="sxs-lookup"><span data-stu-id="c4f20-121">4</span></span>|<span data-ttu-id="c4f20-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="c4f20-122">Intune client managed.</span></span>|
|<span data-ttu-id="c4f20-123">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="c4f20-123">easIntuneClient</span></span>|<span data-ttu-id="c4f20-124">17:00</span><span class="sxs-lookup"><span data-stu-id="c4f20-124">5</span></span>|<span data-ttu-id="c4f20-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="c4f20-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="c4f20-126">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="c4f20-126">configurationManagerClient</span></span>|<span data-ttu-id="c4f20-127">8 </span><span class="sxs-lookup"><span data-stu-id="c4f20-127">8</span></span>|<span data-ttu-id="c4f20-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c4f20-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="c4f20-129">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="c4f20-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="c4f20-130">10 </span><span class="sxs-lookup"><span data-stu-id="c4f20-130">10</span></span>|<span data-ttu-id="c4f20-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="c4f20-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="c4f20-132">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="c4f20-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="c4f20-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="c4f20-133">11</span></span>|<span data-ttu-id="c4f20-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="c4f20-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="c4f20-135">unknown</span><span class="sxs-lookup"><span data-stu-id="c4f20-135">unknown</span></span>|<span data-ttu-id="c4f20-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="c4f20-136">16</span></span>|<span data-ttu-id="c4f20-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="c4f20-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="c4f20-138">жамф</span><span class="sxs-lookup"><span data-stu-id="c4f20-138">jamf</span></span>|<span data-ttu-id="c4f20-139">32</span><span class="sxs-lookup"><span data-stu-id="c4f20-139">32</span></span>|<span data-ttu-id="c4f20-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="c4f20-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="c4f20-141">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="c4f20-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="c4f20-142">64</span><span class="sxs-lookup"><span data-stu-id="c4f20-142">64</span></span>|<span data-ttu-id="c4f20-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="c4f20-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="c4f20-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="c4f20-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="c4f20-145">258</span><span class="sxs-lookup"><span data-stu-id="c4f20-145">258</span></span>|<span data-ttu-id="c4f20-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="c4f20-146">This device is managed by Microsoft 365 through Intune.</span></span>|




