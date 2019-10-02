---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df4f3cbe6237471548dced1c13cfef601cbe7965
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356914"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7b3de-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="7b3de-103">managementAgentType enum type</span></span>

> <span data-ttu-id="7b3de-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b3de-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3de-105">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7b3de-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="7b3de-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b3de-106">Members</span></span>
|<span data-ttu-id="7b3de-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b3de-107">Member</span></span>|<span data-ttu-id="7b3de-108">Значение</span><span class="sxs-lookup"><span data-stu-id="7b3de-108">Value</span></span>|<span data-ttu-id="7b3de-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7b3de-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3de-110">атрибутов</span><span class="sxs-lookup"><span data-stu-id="7b3de-110">eas</span></span>|<span data-ttu-id="7b3de-111">1,1</span><span class="sxs-lookup"><span data-stu-id="7b3de-111">1</span></span>|<span data-ttu-id="7b3de-112">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7b3de-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7b3de-113">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="7b3de-113">mdm</span></span>|<span data-ttu-id="7b3de-114">2</span><span class="sxs-lookup"><span data-stu-id="7b3de-114">2</span></span>|<span data-ttu-id="7b3de-115">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7b3de-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7b3de-116">еасмдм</span><span class="sxs-lookup"><span data-stu-id="7b3de-116">easMdm</span></span>|<span data-ttu-id="7b3de-117">4</span><span class="sxs-lookup"><span data-stu-id="7b3de-117">3</span></span>|<span data-ttu-id="7b3de-118">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="7b3de-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7b3de-119">интунеклиент</span><span class="sxs-lookup"><span data-stu-id="7b3de-119">intuneClient</span></span>|<span data-ttu-id="7b3de-120">SP4</span><span class="sxs-lookup"><span data-stu-id="7b3de-120">4</span></span>|<span data-ttu-id="7b3de-121">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7b3de-121">Intune client managed.</span></span>|
|<span data-ttu-id="7b3de-122">еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="7b3de-122">easIntuneClient</span></span>|<span data-ttu-id="7b3de-123">17:00</span><span class="sxs-lookup"><span data-stu-id="7b3de-123">5</span></span>|<span data-ttu-id="7b3de-124">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="7b3de-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7b3de-125">конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="7b3de-125">configurationManagerClient</span></span>|<span data-ttu-id="7b3de-126">8 </span><span class="sxs-lookup"><span data-stu-id="7b3de-126">8</span></span>|<span data-ttu-id="7b3de-127">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="7b3de-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7b3de-128">конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="7b3de-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="7b3de-129">10 </span><span class="sxs-lookup"><span data-stu-id="7b3de-129">10</span></span>|<span data-ttu-id="7b3de-130">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="7b3de-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7b3de-131">конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="7b3de-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7b3de-132">-11:00</span><span class="sxs-lookup"><span data-stu-id="7b3de-132">11</span></span>|<span data-ttu-id="7b3de-133">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="7b3de-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7b3de-134">unknown</span><span class="sxs-lookup"><span data-stu-id="7b3de-134">unknown</span></span>|<span data-ttu-id="7b3de-135">столбцов</span><span class="sxs-lookup"><span data-stu-id="7b3de-135">16</span></span>|<span data-ttu-id="7b3de-136">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="7b3de-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="7b3de-137">жамф</span><span class="sxs-lookup"><span data-stu-id="7b3de-137">jamf</span></span>|<span data-ttu-id="7b3de-138">32</span><span class="sxs-lookup"><span data-stu-id="7b3de-138">32</span></span>|<span data-ttu-id="7b3de-139">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="7b3de-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7b3de-140">гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="7b3de-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7b3de-141">64</span><span class="sxs-lookup"><span data-stu-id="7b3de-141">64</span></span>|<span data-ttu-id="7b3de-142">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="7b3de-142">The device is managed by Google's CloudDPC.</span></span>|




