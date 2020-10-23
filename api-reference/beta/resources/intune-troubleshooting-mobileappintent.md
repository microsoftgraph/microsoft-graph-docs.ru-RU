---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4be968bfb2191b71fd810ee83ce36d4e795ea17b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730313"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="18c3b-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="18c3b-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="18c3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18c3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18c3b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18c3b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18c3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18c3b-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="18c3b-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="18c3b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="18c3b-108">Members</span></span>
|<span data-ttu-id="18c3b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="18c3b-109">Member</span></span>|<span data-ttu-id="18c3b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="18c3b-110">Value</span></span>|<span data-ttu-id="18c3b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18c3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18c3b-112">доступен</span><span class="sxs-lookup"><span data-stu-id="18c3b-112">available</span></span>|<span data-ttu-id="18c3b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="18c3b-113">0</span></span>|<span data-ttu-id="18c3b-114">Available</span><span class="sxs-lookup"><span data-stu-id="18c3b-114">Available</span></span>|
|<span data-ttu-id="18c3b-115">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="18c3b-115">notAvailable</span></span>|<span data-ttu-id="18c3b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="18c3b-116">1</span></span>|<span data-ttu-id="18c3b-117">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="18c3b-117">Not Available</span></span>|
|<span data-ttu-id="18c3b-118">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="18c3b-118">requiredInstall</span></span>|<span data-ttu-id="18c3b-119">2</span><span class="sxs-lookup"><span data-stu-id="18c3b-119">2</span></span>|<span data-ttu-id="18c3b-120">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="18c3b-120">Required Install</span></span>|
|<span data-ttu-id="18c3b-121">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="18c3b-121">requiredUninstall</span></span>|<span data-ttu-id="18c3b-122">4</span><span class="sxs-lookup"><span data-stu-id="18c3b-122">3</span></span>|<span data-ttu-id="18c3b-123">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="18c3b-123">Required Uninstall</span></span>|
|<span data-ttu-id="18c3b-124">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="18c3b-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="18c3b-125">4 </span><span class="sxs-lookup"><span data-stu-id="18c3b-125">4</span></span>|<span data-ttu-id="18c3b-126">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="18c3b-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="18c3b-127">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="18c3b-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="18c3b-128">5 </span><span class="sxs-lookup"><span data-stu-id="18c3b-128">5</span></span>|<span data-ttu-id="18c3b-129">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="18c3b-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="18c3b-130">Отличающ</span><span class="sxs-lookup"><span data-stu-id="18c3b-130">exclude</span></span>|<span data-ttu-id="18c3b-131">6 </span><span class="sxs-lookup"><span data-stu-id="18c3b-131">6</span></span>|<span data-ttu-id="18c3b-132">Исключить</span><span class="sxs-lookup"><span data-stu-id="18c3b-132">Exclude</span></span>|





