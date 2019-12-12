---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 630a3825367cc1850e6793598010a7fdbb027016
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955331"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="8a077-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="8a077-103">managementAgentType enum type</span></span>

> <span data-ttu-id="8a077-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a077-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a077-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="8a077-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="8a077-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8a077-107">Members</span></span>
|<span data-ttu-id="8a077-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8a077-108">Member</span></span>|<span data-ttu-id="8a077-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8a077-109">Value</span></span>|<span data-ttu-id="8a077-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a077-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a077-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="8a077-111">eas</span></span>|<span data-ttu-id="8a077-112">1,1</span><span class="sxs-lookup"><span data-stu-id="8a077-112">1</span></span>|<span data-ttu-id="8a077-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="8a077-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="8a077-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="8a077-114">mdm</span></span>|<span data-ttu-id="8a077-115">2</span><span class="sxs-lookup"><span data-stu-id="8a077-115">2</span></span>|<span data-ttu-id="8a077-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="8a077-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="8a077-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="8a077-117">easMdm</span></span>|<span data-ttu-id="8a077-118">4</span><span class="sxs-lookup"><span data-stu-id="8a077-118">3</span></span>|<span data-ttu-id="8a077-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="8a077-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="8a077-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="8a077-120">intuneClient</span></span>|<span data-ttu-id="8a077-121">4 </span><span class="sxs-lookup"><span data-stu-id="8a077-121">4</span></span>|<span data-ttu-id="8a077-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="8a077-122">Intune client managed.</span></span>|
|<span data-ttu-id="8a077-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="8a077-123">easIntuneClient</span></span>|<span data-ttu-id="8a077-124">5 </span><span class="sxs-lookup"><span data-stu-id="8a077-124">5</span></span>|<span data-ttu-id="8a077-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="8a077-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="8a077-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="8a077-126">configurationManagerClient</span></span>|<span data-ttu-id="8a077-127">8 </span><span class="sxs-lookup"><span data-stu-id="8a077-127">8</span></span>|<span data-ttu-id="8a077-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8a077-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="8a077-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="8a077-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="8a077-130">10 </span><span class="sxs-lookup"><span data-stu-id="8a077-130">10</span></span>|<span data-ttu-id="8a077-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="8a077-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="8a077-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="8a077-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="8a077-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="8a077-133">11</span></span>|<span data-ttu-id="8a077-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="8a077-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="8a077-135">unknown</span><span class="sxs-lookup"><span data-stu-id="8a077-135">unknown</span></span>|<span data-ttu-id="8a077-136">16 </span><span class="sxs-lookup"><span data-stu-id="8a077-136">16</span></span>|<span data-ttu-id="8a077-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="8a077-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="8a077-138">жамф</span><span class="sxs-lookup"><span data-stu-id="8a077-138">jamf</span></span>|<span data-ttu-id="8a077-139">32</span><span class="sxs-lookup"><span data-stu-id="8a077-139">32</span></span>|<span data-ttu-id="8a077-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="8a077-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="8a077-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="8a077-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="8a077-142">64</span><span class="sxs-lookup"><span data-stu-id="8a077-142">64</span></span>|<span data-ttu-id="8a077-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="8a077-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="8a077-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="8a077-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="8a077-145">258</span><span class="sxs-lookup"><span data-stu-id="8a077-145">258</span></span>|<span data-ttu-id="8a077-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="8a077-146">This device is managed by Microsoft 365 through Intune.</span></span>|



