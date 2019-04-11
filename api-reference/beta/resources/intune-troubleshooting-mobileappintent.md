---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785918"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="2e2af-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="2e2af-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="2e2af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e2af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e2af-106">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2e2af-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="2e2af-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2e2af-107">Members</span></span>
|<span data-ttu-id="2e2af-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2e2af-108">Member</span></span>|<span data-ttu-id="2e2af-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2e2af-109">Value</span></span>|<span data-ttu-id="2e2af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2af-111">доступен</span><span class="sxs-lookup"><span data-stu-id="2e2af-111">available</span></span>|<span data-ttu-id="2e2af-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2e2af-112">0</span></span>|<span data-ttu-id="2e2af-113">Available</span><span class="sxs-lookup"><span data-stu-id="2e2af-113">Available</span></span>|
|<span data-ttu-id="2e2af-114">Нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="2e2af-114">notAvailable</span></span>|<span data-ttu-id="2e2af-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2e2af-115">1</span></span>|<span data-ttu-id="2e2af-116">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="2e2af-116">Not Available</span></span>|
|<span data-ttu-id="2e2af-117">Рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="2e2af-117">requiredInstall</span></span>|<span data-ttu-id="2e2af-118">2</span><span class="sxs-lookup"><span data-stu-id="2e2af-118">2</span></span>|<span data-ttu-id="2e2af-119">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="2e2af-119">Required Install</span></span>|
|<span data-ttu-id="2e2af-120">Рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="2e2af-120">requiredUninstall</span></span>|<span data-ttu-id="2e2af-121">4</span><span class="sxs-lookup"><span data-stu-id="2e2af-121">3</span></span>|<span data-ttu-id="2e2af-122">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="2e2af-122">Required Uninstall</span></span>|
|<span data-ttu-id="2e2af-123">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="2e2af-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="2e2af-124">SP4</span><span class="sxs-lookup"><span data-stu-id="2e2af-124">4</span></span>|<span data-ttu-id="2e2af-125">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="2e2af-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="2e2af-126">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="2e2af-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="2e2af-127">17:00</span><span class="sxs-lookup"><span data-stu-id="2e2af-127">5</span></span>|<span data-ttu-id="2e2af-128">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="2e2af-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="2e2af-129">Отличающ</span><span class="sxs-lookup"><span data-stu-id="2e2af-129">exclude</span></span>|<span data-ttu-id="2e2af-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="2e2af-130">6</span></span>|<span data-ttu-id="2e2af-131">Исключить</span><span class="sxs-lookup"><span data-stu-id="2e2af-131">Exclude</span></span>|



