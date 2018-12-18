---
title: Тип перечисления mobileAppIntent
description: Указывает состояние мобильного приложения на устройстве.
author: tfitzmac
ms.openlocfilehash: 0a230279a947ab60314a53872670fff871eff745
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347231"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="9da0c-103">Тип перечисления mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="9da0c-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="9da0c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9da0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9da0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9da0c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9da0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9da0c-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9da0c-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="9da0c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9da0c-108">Members</span></span>
|<span data-ttu-id="9da0c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9da0c-109">Member</span></span>|<span data-ttu-id="9da0c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9da0c-110">Value</span></span>|<span data-ttu-id="9da0c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9da0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9da0c-112">доступен</span><span class="sxs-lookup"><span data-stu-id="9da0c-112">available</span></span>|<span data-ttu-id="9da0c-113">0</span><span class="sxs-lookup"><span data-stu-id="9da0c-113">0</span></span>|<span data-ttu-id="9da0c-114">Available</span><span class="sxs-lookup"><span data-stu-id="9da0c-114">Available</span></span>|
|<span data-ttu-id="9da0c-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="9da0c-115">notAvailable</span></span>|<span data-ttu-id="9da0c-116">1</span><span class="sxs-lookup"><span data-stu-id="9da0c-116">1</span></span>|<span data-ttu-id="9da0c-117">Недоступно</span><span class="sxs-lookup"><span data-stu-id="9da0c-117">Not Available</span></span>|
|<span data-ttu-id="9da0c-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="9da0c-118">requiredInstall</span></span>|<span data-ttu-id="9da0c-119">2</span><span class="sxs-lookup"><span data-stu-id="9da0c-119">2</span></span>|<span data-ttu-id="9da0c-120">Требуется установка</span><span class="sxs-lookup"><span data-stu-id="9da0c-120">Required Install</span></span>|
|<span data-ttu-id="9da0c-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="9da0c-121">requiredUninstall</span></span>|<span data-ttu-id="9da0c-122">3</span><span class="sxs-lookup"><span data-stu-id="9da0c-122">3</span></span>|<span data-ttu-id="9da0c-123">Требуется удалить</span><span class="sxs-lookup"><span data-stu-id="9da0c-123">Required Uninstall</span></span>|
|<span data-ttu-id="9da0c-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="9da0c-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="9da0c-125">4</span><span class="sxs-lookup"><span data-stu-id="9da0c-125">4</span></span>|<span data-ttu-id="9da0c-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="9da0c-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="9da0c-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="9da0c-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="9da0c-128">5</span><span class="sxs-lookup"><span data-stu-id="9da0c-128">5</span></span>|<span data-ttu-id="9da0c-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="9da0c-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="9da0c-130">исключение</span><span class="sxs-lookup"><span data-stu-id="9da0c-130">exclude</span></span>|<span data-ttu-id="9da0c-131">6</span><span class="sxs-lookup"><span data-stu-id="9da0c-131">6</span></span>|<span data-ttu-id="9da0c-132">Исключение</span><span class="sxs-lookup"><span data-stu-id="9da0c-132">Exclude</span></span>|





