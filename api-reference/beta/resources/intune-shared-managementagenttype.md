---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e769cd3f270a8ca1d00b6272a90154b925cc771d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48681959"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="1a695-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="1a695-103">managementAgentType enum type</span></span>

<span data-ttu-id="1a695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a695-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a695-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a695-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a695-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a695-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="1a695-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="1a695-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1a695-108">Members</span></span>
|<span data-ttu-id="1a695-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1a695-109">Member</span></span>|<span data-ttu-id="1a695-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1a695-110">Value</span></span>|<span data-ttu-id="1a695-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a695-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a695-112">атрибутов</span><span class="sxs-lookup"><span data-stu-id="1a695-112">eas</span></span>|<span data-ttu-id="1a695-113">1,1</span><span class="sxs-lookup"><span data-stu-id="1a695-113">1</span></span>|<span data-ttu-id="1a695-114">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="1a695-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="1a695-115">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1a695-115">mdm</span></span>|<span data-ttu-id="1a695-116">2</span><span class="sxs-lookup"><span data-stu-id="1a695-116">2</span></span>|<span data-ttu-id="1a695-117">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="1a695-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="1a695-118">еасмдм</span><span class="sxs-lookup"><span data-stu-id="1a695-118">easMdm</span></span>|<span data-ttu-id="1a695-119">4</span><span class="sxs-lookup"><span data-stu-id="1a695-119">3</span></span>|<span data-ttu-id="1a695-120">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="1a695-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="1a695-121">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="1a695-121">intuneClient</span></span>|<span data-ttu-id="1a695-122">4 </span><span class="sxs-lookup"><span data-stu-id="1a695-122">4</span></span>|<span data-ttu-id="1a695-123">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="1a695-123">Intune client managed.</span></span>|
|<span data-ttu-id="1a695-124">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="1a695-124">easIntuneClient</span></span>|<span data-ttu-id="1a695-125">5 </span><span class="sxs-lookup"><span data-stu-id="1a695-125">5</span></span>|<span data-ttu-id="1a695-126">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="1a695-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="1a695-127">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="1a695-127">configurationManagerClient</span></span>|<span data-ttu-id="1a695-128">8 </span><span class="sxs-lookup"><span data-stu-id="1a695-128">8</span></span>|<span data-ttu-id="1a695-129">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="1a695-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="1a695-130">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="1a695-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="1a695-131">10 </span><span class="sxs-lookup"><span data-stu-id="1a695-131">10</span></span>|<span data-ttu-id="1a695-132">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="1a695-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="1a695-133">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="1a695-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="1a695-134">-11:00</span><span class="sxs-lookup"><span data-stu-id="1a695-134">11</span></span>|<span data-ttu-id="1a695-135">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="1a695-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="1a695-136">unknown</span><span class="sxs-lookup"><span data-stu-id="1a695-136">unknown</span></span>|<span data-ttu-id="1a695-137">16 </span><span class="sxs-lookup"><span data-stu-id="1a695-137">16</span></span>|<span data-ttu-id="1a695-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="1a695-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="1a695-139">жамф</span><span class="sxs-lookup"><span data-stu-id="1a695-139">jamf</span></span>|<span data-ttu-id="1a695-140">32</span><span class="sxs-lookup"><span data-stu-id="1a695-140">32</span></span>|<span data-ttu-id="1a695-141">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="1a695-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="1a695-142">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="1a695-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="1a695-143">64</span><span class="sxs-lookup"><span data-stu-id="1a695-143">64</span></span>|<span data-ttu-id="1a695-144">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="1a695-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="1a695-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="1a695-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="1a695-146">258</span><span class="sxs-lookup"><span data-stu-id="1a695-146">258</span></span>|<span data-ttu-id="1a695-147">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="1a695-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="1a695-148">виндовсманажементклаудапи</span><span class="sxs-lookup"><span data-stu-id="1a695-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="1a695-149">512</span><span class="sxs-lookup"><span data-stu-id="1a695-149">512</span></span>|<span data-ttu-id="1a695-150">Это устройство управляется Cloud API управления Windows.</span><span class="sxs-lookup"><span data-stu-id="1a695-150">This device is managed by Windows Management Cloud API.</span></span>|





