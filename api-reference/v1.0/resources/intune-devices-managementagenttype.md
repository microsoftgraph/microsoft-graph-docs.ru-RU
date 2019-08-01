---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b1aabb6b3e08abdd3230eaab6ef5d640f4f908fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027442"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="12480-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="12480-103">managementAgentType enum type</span></span>

> <span data-ttu-id="12480-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12480-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12480-105">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="12480-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="12480-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="12480-106">Members</span></span>
|<span data-ttu-id="12480-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="12480-107">Member</span></span>|<span data-ttu-id="12480-108">Значение</span><span class="sxs-lookup"><span data-stu-id="12480-108">Value</span></span>|<span data-ttu-id="12480-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12480-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12480-110">атрибутов</span><span class="sxs-lookup"><span data-stu-id="12480-110">eas</span></span>|<span data-ttu-id="12480-111">1,1</span><span class="sxs-lookup"><span data-stu-id="12480-111">1</span></span>|<span data-ttu-id="12480-112">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="12480-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="12480-113">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="12480-113">mdm</span></span>|<span data-ttu-id="12480-114">2</span><span class="sxs-lookup"><span data-stu-id="12480-114">2</span></span>|<span data-ttu-id="12480-115">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="12480-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="12480-116">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="12480-116">easMdm</span></span>|<span data-ttu-id="12480-117">4</span><span class="sxs-lookup"><span data-stu-id="12480-117">3</span></span>|<span data-ttu-id="12480-118">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="12480-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="12480-119">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="12480-119">intuneClient</span></span>|<span data-ttu-id="12480-120">SP4</span><span class="sxs-lookup"><span data-stu-id="12480-120">4</span></span>|<span data-ttu-id="12480-121">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="12480-121">Intune client managed.</span></span>|
|<span data-ttu-id="12480-122">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="12480-122">easIntuneClient</span></span>|<span data-ttu-id="12480-123">17:00</span><span class="sxs-lookup"><span data-stu-id="12480-123">5</span></span>|<span data-ttu-id="12480-124">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="12480-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="12480-125">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="12480-125">configurationManagerClient</span></span>|<span data-ttu-id="12480-126">8 </span><span class="sxs-lookup"><span data-stu-id="12480-126">8</span></span>|<span data-ttu-id="12480-127">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="12480-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="12480-128">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="12480-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="12480-129">10 </span><span class="sxs-lookup"><span data-stu-id="12480-129">10</span></span>|<span data-ttu-id="12480-130">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="12480-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="12480-131">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="12480-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="12480-132">-11:00</span><span class="sxs-lookup"><span data-stu-id="12480-132">11</span></span>|<span data-ttu-id="12480-133">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="12480-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="12480-134">unknown</span><span class="sxs-lookup"><span data-stu-id="12480-134">unknown</span></span>|<span data-ttu-id="12480-135">столбцов</span><span class="sxs-lookup"><span data-stu-id="12480-135">16</span></span>|<span data-ttu-id="12480-136">Неизвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="12480-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="12480-137">жамф</span><span class="sxs-lookup"><span data-stu-id="12480-137">jamf</span></span>|<span data-ttu-id="12480-138">32</span><span class="sxs-lookup"><span data-stu-id="12480-138">32</span></span>|<span data-ttu-id="12480-139">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="12480-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="12480-140">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="12480-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="12480-141">64</span><span class="sxs-lookup"><span data-stu-id="12480-141">64</span></span>|<span data-ttu-id="12480-142">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="12480-142">The device is managed by Google's CloudDPC.</span></span>|



