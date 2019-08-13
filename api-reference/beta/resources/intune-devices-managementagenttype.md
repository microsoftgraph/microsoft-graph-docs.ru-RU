---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 630a3825367cc1850e6793598010a7fdbb027016
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372169"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="763e2-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="763e2-103">managementAgentType enum type</span></span>

> <span data-ttu-id="763e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="763e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="763e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="763e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="763e2-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="763e2-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="763e2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="763e2-107">Members</span></span>
|<span data-ttu-id="763e2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="763e2-108">Member</span></span>|<span data-ttu-id="763e2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="763e2-109">Value</span></span>|<span data-ttu-id="763e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="763e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="763e2-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="763e2-111">eas</span></span>|<span data-ttu-id="763e2-112">1,1</span><span class="sxs-lookup"><span data-stu-id="763e2-112">1</span></span>|<span data-ttu-id="763e2-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="763e2-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="763e2-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="763e2-114">mdm</span></span>|<span data-ttu-id="763e2-115">2</span><span class="sxs-lookup"><span data-stu-id="763e2-115">2</span></span>|<span data-ttu-id="763e2-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="763e2-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="763e2-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="763e2-117">easMdm</span></span>|<span data-ttu-id="763e2-118">4</span><span class="sxs-lookup"><span data-stu-id="763e2-118">3</span></span>|<span data-ttu-id="763e2-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="763e2-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="763e2-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="763e2-120">intuneClient</span></span>|<span data-ttu-id="763e2-121">SP4</span><span class="sxs-lookup"><span data-stu-id="763e2-121">4</span></span>|<span data-ttu-id="763e2-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="763e2-122">Intune client managed.</span></span>|
|<span data-ttu-id="763e2-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="763e2-123">easIntuneClient</span></span>|<span data-ttu-id="763e2-124">17:00</span><span class="sxs-lookup"><span data-stu-id="763e2-124">5</span></span>|<span data-ttu-id="763e2-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="763e2-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="763e2-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="763e2-126">configurationManagerClient</span></span>|<span data-ttu-id="763e2-127">8 </span><span class="sxs-lookup"><span data-stu-id="763e2-127">8</span></span>|<span data-ttu-id="763e2-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="763e2-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="763e2-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="763e2-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="763e2-130">10 </span><span class="sxs-lookup"><span data-stu-id="763e2-130">10</span></span>|<span data-ttu-id="763e2-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="763e2-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="763e2-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="763e2-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="763e2-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="763e2-133">11</span></span>|<span data-ttu-id="763e2-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="763e2-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="763e2-135">unknown</span><span class="sxs-lookup"><span data-stu-id="763e2-135">unknown</span></span>|<span data-ttu-id="763e2-136">столбцов</span><span class="sxs-lookup"><span data-stu-id="763e2-136">16</span></span>|<span data-ttu-id="763e2-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="763e2-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="763e2-138">жамф</span><span class="sxs-lookup"><span data-stu-id="763e2-138">jamf</span></span>|<span data-ttu-id="763e2-139">32</span><span class="sxs-lookup"><span data-stu-id="763e2-139">32</span></span>|<span data-ttu-id="763e2-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="763e2-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="763e2-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="763e2-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="763e2-142">64</span><span class="sxs-lookup"><span data-stu-id="763e2-142">64</span></span>|<span data-ttu-id="763e2-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="763e2-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="763e2-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="763e2-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="763e2-145">258</span><span class="sxs-lookup"><span data-stu-id="763e2-145">258</span></span>|<span data-ttu-id="763e2-146">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="763e2-146">This device is managed by Microsoft 365 through Intune.</span></span>|



