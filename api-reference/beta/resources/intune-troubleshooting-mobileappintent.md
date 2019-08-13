---
title: тип перечисления Мобилеаппинтент
description: Указывает состояние мобильного приложения на устройстве.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 27af99e84bfae80021f26163e3618da0c0a44113
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370713"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="0fbb4-103">тип перечисления Мобилеаппинтент</span><span class="sxs-lookup"><span data-stu-id="0fbb4-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="0fbb4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fbb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbb4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fbb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbb4-106">Указывает состояние мобильного приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0fbb4-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="0fbb4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0fbb4-107">Members</span></span>
|<span data-ttu-id="0fbb4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0fbb4-108">Member</span></span>|<span data-ttu-id="0fbb4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0fbb4-109">Value</span></span>|<span data-ttu-id="0fbb4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0fbb4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fbb4-111">доступен</span><span class="sxs-lookup"><span data-stu-id="0fbb4-111">available</span></span>|<span data-ttu-id="0fbb4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0fbb4-112">0</span></span>|<span data-ttu-id="0fbb4-113">Available</span><span class="sxs-lookup"><span data-stu-id="0fbb4-113">Available</span></span>|
|<span data-ttu-id="0fbb4-114">нотаваилабле</span><span class="sxs-lookup"><span data-stu-id="0fbb4-114">notAvailable</span></span>|<span data-ttu-id="0fbb4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0fbb4-115">1</span></span>|<span data-ttu-id="0fbb4-116">Компонент недоступен</span><span class="sxs-lookup"><span data-stu-id="0fbb4-116">Not Available</span></span>|
|<span data-ttu-id="0fbb4-117">рекуирединсталл</span><span class="sxs-lookup"><span data-stu-id="0fbb4-117">requiredInstall</span></span>|<span data-ttu-id="0fbb4-118">2</span><span class="sxs-lookup"><span data-stu-id="0fbb4-118">2</span></span>|<span data-ttu-id="0fbb4-119">Обязательная установка</span><span class="sxs-lookup"><span data-stu-id="0fbb4-119">Required Install</span></span>|
|<span data-ttu-id="0fbb4-120">рекуиредунинсталл</span><span class="sxs-lookup"><span data-stu-id="0fbb4-120">requiredUninstall</span></span>|<span data-ttu-id="0fbb4-121">4</span><span class="sxs-lookup"><span data-stu-id="0fbb4-121">3</span></span>|<span data-ttu-id="0fbb4-122">Обязательное удаление</span><span class="sxs-lookup"><span data-stu-id="0fbb4-122">Required Uninstall</span></span>|
|<span data-ttu-id="0fbb4-123">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="0fbb4-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="0fbb4-124">SP4</span><span class="sxs-lookup"><span data-stu-id="0fbb4-124">4</span></span>|<span data-ttu-id="0fbb4-125">рекуиредандаваилаблеинсталл</span><span class="sxs-lookup"><span data-stu-id="0fbb4-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="0fbb4-126">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="0fbb4-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="0fbb4-127">17:00</span><span class="sxs-lookup"><span data-stu-id="0fbb4-127">5</span></span>|<span data-ttu-id="0fbb4-128">аваилаблеинсталлвисаутенроллмент</span><span class="sxs-lookup"><span data-stu-id="0fbb4-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="0fbb4-129">Отличающ</span><span class="sxs-lookup"><span data-stu-id="0fbb4-129">exclude</span></span>|<span data-ttu-id="0fbb4-130">6 </span><span class="sxs-lookup"><span data-stu-id="0fbb4-130">6</span></span>|<span data-ttu-id="0fbb4-131">Исключить</span><span class="sxs-lookup"><span data-stu-id="0fbb4-131">Exclude</span></span>|



