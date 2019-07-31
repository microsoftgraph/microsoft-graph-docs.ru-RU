---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae96113e687d406f5c0342b3b71fd63ea6de9918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999754"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="c9d22-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="c9d22-103">managementAgentType enum type</span></span>

> <span data-ttu-id="c9d22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9d22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9d22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d22-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="c9d22-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="c9d22-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c9d22-107">Members</span></span>
|<span data-ttu-id="c9d22-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c9d22-108">Member</span></span>|<span data-ttu-id="c9d22-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c9d22-109">Value</span></span>|<span data-ttu-id="c9d22-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9d22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d22-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="c9d22-111">eas</span></span>|<span data-ttu-id="c9d22-112">1,1</span><span class="sxs-lookup"><span data-stu-id="c9d22-112">1</span></span>|<span data-ttu-id="c9d22-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="c9d22-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="c9d22-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="c9d22-114">mdm</span></span>|<span data-ttu-id="c9d22-115">2</span><span class="sxs-lookup"><span data-stu-id="c9d22-115">2</span></span>|<span data-ttu-id="c9d22-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="c9d22-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="c9d22-117">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="c9d22-117">easMdm</span></span>|<span data-ttu-id="c9d22-118">4</span><span class="sxs-lookup"><span data-stu-id="c9d22-118">3</span></span>|<span data-ttu-id="c9d22-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="c9d22-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="c9d22-120">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="c9d22-120">intuneClient</span></span>|<span data-ttu-id="c9d22-121">SP4</span><span class="sxs-lookup"><span data-stu-id="c9d22-121">4</span></span>|<span data-ttu-id="c9d22-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="c9d22-122">Intune client managed.</span></span>|
|<span data-ttu-id="c9d22-123">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="c9d22-123">easIntuneClient</span></span>|<span data-ttu-id="c9d22-124">17:00</span><span class="sxs-lookup"><span data-stu-id="c9d22-124">5</span></span>|<span data-ttu-id="c9d22-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="c9d22-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="c9d22-126">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="c9d22-126">configurationManagerClient</span></span>|<span data-ttu-id="c9d22-127">8 </span><span class="sxs-lookup"><span data-stu-id="c9d22-127">8</span></span>|<span data-ttu-id="c9d22-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c9d22-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="c9d22-129">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="c9d22-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="c9d22-130">10 </span><span class="sxs-lookup"><span data-stu-id="c9d22-130">10</span></span>|<span data-ttu-id="c9d22-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="c9d22-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="c9d22-132">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="c9d22-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="c9d22-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="c9d22-133">11</span></span>|<span data-ttu-id="c9d22-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="c9d22-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="c9d22-135">unknown</span><span class="sxs-lookup"><span data-stu-id="c9d22-135">unknown</span></span>|<span data-ttu-id="c9d22-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="c9d22-136">16</span></span>|<span data-ttu-id="c9d22-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="c9d22-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="c9d22-138">жамф</span><span class="sxs-lookup"><span data-stu-id="c9d22-138">jamf</span></span>|<span data-ttu-id="c9d22-139">32</span><span class="sxs-lookup"><span data-stu-id="c9d22-139">32</span></span>|<span data-ttu-id="c9d22-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="c9d22-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="c9d22-141">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="c9d22-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="c9d22-142">64</span><span class="sxs-lookup"><span data-stu-id="c9d22-142">64</span></span>|<span data-ttu-id="c9d22-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="c9d22-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="c9d22-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="c9d22-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="c9d22-145">258</span><span class="sxs-lookup"><span data-stu-id="c9d22-145">258</span></span>|<span data-ttu-id="c9d22-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="c9d22-146">This device is managed by Microsoft 365 through Intune.</span></span>|





