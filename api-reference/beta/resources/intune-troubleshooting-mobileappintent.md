---
title: Тип перечисления mobileAppIntent
description: Указывает состояние мобильного приложения на устройстве.
ms.openlocfilehash: 52d704f19379e2ac6232a37926185fd5d78c2e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080629"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="3f6be-103">Тип перечисления mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="3f6be-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="3f6be-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f6be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f6be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f6be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f6be-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f6be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f6be-107">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3f6be-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="3f6be-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3f6be-108">Members</span></span>
|<span data-ttu-id="3f6be-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3f6be-109">Member</span></span>|<span data-ttu-id="3f6be-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3f6be-110">Value</span></span>|<span data-ttu-id="3f6be-111">Description</span><span class="sxs-lookup"><span data-stu-id="3f6be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f6be-112">доступен</span><span class="sxs-lookup"><span data-stu-id="3f6be-112">available</span></span>|<span data-ttu-id="3f6be-113">0</span><span class="sxs-lookup"><span data-stu-id="3f6be-113">0</span></span>|<span data-ttu-id="3f6be-114">Available</span><span class="sxs-lookup"><span data-stu-id="3f6be-114">Available</span></span>|
|<span data-ttu-id="3f6be-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="3f6be-115">notAvailable</span></span>|<span data-ttu-id="3f6be-116">1</span><span class="sxs-lookup"><span data-stu-id="3f6be-116">1</span></span>|<span data-ttu-id="3f6be-117">Недоступно</span><span class="sxs-lookup"><span data-stu-id="3f6be-117">Not Available</span></span>|
|<span data-ttu-id="3f6be-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="3f6be-118">requiredInstall</span></span>|<span data-ttu-id="3f6be-119">2</span><span class="sxs-lookup"><span data-stu-id="3f6be-119">2</span></span>|<span data-ttu-id="3f6be-120">Требуется установка</span><span class="sxs-lookup"><span data-stu-id="3f6be-120">Required Install</span></span>|
|<span data-ttu-id="3f6be-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="3f6be-121">requiredUninstall</span></span>|<span data-ttu-id="3f6be-122">3</span><span class="sxs-lookup"><span data-stu-id="3f6be-122">3</span></span>|<span data-ttu-id="3f6be-123">Требуется удалить</span><span class="sxs-lookup"><span data-stu-id="3f6be-123">Required Uninstall</span></span>|
|<span data-ttu-id="3f6be-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="3f6be-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="3f6be-125">4</span><span class="sxs-lookup"><span data-stu-id="3f6be-125">4</span></span>|<span data-ttu-id="3f6be-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="3f6be-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="3f6be-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="3f6be-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="3f6be-128">5</span><span class="sxs-lookup"><span data-stu-id="3f6be-128">5</span></span>|<span data-ttu-id="3f6be-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="3f6be-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="3f6be-130">исключение</span><span class="sxs-lookup"><span data-stu-id="3f6be-130">exclude</span></span>|<span data-ttu-id="3f6be-131">6</span><span class="sxs-lookup"><span data-stu-id="3f6be-131">6</span></span>|<span data-ttu-id="3f6be-132">Исключение</span><span class="sxs-lookup"><span data-stu-id="3f6be-132">Exclude</span></span>|





