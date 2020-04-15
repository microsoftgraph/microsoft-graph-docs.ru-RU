---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d5f698a2878b0662193128044d7b069c8dfe8b3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406835"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="07f62-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="07f62-103">managementAgentType enum type</span></span>

<span data-ttu-id="07f62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07f62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07f62-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07f62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f62-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="07f62-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="07f62-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="07f62-107">Members</span></span>
|<span data-ttu-id="07f62-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="07f62-108">Member</span></span>|<span data-ttu-id="07f62-109">Значение</span><span class="sxs-lookup"><span data-stu-id="07f62-109">Value</span></span>|<span data-ttu-id="07f62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07f62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f62-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="07f62-111">eas</span></span>|<span data-ttu-id="07f62-112">1,1</span><span class="sxs-lookup"><span data-stu-id="07f62-112">1</span></span>|<span data-ttu-id="07f62-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="07f62-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="07f62-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="07f62-114">mdm</span></span>|<span data-ttu-id="07f62-115">2</span><span class="sxs-lookup"><span data-stu-id="07f62-115">2</span></span>|<span data-ttu-id="07f62-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="07f62-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="07f62-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="07f62-117">easMdm</span></span>|<span data-ttu-id="07f62-118">4</span><span class="sxs-lookup"><span data-stu-id="07f62-118">3</span></span>|<span data-ttu-id="07f62-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="07f62-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="07f62-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="07f62-120">intuneClient</span></span>|<span data-ttu-id="07f62-121">4 </span><span class="sxs-lookup"><span data-stu-id="07f62-121">4</span></span>|<span data-ttu-id="07f62-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="07f62-122">Intune client managed.</span></span>|
|<span data-ttu-id="07f62-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="07f62-123">easIntuneClient</span></span>|<span data-ttu-id="07f62-124">5 </span><span class="sxs-lookup"><span data-stu-id="07f62-124">5</span></span>|<span data-ttu-id="07f62-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="07f62-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="07f62-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="07f62-126">configurationManagerClient</span></span>|<span data-ttu-id="07f62-127">8 </span><span class="sxs-lookup"><span data-stu-id="07f62-127">8</span></span>|<span data-ttu-id="07f62-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="07f62-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="07f62-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="07f62-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="07f62-130">10 </span><span class="sxs-lookup"><span data-stu-id="07f62-130">10</span></span>|<span data-ttu-id="07f62-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="07f62-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="07f62-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="07f62-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="07f62-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="07f62-133">11</span></span>|<span data-ttu-id="07f62-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="07f62-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="07f62-135">unknown</span><span class="sxs-lookup"><span data-stu-id="07f62-135">unknown</span></span>|<span data-ttu-id="07f62-136">16 </span><span class="sxs-lookup"><span data-stu-id="07f62-136">16</span></span>|<span data-ttu-id="07f62-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="07f62-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="07f62-138">жамф</span><span class="sxs-lookup"><span data-stu-id="07f62-138">jamf</span></span>|<span data-ttu-id="07f62-139">32</span><span class="sxs-lookup"><span data-stu-id="07f62-139">32</span></span>|<span data-ttu-id="07f62-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="07f62-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="07f62-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="07f62-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="07f62-142">64</span><span class="sxs-lookup"><span data-stu-id="07f62-142">64</span></span>|<span data-ttu-id="07f62-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="07f62-143">The device is managed by Google's CloudDPC.</span></span>|







