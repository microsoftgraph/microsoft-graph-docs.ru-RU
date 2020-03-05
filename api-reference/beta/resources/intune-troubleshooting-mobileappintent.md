---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a530c7b67d4bde5829f11471434341d365d3275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523347"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="c328a-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="c328a-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="c328a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c328a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c328a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c328a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c328a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c328a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c328a-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c328a-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="c328a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c328a-108">Members</span></span>
|<span data-ttu-id="c328a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c328a-109">Member</span></span>|<span data-ttu-id="c328a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c328a-110">Value</span></span>|<span data-ttu-id="c328a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c328a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c328a-112">доступен</span><span class="sxs-lookup"><span data-stu-id="c328a-112">available</span></span>|<span data-ttu-id="c328a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c328a-113">0</span></span>|<span data-ttu-id="c328a-114">Available</span><span class="sxs-lookup"><span data-stu-id="c328a-114">Available</span></span>|
|<span data-ttu-id="c328a-115">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="c328a-115">notAvailable</span></span>|<span data-ttu-id="c328a-116">1 </span><span class="sxs-lookup"><span data-stu-id="c328a-116">1</span></span>|<span data-ttu-id="c328a-117">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="c328a-117">Not Available</span></span>|
|<span data-ttu-id="c328a-118">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="c328a-118">requiredInstall</span></span>|<span data-ttu-id="c328a-119">2 </span><span class="sxs-lookup"><span data-stu-id="c328a-119">2</span></span>|<span data-ttu-id="c328a-120">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="c328a-120">Required Install</span></span>|
|<span data-ttu-id="c328a-121">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="c328a-121">requiredUninstall</span></span>|<span data-ttu-id="c328a-122">3 </span><span class="sxs-lookup"><span data-stu-id="c328a-122">3</span></span>|<span data-ttu-id="c328a-123">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="c328a-123">Required Uninstall</span></span>|
|<span data-ttu-id="c328a-124">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="c328a-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="c328a-125">4 </span><span class="sxs-lookup"><span data-stu-id="c328a-125">4</span></span>|<span data-ttu-id="c328a-126">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="c328a-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="c328a-127">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="c328a-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="c328a-128">5 </span><span class="sxs-lookup"><span data-stu-id="c328a-128">5</span></span>|<span data-ttu-id="c328a-129">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="c328a-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="c328a-130">Отличающ</span><span class="sxs-lookup"><span data-stu-id="c328a-130">exclude</span></span>|<span data-ttu-id="c328a-131">6 </span><span class="sxs-lookup"><span data-stu-id="c328a-131">6</span></span>|<span data-ttu-id="c328a-132">Исключить</span><span class="sxs-lookup"><span data-stu-id="c328a-132">Exclude</span></span>|



