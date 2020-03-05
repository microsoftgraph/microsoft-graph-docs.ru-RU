---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5305a0a6e2749851e1669d51310db52e5a587b86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523641"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f680a-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="f680a-103">managementAgentType enum type</span></span>

<span data-ttu-id="f680a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f680a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f680a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f680a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f680a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f680a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f680a-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f680a-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f680a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f680a-108">Members</span></span>
|<span data-ttu-id="f680a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f680a-109">Member</span></span>|<span data-ttu-id="f680a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f680a-110">Value</span></span>|<span data-ttu-id="f680a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f680a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f680a-112">атрибутов</span><span class="sxs-lookup"><span data-stu-id="f680a-112">eas</span></span>|<span data-ttu-id="f680a-113">1 </span><span class="sxs-lookup"><span data-stu-id="f680a-113">1</span></span>|<span data-ttu-id="f680a-114">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f680a-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f680a-115">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="f680a-115">mdm</span></span>|<span data-ttu-id="f680a-116">2 </span><span class="sxs-lookup"><span data-stu-id="f680a-116">2</span></span>|<span data-ttu-id="f680a-117">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f680a-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f680a-118">еасмдм</span><span class="sxs-lookup"><span data-stu-id="f680a-118">easMdm</span></span>|<span data-ttu-id="f680a-119">3 </span><span class="sxs-lookup"><span data-stu-id="f680a-119">3</span></span>|<span data-ttu-id="f680a-120">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="f680a-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f680a-121">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="f680a-121">intuneClient</span></span>|<span data-ttu-id="f680a-122">4 </span><span class="sxs-lookup"><span data-stu-id="f680a-122">4</span></span>|<span data-ttu-id="f680a-123">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f680a-123">Intune client managed.</span></span>|
|<span data-ttu-id="f680a-124">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="f680a-124">easIntuneClient</span></span>|<span data-ttu-id="f680a-125">5 </span><span class="sxs-lookup"><span data-stu-id="f680a-125">5</span></span>|<span data-ttu-id="f680a-126">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="f680a-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f680a-127">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="f680a-127">configurationManagerClient</span></span>|<span data-ttu-id="f680a-128">8 </span><span class="sxs-lookup"><span data-stu-id="f680a-128">8</span></span>|<span data-ttu-id="f680a-129">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f680a-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f680a-130">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="f680a-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="f680a-131">10 </span><span class="sxs-lookup"><span data-stu-id="f680a-131">10</span></span>|<span data-ttu-id="f680a-132">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="f680a-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f680a-133">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="f680a-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f680a-134">11 </span><span class="sxs-lookup"><span data-stu-id="f680a-134">11</span></span>|<span data-ttu-id="f680a-135">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="f680a-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f680a-136">unknown</span><span class="sxs-lookup"><span data-stu-id="f680a-136">unknown</span></span>|<span data-ttu-id="f680a-137">16 </span><span class="sxs-lookup"><span data-stu-id="f680a-137">16</span></span>|<span data-ttu-id="f680a-138">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="f680a-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="f680a-139">жамф</span><span class="sxs-lookup"><span data-stu-id="f680a-139">jamf</span></span>|<span data-ttu-id="f680a-140">32</span><span class="sxs-lookup"><span data-stu-id="f680a-140">32</span></span>|<span data-ttu-id="f680a-141">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="f680a-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f680a-142">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="f680a-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f680a-143">64</span><span class="sxs-lookup"><span data-stu-id="f680a-143">64</span></span>|<span data-ttu-id="f680a-144">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="f680a-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="f680a-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="f680a-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="f680a-146">258</span><span class="sxs-lookup"><span data-stu-id="f680a-146">258</span></span>|<span data-ttu-id="f680a-147">Это устройство управляется Microsoft 365 с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="f680a-147">This device is managed by Microsoft 365 through Intune.</span></span>|



