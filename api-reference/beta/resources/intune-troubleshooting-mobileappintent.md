---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07c57d57217e76e67dd6e66a58f76d98eccd4eeb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271613"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="32c8a-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="32c8a-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="32c8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32c8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32c8a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32c8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32c8a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32c8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32c8a-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="32c8a-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="32c8a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="32c8a-108">Members</span></span>
|<span data-ttu-id="32c8a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="32c8a-109">Member</span></span>|<span data-ttu-id="32c8a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="32c8a-110">Value</span></span>|<span data-ttu-id="32c8a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32c8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32c8a-112">доступен</span><span class="sxs-lookup"><span data-stu-id="32c8a-112">available</span></span>|<span data-ttu-id="32c8a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="32c8a-113">0</span></span>|<span data-ttu-id="32c8a-114">Available</span><span class="sxs-lookup"><span data-stu-id="32c8a-114">Available</span></span>|
|<span data-ttu-id="32c8a-115">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="32c8a-115">notAvailable</span></span>|<span data-ttu-id="32c8a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="32c8a-116">1</span></span>|<span data-ttu-id="32c8a-117">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="32c8a-117">Not Available</span></span>|
|<span data-ttu-id="32c8a-118">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="32c8a-118">requiredInstall</span></span>|<span data-ttu-id="32c8a-119">2</span><span class="sxs-lookup"><span data-stu-id="32c8a-119">2</span></span>|<span data-ttu-id="32c8a-120">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="32c8a-120">Required Install</span></span>|
|<span data-ttu-id="32c8a-121">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="32c8a-121">requiredUninstall</span></span>|<span data-ttu-id="32c8a-122">4</span><span class="sxs-lookup"><span data-stu-id="32c8a-122">3</span></span>|<span data-ttu-id="32c8a-123">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="32c8a-123">Required Uninstall</span></span>|
|<span data-ttu-id="32c8a-124">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="32c8a-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="32c8a-125">4 </span><span class="sxs-lookup"><span data-stu-id="32c8a-125">4</span></span>|<span data-ttu-id="32c8a-126">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="32c8a-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="32c8a-127">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="32c8a-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="32c8a-128">5 </span><span class="sxs-lookup"><span data-stu-id="32c8a-128">5</span></span>|<span data-ttu-id="32c8a-129">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="32c8a-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="32c8a-130">Отличающ</span><span class="sxs-lookup"><span data-stu-id="32c8a-130">exclude</span></span>|<span data-ttu-id="32c8a-131">6 </span><span class="sxs-lookup"><span data-stu-id="32c8a-131">6</span></span>|<span data-ttu-id="32c8a-132">Исключить</span><span class="sxs-lookup"><span data-stu-id="32c8a-132">Exclude</span></span>|




