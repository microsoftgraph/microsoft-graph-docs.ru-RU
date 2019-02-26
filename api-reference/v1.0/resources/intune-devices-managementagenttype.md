---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251568"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="e2c6a-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="e2c6a-103">managementAgentType enum type</span></span>

> <span data-ttu-id="e2c6a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2c6a-105">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="e2c6a-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e2c6a-106">Members</span></span>
|<span data-ttu-id="e2c6a-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e2c6a-107">Member</span></span>|<span data-ttu-id="e2c6a-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e2c6a-108">Value</span></span>|<span data-ttu-id="e2c6a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2c6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2c6a-110">атрибутов</span><span class="sxs-lookup"><span data-stu-id="e2c6a-110">eas</span></span>|<span data-ttu-id="e2c6a-111">1,1</span><span class="sxs-lookup"><span data-stu-id="e2c6a-111">1</span></span>|<span data-ttu-id="e2c6a-112">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="e2c6a-113">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="e2c6a-113">mdm</span></span>|<span data-ttu-id="e2c6a-114">2</span><span class="sxs-lookup"><span data-stu-id="e2c6a-114">2</span></span>|<span data-ttu-id="e2c6a-115">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="e2c6a-116">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="e2c6a-116">easMdm</span></span>|<span data-ttu-id="e2c6a-117">4</span><span class="sxs-lookup"><span data-stu-id="e2c6a-117">3</span></span>|<span data-ttu-id="e2c6a-118">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="e2c6a-119">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="e2c6a-119">intuneClient</span></span>|<span data-ttu-id="e2c6a-120">4</span><span class="sxs-lookup"><span data-stu-id="e2c6a-120">4</span></span>|<span data-ttu-id="e2c6a-121">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-121">Intune client managed.</span></span>|
|<span data-ttu-id="e2c6a-122">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="e2c6a-122">easIntuneClient</span></span>|<span data-ttu-id="e2c6a-123">17:00</span><span class="sxs-lookup"><span data-stu-id="e2c6a-123">5</span></span>|<span data-ttu-id="e2c6a-124">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="e2c6a-125">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="e2c6a-125">configurationManagerClient</span></span>|<span data-ttu-id="e2c6a-126">8,5</span><span class="sxs-lookup"><span data-stu-id="e2c6a-126">8</span></span>|<span data-ttu-id="e2c6a-127">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="e2c6a-128">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="e2c6a-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="e2c6a-129">десяти</span><span class="sxs-lookup"><span data-stu-id="e2c6a-129">10</span></span>|<span data-ttu-id="e2c6a-130">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="e2c6a-131">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="e2c6a-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="e2c6a-132">-11:00</span><span class="sxs-lookup"><span data-stu-id="e2c6a-132">11</span></span>|<span data-ttu-id="e2c6a-133">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="e2c6a-134">unknown</span><span class="sxs-lookup"><span data-stu-id="e2c6a-134">unknown</span></span>|<span data-ttu-id="e2c6a-135">столбцов</span><span class="sxs-lookup"><span data-stu-id="e2c6a-135">16</span></span>|<span data-ttu-id="e2c6a-136">НеИзвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="e2c6a-137">жамф</span><span class="sxs-lookup"><span data-stu-id="e2c6a-137">jamf</span></span>|<span data-ttu-id="e2c6a-138">32</span><span class="sxs-lookup"><span data-stu-id="e2c6a-138">32</span></span>|<span data-ttu-id="e2c6a-139">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="e2c6a-140">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="e2c6a-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="e2c6a-141">64</span><span class="sxs-lookup"><span data-stu-id="e2c6a-141">64</span></span>|<span data-ttu-id="e2c6a-142">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="e2c6a-142">The device is managed by Google's CloudDPC.</span></span>|



