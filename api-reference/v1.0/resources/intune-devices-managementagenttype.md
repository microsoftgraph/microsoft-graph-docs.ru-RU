---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a5835a0a8ca83cef2d5590679ce8aa4e77b0859
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530289"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="b47ce-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="b47ce-103">managementAgentType enum type</span></span>

<span data-ttu-id="b47ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b47ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b47ce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b47ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b47ce-106">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="b47ce-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="b47ce-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b47ce-107">Members</span></span>
|<span data-ttu-id="b47ce-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b47ce-108">Member</span></span>|<span data-ttu-id="b47ce-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b47ce-109">Value</span></span>|<span data-ttu-id="b47ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b47ce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b47ce-111">атрибутов</span><span class="sxs-lookup"><span data-stu-id="b47ce-111">eas</span></span>|<span data-ttu-id="b47ce-112">1 </span><span class="sxs-lookup"><span data-stu-id="b47ce-112">1</span></span>|<span data-ttu-id="b47ce-113">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="b47ce-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="b47ce-114">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="b47ce-114">mdm</span></span>|<span data-ttu-id="b47ce-115">2 </span><span class="sxs-lookup"><span data-stu-id="b47ce-115">2</span></span>|<span data-ttu-id="b47ce-116">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="b47ce-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="b47ce-117">еасмдм</span><span class="sxs-lookup"><span data-stu-id="b47ce-117">easMdm</span></span>|<span data-ttu-id="b47ce-118">3 </span><span class="sxs-lookup"><span data-stu-id="b47ce-118">3</span></span>|<span data-ttu-id="b47ce-119">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="b47ce-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="b47ce-120">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="b47ce-120">intuneClient</span></span>|<span data-ttu-id="b47ce-121">4 </span><span class="sxs-lookup"><span data-stu-id="b47ce-121">4</span></span>|<span data-ttu-id="b47ce-122">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="b47ce-122">Intune client managed.</span></span>|
|<span data-ttu-id="b47ce-123">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="b47ce-123">easIntuneClient</span></span>|<span data-ttu-id="b47ce-124">5 </span><span class="sxs-lookup"><span data-stu-id="b47ce-124">5</span></span>|<span data-ttu-id="b47ce-125">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="b47ce-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="b47ce-126">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="b47ce-126">configurationManagerClient</span></span>|<span data-ttu-id="b47ce-127">8 </span><span class="sxs-lookup"><span data-stu-id="b47ce-127">8</span></span>|<span data-ttu-id="b47ce-128">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="b47ce-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="b47ce-129">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="b47ce-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="b47ce-130">10 </span><span class="sxs-lookup"><span data-stu-id="b47ce-130">10</span></span>|<span data-ttu-id="b47ce-131">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="b47ce-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="b47ce-132">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="b47ce-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="b47ce-133">-11:00</span><span class="sxs-lookup"><span data-stu-id="b47ce-133">11</span></span>|<span data-ttu-id="b47ce-134">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="b47ce-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="b47ce-135">unknown</span><span class="sxs-lookup"><span data-stu-id="b47ce-135">unknown</span></span>|<span data-ttu-id="b47ce-136">16 </span><span class="sxs-lookup"><span data-stu-id="b47ce-136">16</span></span>|<span data-ttu-id="b47ce-137">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="b47ce-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="b47ce-138">жамф</span><span class="sxs-lookup"><span data-stu-id="b47ce-138">jamf</span></span>|<span data-ttu-id="b47ce-139">32</span><span class="sxs-lookup"><span data-stu-id="b47ce-139">32</span></span>|<span data-ttu-id="b47ce-140">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="b47ce-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="b47ce-141">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="b47ce-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="b47ce-142">64</span><span class="sxs-lookup"><span data-stu-id="b47ce-142">64</span></span>|<span data-ttu-id="b47ce-143">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="b47ce-143">The device is managed by Google's CloudDPC.</span></span>|




