---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8a40b8d6951c13da49766430fdd7fb303cbba0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775305"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ad418-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="ad418-103">managementAgentType enum type</span></span>

> <span data-ttu-id="ad418-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad418-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad418-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="ad418-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="ad418-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ad418-107">Members</span></span>
|<span data-ttu-id="ad418-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ad418-108">Member</span></span>|<span data-ttu-id="ad418-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ad418-109">Value</span></span>|<span data-ttu-id="ad418-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad418-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad418-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="ad418-111">eas</span></span>|<span data-ttu-id="ad418-112">1,1</span><span class="sxs-lookup"><span data-stu-id="ad418-112">1</span></span>|<span data-ttu-id="ad418-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ad418-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ad418-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="ad418-114">mdm</span></span>|<span data-ttu-id="ad418-115">2</span><span class="sxs-lookup"><span data-stu-id="ad418-115">2</span></span>|<span data-ttu-id="ad418-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="ad418-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ad418-117">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="ad418-117">easMdm</span></span>|<span data-ttu-id="ad418-118">4</span><span class="sxs-lookup"><span data-stu-id="ad418-118">3</span></span>|<span data-ttu-id="ad418-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="ad418-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ad418-120">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="ad418-120">intuneClient</span></span>|<span data-ttu-id="ad418-121">SP4</span><span class="sxs-lookup"><span data-stu-id="ad418-121">4</span></span>|<span data-ttu-id="ad418-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="ad418-122">Intune client managed.</span></span>|
|<span data-ttu-id="ad418-123">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="ad418-123">easIntuneClient</span></span>|<span data-ttu-id="ad418-124">17:00</span><span class="sxs-lookup"><span data-stu-id="ad418-124">5</span></span>|<span data-ttu-id="ad418-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="ad418-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ad418-126">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="ad418-126">configurationManagerClient</span></span>|<span data-ttu-id="ad418-127">8,5</span><span class="sxs-lookup"><span data-stu-id="ad418-127">8</span></span>|<span data-ttu-id="ad418-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ad418-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ad418-129">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="ad418-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="ad418-130">десяти</span><span class="sxs-lookup"><span data-stu-id="ad418-130">10</span></span>|<span data-ttu-id="ad418-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="ad418-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ad418-132">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="ad418-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ad418-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="ad418-133">11</span></span>|<span data-ttu-id="ad418-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="ad418-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ad418-135">unknown</span><span class="sxs-lookup"><span data-stu-id="ad418-135">unknown</span></span>|<span data-ttu-id="ad418-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="ad418-136">16</span></span>|<span data-ttu-id="ad418-137">НеИзвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="ad418-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="ad418-138">жамф</span><span class="sxs-lookup"><span data-stu-id="ad418-138">jamf</span></span>|<span data-ttu-id="ad418-139">32</span><span class="sxs-lookup"><span data-stu-id="ad418-139">32</span></span>|<span data-ttu-id="ad418-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="ad418-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ad418-141">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="ad418-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ad418-142">64</span><span class="sxs-lookup"><span data-stu-id="ad418-142">64</span></span>|<span data-ttu-id="ad418-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="ad418-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="ad418-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="ad418-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="ad418-145">258</span><span class="sxs-lookup"><span data-stu-id="ad418-145">258</span></span>|<span data-ttu-id="ad418-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="ad418-146">This device is managed by Microsoft 365 through Intune.</span></span>|





