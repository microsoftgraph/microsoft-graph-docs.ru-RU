---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522715"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="8f581-103">тип перечисления Манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="8f581-103">managementAgentType enum type</span></span>

> <span data-ttu-id="8f581-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f581-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f581-105">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="8f581-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="8f581-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f581-106">Members</span></span>
|<span data-ttu-id="8f581-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f581-107">Member</span></span>|<span data-ttu-id="8f581-108">Значение</span><span class="sxs-lookup"><span data-stu-id="8f581-108">Value</span></span>|<span data-ttu-id="8f581-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f581-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f581-110">атрибутов</span><span class="sxs-lookup"><span data-stu-id="8f581-110">eas</span></span>|<span data-ttu-id="8f581-111">1 </span><span class="sxs-lookup"><span data-stu-id="8f581-111">1</span></span>|<span data-ttu-id="8f581-112">Управление устройством осуществляется с помощью Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="8f581-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="8f581-113">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="8f581-113">mdm</span></span>|<span data-ttu-id="8f581-114">2 </span><span class="sxs-lookup"><span data-stu-id="8f581-114">2</span></span>|<span data-ttu-id="8f581-115">Управление устройством осуществляется с помощью Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="8f581-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="8f581-116">Еасмдм</span><span class="sxs-lookup"><span data-stu-id="8f581-116">easMdm</span></span>|<span data-ttu-id="8f581-117">3 </span><span class="sxs-lookup"><span data-stu-id="8f581-117">3</span></span>|<span data-ttu-id="8f581-118">Устройство управляется как в Exchange Server, так и в Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="8f581-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="8f581-119">Интунеклиент</span><span class="sxs-lookup"><span data-stu-id="8f581-119">intuneClient</span></span>|<span data-ttu-id="8f581-120">4 </span><span class="sxs-lookup"><span data-stu-id="8f581-120">4</span></span>|<span data-ttu-id="8f581-121">Управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="8f581-121">Intune client managed.</span></span>|
|<span data-ttu-id="8f581-122">Еасинтунеклиент</span><span class="sxs-lookup"><span data-stu-id="8f581-122">easIntuneClient</span></span>|<span data-ttu-id="8f581-123">5 </span><span class="sxs-lookup"><span data-stu-id="8f581-123">5</span></span>|<span data-ttu-id="8f581-124">Устройство — это EAS и двойное управление клиентом Intune.</span><span class="sxs-lookup"><span data-stu-id="8f581-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="8f581-125">Конфигуратионманажерклиент</span><span class="sxs-lookup"><span data-stu-id="8f581-125">configurationManagerClient</span></span>|<span data-ttu-id="8f581-126">8 </span><span class="sxs-lookup"><span data-stu-id="8f581-126">8</span></span>|<span data-ttu-id="8f581-127">Управление устройством осуществляется с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8f581-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="8f581-128">Конфигуратионманажерклиентмдм</span><span class="sxs-lookup"><span data-stu-id="8f581-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="8f581-129">10 </span><span class="sxs-lookup"><span data-stu-id="8f581-129">10</span></span>|<span data-ttu-id="8f581-130">Управление устройством осуществляется с помощью Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="8f581-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="8f581-131">Конфигуратионманажерклиентмдмеас</span><span class="sxs-lookup"><span data-stu-id="8f581-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="8f581-132">11 </span><span class="sxs-lookup"><span data-stu-id="8f581-132">11</span></span>|<span data-ttu-id="8f581-133">Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.</span><span class="sxs-lookup"><span data-stu-id="8f581-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="8f581-134">unknown</span><span class="sxs-lookup"><span data-stu-id="8f581-134">unknown</span></span>|<span data-ttu-id="8f581-135">16 </span><span class="sxs-lookup"><span data-stu-id="8f581-135">16</span></span>|<span data-ttu-id="8f581-136">НеИзвестный тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="8f581-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="8f581-137">жамф</span><span class="sxs-lookup"><span data-stu-id="8f581-137">jamf</span></span>|<span data-ttu-id="8f581-138">32</span><span class="sxs-lookup"><span data-stu-id="8f581-138">32</span></span>|<span data-ttu-id="8f581-139">Атрибуты устройства извлекаются из Жамф.</span><span class="sxs-lookup"><span data-stu-id="8f581-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="8f581-140">Гуглеклауддевицеполициконтроллер</span><span class="sxs-lookup"><span data-stu-id="8f581-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="8f581-141">64</span><span class="sxs-lookup"><span data-stu-id="8f581-141">64</span></span>|<span data-ttu-id="8f581-142">Управление устройством осуществляется с помощью Клауддпк Google.</span><span class="sxs-lookup"><span data-stu-id="8f581-142">The device is managed by Google's CloudDPC.</span></span>|



