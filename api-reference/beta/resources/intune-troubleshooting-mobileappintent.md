---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6da589015b5120add046eabfa146069cc349951
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075765"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="0a537-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="0a537-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="0a537-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a537-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a537-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a537-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a537-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a537-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="0a537-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a537-108">Members</span></span>
|<span data-ttu-id="0a537-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a537-109">Member</span></span>|<span data-ttu-id="0a537-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0a537-110">Value</span></span>|<span data-ttu-id="0a537-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a537-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a537-112">доступен</span><span class="sxs-lookup"><span data-stu-id="0a537-112">available</span></span>|<span data-ttu-id="0a537-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0a537-113">0</span></span>|<span data-ttu-id="0a537-114">Available</span><span class="sxs-lookup"><span data-stu-id="0a537-114">Available</span></span>|
|<span data-ttu-id="0a537-115">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="0a537-115">notAvailable</span></span>|<span data-ttu-id="0a537-116">1 </span><span class="sxs-lookup"><span data-stu-id="0a537-116">1</span></span>|<span data-ttu-id="0a537-117">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="0a537-117">Not Available</span></span>|
|<span data-ttu-id="0a537-118">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="0a537-118">requiredInstall</span></span>|<span data-ttu-id="0a537-119">2 </span><span class="sxs-lookup"><span data-stu-id="0a537-119">2</span></span>|<span data-ttu-id="0a537-120">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="0a537-120">Required Install</span></span>|
|<span data-ttu-id="0a537-121">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="0a537-121">requiredUninstall</span></span>|<span data-ttu-id="0a537-122">4</span><span class="sxs-lookup"><span data-stu-id="0a537-122">3</span></span>|<span data-ttu-id="0a537-123">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="0a537-123">Required Uninstall</span></span>|
|<span data-ttu-id="0a537-124">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="0a537-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="0a537-125">4 </span><span class="sxs-lookup"><span data-stu-id="0a537-125">4</span></span>|<span data-ttu-id="0a537-126">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="0a537-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="0a537-127">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="0a537-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="0a537-128">5 </span><span class="sxs-lookup"><span data-stu-id="0a537-128">5</span></span>|<span data-ttu-id="0a537-129">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="0a537-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="0a537-130">Отличающ</span><span class="sxs-lookup"><span data-stu-id="0a537-130">exclude</span></span>|<span data-ttu-id="0a537-131">6 </span><span class="sxs-lookup"><span data-stu-id="0a537-131">6</span></span>|<span data-ttu-id="0a537-132">Исключить</span><span class="sxs-lookup"><span data-stu-id="0a537-132">Exclude</span></span>|






