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
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="116e0-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="116e0-103">managementAgentType enum type</span></span>

<span data-ttu-id="116e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="116e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="116e0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="116e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116e0-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="116e0-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="116e0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="116e0-107">Members</span></span>
|<span data-ttu-id="116e0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="116e0-108">Member</span></span>|<span data-ttu-id="116e0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="116e0-109">Value</span></span>|<span data-ttu-id="116e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="116e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116e0-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="116e0-111">eas</span></span>|<span data-ttu-id="116e0-112">1,1</span><span class="sxs-lookup"><span data-stu-id="116e0-112">1</span></span>|<span data-ttu-id="116e0-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="116e0-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="116e0-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="116e0-114">mdm</span></span>|<span data-ttu-id="116e0-115">2</span><span class="sxs-lookup"><span data-stu-id="116e0-115">2</span></span>|<span data-ttu-id="116e0-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="116e0-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="116e0-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="116e0-117">easMdm</span></span>|<span data-ttu-id="116e0-118">4</span><span class="sxs-lookup"><span data-stu-id="116e0-118">3</span></span>|<span data-ttu-id="116e0-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="116e0-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="116e0-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="116e0-120">intuneClient</span></span>|<span data-ttu-id="116e0-121">4 </span><span class="sxs-lookup"><span data-stu-id="116e0-121">4</span></span>|<span data-ttu-id="116e0-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="116e0-122">Intune client managed.</span></span>|
|<span data-ttu-id="116e0-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="116e0-123">easIntuneClient</span></span>|<span data-ttu-id="116e0-124">5 </span><span class="sxs-lookup"><span data-stu-id="116e0-124">5</span></span>|<span data-ttu-id="116e0-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="116e0-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="116e0-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="116e0-126">configurationManagerClient</span></span>|<span data-ttu-id="116e0-127">8 </span><span class="sxs-lookup"><span data-stu-id="116e0-127">8</span></span>|<span data-ttu-id="116e0-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="116e0-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="116e0-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="116e0-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="116e0-130">10 </span><span class="sxs-lookup"><span data-stu-id="116e0-130">10</span></span>|<span data-ttu-id="116e0-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="116e0-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="116e0-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="116e0-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="116e0-133">11 </span><span class="sxs-lookup"><span data-stu-id="116e0-133">11</span></span>|<span data-ttu-id="116e0-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="116e0-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="116e0-135">unknown</span><span class="sxs-lookup"><span data-stu-id="116e0-135">unknown</span></span>|<span data-ttu-id="116e0-136">16 </span><span class="sxs-lookup"><span data-stu-id="116e0-136">16</span></span>|<span data-ttu-id="116e0-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="116e0-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="116e0-138">жамф</span><span class="sxs-lookup"><span data-stu-id="116e0-138">jamf</span></span>|<span data-ttu-id="116e0-139">32</span><span class="sxs-lookup"><span data-stu-id="116e0-139">32</span></span>|<span data-ttu-id="116e0-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="116e0-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="116e0-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="116e0-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="116e0-142">64</span><span class="sxs-lookup"><span data-stu-id="116e0-142">64</span></span>|<span data-ttu-id="116e0-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="116e0-143">The device is managed by Google's CloudDPC.</span></span>|







