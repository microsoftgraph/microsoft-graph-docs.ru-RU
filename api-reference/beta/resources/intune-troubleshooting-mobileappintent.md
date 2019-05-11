---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 135800266a2737c6c6dc3931b2a78990c059ef2c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939688"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="4ee5e-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="4ee5e-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="4ee5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ee5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ee5e-106">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4ee5e-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="4ee5e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4ee5e-107">Members</span></span>
|<span data-ttu-id="4ee5e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4ee5e-108">Member</span></span>|<span data-ttu-id="4ee5e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee5e-109">Value</span></span>|<span data-ttu-id="4ee5e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ee5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ee5e-111">доступен</span><span class="sxs-lookup"><span data-stu-id="4ee5e-111">available</span></span>|<span data-ttu-id="4ee5e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4ee5e-112">0</span></span>|<span data-ttu-id="4ee5e-113">Available</span><span class="sxs-lookup"><span data-stu-id="4ee5e-113">Available</span></span>|
|<span data-ttu-id="4ee5e-114">Нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="4ee5e-114">notAvailable</span></span>|<span data-ttu-id="4ee5e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4ee5e-115">1</span></span>|<span data-ttu-id="4ee5e-116">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="4ee5e-116">Not Available</span></span>|
|<span data-ttu-id="4ee5e-117">Рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="4ee5e-117">requiredInstall</span></span>|<span data-ttu-id="4ee5e-118">2</span><span class="sxs-lookup"><span data-stu-id="4ee5e-118">2</span></span>|<span data-ttu-id="4ee5e-119">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="4ee5e-119">Required Install</span></span>|
|<span data-ttu-id="4ee5e-120">Рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="4ee5e-120">requiredUninstall</span></span>|<span data-ttu-id="4ee5e-121">4</span><span class="sxs-lookup"><span data-stu-id="4ee5e-121">3</span></span>|<span data-ttu-id="4ee5e-122">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="4ee5e-122">Required Uninstall</span></span>|
|<span data-ttu-id="4ee5e-123">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="4ee5e-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="4ee5e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="4ee5e-124">4</span></span>|<span data-ttu-id="4ee5e-125">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="4ee5e-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="4ee5e-126">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="4ee5e-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="4ee5e-127">17:00</span><span class="sxs-lookup"><span data-stu-id="4ee5e-127">5</span></span>|<span data-ttu-id="4ee5e-128">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="4ee5e-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="4ee5e-129">Отличающ</span><span class="sxs-lookup"><span data-stu-id="4ee5e-129">exclude</span></span>|<span data-ttu-id="4ee5e-130">6 </span><span class="sxs-lookup"><span data-stu-id="4ee5e-130">6</span></span>|<span data-ttu-id="4ee5e-131">Исключить</span><span class="sxs-lookup"><span data-stu-id="4ee5e-131">Exclude</span></span>|




