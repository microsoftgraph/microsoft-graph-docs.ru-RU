---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558259"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="e0fdd-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="e0fdd-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="e0fdd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0fdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0fdd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0fdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0fdd-106">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0fdd-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="e0fdd-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e0fdd-107">Members</span></span>
|<span data-ttu-id="e0fdd-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e0fdd-108">Member</span></span>|<span data-ttu-id="e0fdd-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e0fdd-109">Value</span></span>|<span data-ttu-id="e0fdd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0fdd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fdd-111">доступен</span><span class="sxs-lookup"><span data-stu-id="e0fdd-111">available</span></span>|<span data-ttu-id="e0fdd-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e0fdd-112">0</span></span>|<span data-ttu-id="e0fdd-113">Available</span><span class="sxs-lookup"><span data-stu-id="e0fdd-113">Available</span></span>|
|<span data-ttu-id="e0fdd-114">Нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="e0fdd-114">notAvailable</span></span>|<span data-ttu-id="e0fdd-115">1 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-115">1</span></span>|<span data-ttu-id="e0fdd-116">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="e0fdd-116">Not Available</span></span>|
|<span data-ttu-id="e0fdd-117">Рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="e0fdd-117">requiredInstall</span></span>|<span data-ttu-id="e0fdd-118">2 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-118">2</span></span>|<span data-ttu-id="e0fdd-119">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="e0fdd-119">Required Install</span></span>|
|<span data-ttu-id="e0fdd-120">Рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="e0fdd-120">requiredUninstall</span></span>|<span data-ttu-id="e0fdd-121">3 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-121">3</span></span>|<span data-ttu-id="e0fdd-122">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="e0fdd-122">Required Uninstall</span></span>|
|<span data-ttu-id="e0fdd-123">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="e0fdd-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="e0fdd-124">4 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-124">4</span></span>|<span data-ttu-id="e0fdd-125">Рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="e0fdd-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="e0fdd-126">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="e0fdd-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="e0fdd-127">5 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-127">5</span></span>|<span data-ttu-id="e0fdd-128">Аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="e0fdd-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="e0fdd-129">Отличающ</span><span class="sxs-lookup"><span data-stu-id="e0fdd-129">exclude</span></span>|<span data-ttu-id="e0fdd-130">6 </span><span class="sxs-lookup"><span data-stu-id="e0fdd-130">6</span></span>|<span data-ttu-id="e0fdd-131">Исключить</span><span class="sxs-lookup"><span data-stu-id="e0fdd-131">Exclude</span></span>|



