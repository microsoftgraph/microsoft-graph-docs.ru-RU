---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b9fd469a787e0afdacb26dc5a07ee114d72bbe
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986125"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f5e0a-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="f5e0a-103">managementAgentType enum type</span></span>

> <span data-ttu-id="f5e0a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5e0a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5e0a-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f5e0a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f5e0a-107">Members</span></span>
|<span data-ttu-id="f5e0a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f5e0a-108">Member</span></span>|<span data-ttu-id="f5e0a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f5e0a-109">Value</span></span>|<span data-ttu-id="f5e0a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5e0a-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="f5e0a-111">eas</span></span>|<span data-ttu-id="f5e0a-112">1,1</span><span class="sxs-lookup"><span data-stu-id="f5e0a-112">1</span></span>|<span data-ttu-id="f5e0a-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f5e0a-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="f5e0a-114">mdm</span></span>|<span data-ttu-id="f5e0a-115">2</span><span class="sxs-lookup"><span data-stu-id="f5e0a-115">2</span></span>|<span data-ttu-id="f5e0a-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f5e0a-117">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="f5e0a-117">easMdm</span></span>|<span data-ttu-id="f5e0a-118">4</span><span class="sxs-lookup"><span data-stu-id="f5e0a-118">3</span></span>|<span data-ttu-id="f5e0a-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f5e0a-120">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="f5e0a-120">intuneClient</span></span>|<span data-ttu-id="f5e0a-121">SP4</span><span class="sxs-lookup"><span data-stu-id="f5e0a-121">4</span></span>|<span data-ttu-id="f5e0a-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-122">Intune client managed.</span></span>|
|<span data-ttu-id="f5e0a-123">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="f5e0a-123">easIntuneClient</span></span>|<span data-ttu-id="f5e0a-124">17:00</span><span class="sxs-lookup"><span data-stu-id="f5e0a-124">5</span></span>|<span data-ttu-id="f5e0a-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f5e0a-126">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="f5e0a-126">configurationManagerClient</span></span>|<span data-ttu-id="f5e0a-127">8 </span><span class="sxs-lookup"><span data-stu-id="f5e0a-127">8</span></span>|<span data-ttu-id="f5e0a-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f5e0a-129">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="f5e0a-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="f5e0a-130">10 </span><span class="sxs-lookup"><span data-stu-id="f5e0a-130">10</span></span>|<span data-ttu-id="f5e0a-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f5e0a-132">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="f5e0a-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f5e0a-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="f5e0a-133">11</span></span>|<span data-ttu-id="f5e0a-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f5e0a-135">unknown</span><span class="sxs-lookup"><span data-stu-id="f5e0a-135">unknown</span></span>|<span data-ttu-id="f5e0a-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="f5e0a-136">16</span></span>|<span data-ttu-id="f5e0a-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="f5e0a-138">жамф</span><span class="sxs-lookup"><span data-stu-id="f5e0a-138">jamf</span></span>|<span data-ttu-id="f5e0a-139">32</span><span class="sxs-lookup"><span data-stu-id="f5e0a-139">32</span></span>|<span data-ttu-id="f5e0a-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f5e0a-141">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="f5e0a-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f5e0a-142">64</span><span class="sxs-lookup"><span data-stu-id="f5e0a-142">64</span></span>|<span data-ttu-id="f5e0a-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="f5e0a-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="f5e0a-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="f5e0a-145">258</span><span class="sxs-lookup"><span data-stu-id="f5e0a-145">258</span></span>|<span data-ttu-id="f5e0a-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="f5e0a-146">This device is managed by Microsoft 365 through Intune.</span></span>|





