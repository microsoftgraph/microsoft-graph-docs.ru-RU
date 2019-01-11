---
title: Тип перечисления mobileAppIntent
description: Указывает состояние мобильного приложения на устройстве.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b8119cd188823beabf5b273e5324d0098e5b9ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875413"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="5e185-103">Тип перечисления mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="5e185-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="5e185-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e185-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e185-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e185-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e185-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e185-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e185-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5e185-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="5e185-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5e185-108">Members</span></span>
|<span data-ttu-id="5e185-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5e185-109">Member</span></span>|<span data-ttu-id="5e185-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5e185-110">Value</span></span>|<span data-ttu-id="5e185-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e185-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e185-112">доступен</span><span class="sxs-lookup"><span data-stu-id="5e185-112">available</span></span>|<span data-ttu-id="5e185-113">0</span><span class="sxs-lookup"><span data-stu-id="5e185-113">0</span></span>|<span data-ttu-id="5e185-114">Available</span><span class="sxs-lookup"><span data-stu-id="5e185-114">Available</span></span>|
|<span data-ttu-id="5e185-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="5e185-115">notAvailable</span></span>|<span data-ttu-id="5e185-116">1</span><span class="sxs-lookup"><span data-stu-id="5e185-116">1</span></span>|<span data-ttu-id="5e185-117">Недоступно</span><span class="sxs-lookup"><span data-stu-id="5e185-117">Not Available</span></span>|
|<span data-ttu-id="5e185-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="5e185-118">requiredInstall</span></span>|<span data-ttu-id="5e185-119">2</span><span class="sxs-lookup"><span data-stu-id="5e185-119">2</span></span>|<span data-ttu-id="5e185-120">Требуется установка</span><span class="sxs-lookup"><span data-stu-id="5e185-120">Required Install</span></span>|
|<span data-ttu-id="5e185-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="5e185-121">requiredUninstall</span></span>|<span data-ttu-id="5e185-122">3</span><span class="sxs-lookup"><span data-stu-id="5e185-122">3</span></span>|<span data-ttu-id="5e185-123">Требуется удалить</span><span class="sxs-lookup"><span data-stu-id="5e185-123">Required Uninstall</span></span>|
|<span data-ttu-id="5e185-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="5e185-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="5e185-125">4</span><span class="sxs-lookup"><span data-stu-id="5e185-125">4</span></span>|<span data-ttu-id="5e185-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="5e185-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="5e185-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="5e185-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="5e185-128">5</span><span class="sxs-lookup"><span data-stu-id="5e185-128">5</span></span>|<span data-ttu-id="5e185-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="5e185-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="5e185-130">исключение</span><span class="sxs-lookup"><span data-stu-id="5e185-130">exclude</span></span>|<span data-ttu-id="5e185-131">6</span><span class="sxs-lookup"><span data-stu-id="5e185-131">6</span></span>|<span data-ttu-id="5e185-132">Исключение</span><span class="sxs-lookup"><span data-stu-id="5e185-132">Exclude</span></span>|





