---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ea3de0799c31e18603661ef081fc03a0146f341
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317839"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="b82e1-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="b82e1-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="b82e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b82e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b82e1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b82e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b82e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b82e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b82e1-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b82e1-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="b82e1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b82e1-108">Members</span></span>
|<span data-ttu-id="b82e1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b82e1-109">Member</span></span>|<span data-ttu-id="b82e1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b82e1-110">Value</span></span>|<span data-ttu-id="b82e1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b82e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82e1-112">доступен</span><span class="sxs-lookup"><span data-stu-id="b82e1-112">available</span></span>|<span data-ttu-id="b82e1-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b82e1-113">0</span></span>|<span data-ttu-id="b82e1-114">Available</span><span class="sxs-lookup"><span data-stu-id="b82e1-114">Available</span></span>|
|<span data-ttu-id="b82e1-115">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="b82e1-115">notAvailable</span></span>|<span data-ttu-id="b82e1-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b82e1-116">1</span></span>|<span data-ttu-id="b82e1-117">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="b82e1-117">Not Available</span></span>|
|<span data-ttu-id="b82e1-118">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="b82e1-118">requiredInstall</span></span>|<span data-ttu-id="b82e1-119">2</span><span class="sxs-lookup"><span data-stu-id="b82e1-119">2</span></span>|<span data-ttu-id="b82e1-120">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="b82e1-120">Required Install</span></span>|
|<span data-ttu-id="b82e1-121">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="b82e1-121">requiredUninstall</span></span>|<span data-ttu-id="b82e1-122">4</span><span class="sxs-lookup"><span data-stu-id="b82e1-122">3</span></span>|<span data-ttu-id="b82e1-123">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="b82e1-123">Required Uninstall</span></span>|
|<span data-ttu-id="b82e1-124">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="b82e1-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="b82e1-125">4 </span><span class="sxs-lookup"><span data-stu-id="b82e1-125">4</span></span>|<span data-ttu-id="b82e1-126">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="b82e1-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="b82e1-127">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="b82e1-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="b82e1-128">5 </span><span class="sxs-lookup"><span data-stu-id="b82e1-128">5</span></span>|<span data-ttu-id="b82e1-129">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="b82e1-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="b82e1-130">Отличающ</span><span class="sxs-lookup"><span data-stu-id="b82e1-130">exclude</span></span>|<span data-ttu-id="b82e1-131">6 </span><span class="sxs-lookup"><span data-stu-id="b82e1-131">6</span></span>|<span data-ttu-id="b82e1-132">Исключить</span><span class="sxs-lookup"><span data-stu-id="b82e1-132">Exclude</span></span>|



