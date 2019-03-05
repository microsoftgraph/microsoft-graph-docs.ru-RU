---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb948626035bed2dac7ee18d103aa083bd0f2aeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172543"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f0cb5-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="f0cb5-103">managementAgentType enum type</span></span>

> <span data-ttu-id="f0cb5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0cb5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0cb5-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f0cb5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f0cb5-107">Members</span></span>
|<span data-ttu-id="f0cb5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f0cb5-108">Member</span></span>|<span data-ttu-id="f0cb5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f0cb5-109">Value</span></span>|<span data-ttu-id="f0cb5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0cb5-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="f0cb5-111">eas</span></span>|<span data-ttu-id="f0cb5-112">1,1</span><span class="sxs-lookup"><span data-stu-id="f0cb5-112">1</span></span>|<span data-ttu-id="f0cb5-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f0cb5-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="f0cb5-114">mdm</span></span>|<span data-ttu-id="f0cb5-115">2</span><span class="sxs-lookup"><span data-stu-id="f0cb5-115">2</span></span>|<span data-ttu-id="f0cb5-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f0cb5-117">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="f0cb5-117">easMdm</span></span>|<span data-ttu-id="f0cb5-118">4</span><span class="sxs-lookup"><span data-stu-id="f0cb5-118">3</span></span>|<span data-ttu-id="f0cb5-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f0cb5-120">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="f0cb5-120">intuneClient</span></span>|<span data-ttu-id="f0cb5-121">4</span><span class="sxs-lookup"><span data-stu-id="f0cb5-121">4</span></span>|<span data-ttu-id="f0cb5-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-122">Intune client managed.</span></span>|
|<span data-ttu-id="f0cb5-123">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="f0cb5-123">easIntuneClient</span></span>|<span data-ttu-id="f0cb5-124">17:00</span><span class="sxs-lookup"><span data-stu-id="f0cb5-124">5</span></span>|<span data-ttu-id="f0cb5-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f0cb5-126">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="f0cb5-126">configurationManagerClient</span></span>|<span data-ttu-id="f0cb5-127">8,5</span><span class="sxs-lookup"><span data-stu-id="f0cb5-127">8</span></span>|<span data-ttu-id="f0cb5-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f0cb5-129">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="f0cb5-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="f0cb5-130">десяти</span><span class="sxs-lookup"><span data-stu-id="f0cb5-130">10</span></span>|<span data-ttu-id="f0cb5-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f0cb5-132">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="f0cb5-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f0cb5-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="f0cb5-133">11</span></span>|<span data-ttu-id="f0cb5-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f0cb5-135">unknown</span><span class="sxs-lookup"><span data-stu-id="f0cb5-135">unknown</span></span>|<span data-ttu-id="f0cb5-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="f0cb5-136">16</span></span>|<span data-ttu-id="f0cb5-137">НеИзвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="f0cb5-138">жамф</span><span class="sxs-lookup"><span data-stu-id="f0cb5-138">jamf</span></span>|<span data-ttu-id="f0cb5-139">32</span><span class="sxs-lookup"><span data-stu-id="f0cb5-139">32</span></span>|<span data-ttu-id="f0cb5-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f0cb5-141">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="f0cb5-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f0cb5-142">64</span><span class="sxs-lookup"><span data-stu-id="f0cb5-142">64</span></span>|<span data-ttu-id="f0cb5-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="f0cb5-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="f0cb5-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="f0cb5-145">258</span><span class="sxs-lookup"><span data-stu-id="f0cb5-145">258</span></span>|<span data-ttu-id="f0cb5-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="f0cb5-146">This device is managed by Microsoft 365 through Intune.</span></span>|




