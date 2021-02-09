---
title: Тип enum userExperienceAnalyticsOperatingSystemRestartCategory
description: Категория перезапуска операционной системы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d298545fae20b123440b86a475b713686ae65ea4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156814"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="72a1e-103">Тип enum userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="72a1e-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="72a1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72a1e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72a1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72a1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72a1e-107">Категория перезапуска операционной системы</span><span class="sxs-lookup"><span data-stu-id="72a1e-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="72a1e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="72a1e-108">Members</span></span>
|<span data-ttu-id="72a1e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="72a1e-109">Member</span></span>|<span data-ttu-id="72a1e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="72a1e-110">Value</span></span>|<span data-ttu-id="72a1e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="72a1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72a1e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="72a1e-112">unknown</span></span>|<span data-ttu-id="72a1e-113">0</span><span class="sxs-lookup"><span data-stu-id="72a1e-113">0</span></span>|<span data-ttu-id="72a1e-114">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="72a1e-114">Unknown</span></span>|
|<span data-ttu-id="72a1e-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="72a1e-115">restartWithUpdate</span></span>|<span data-ttu-id="72a1e-116">1 </span><span class="sxs-lookup"><span data-stu-id="72a1e-116">1</span></span>|<span data-ttu-id="72a1e-117">Перезапуск с обновлением</span><span class="sxs-lookup"><span data-stu-id="72a1e-117">Restart with update</span></span>|
|<span data-ttu-id="72a1e-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="72a1e-118">restartWithoutUpdate</span></span>|<span data-ttu-id="72a1e-119">2 </span><span class="sxs-lookup"><span data-stu-id="72a1e-119">2</span></span>|<span data-ttu-id="72a1e-120">Перезапуск без обновления</span><span class="sxs-lookup"><span data-stu-id="72a1e-120">Restart without update</span></span>|
|<span data-ttu-id="72a1e-121">blueScreen</span><span class="sxs-lookup"><span data-stu-id="72a1e-121">blueScreen</span></span>|<span data-ttu-id="72a1e-122">3 </span><span class="sxs-lookup"><span data-stu-id="72a1e-122">3</span></span>|<span data-ttu-id="72a1e-123">Перезапуск синего экрана</span><span class="sxs-lookup"><span data-stu-id="72a1e-123">Blue screen restart</span></span>|
|<span data-ttu-id="72a1e-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="72a1e-124">shutdownWithUpdate</span></span>|<span data-ttu-id="72a1e-125">4 </span><span class="sxs-lookup"><span data-stu-id="72a1e-125">4</span></span>|<span data-ttu-id="72a1e-126">Завершение работы с обновлением</span><span class="sxs-lookup"><span data-stu-id="72a1e-126">Shutdown with update</span></span>|
|<span data-ttu-id="72a1e-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="72a1e-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="72a1e-128">5 </span><span class="sxs-lookup"><span data-stu-id="72a1e-128">5</span></span>|<span data-ttu-id="72a1e-129">Завершение работы без обновления</span><span class="sxs-lookup"><span data-stu-id="72a1e-129">Shutdown without update</span></span>|
|<span data-ttu-id="72a1e-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="72a1e-130">longPowerButtonPress</span></span>|<span data-ttu-id="72a1e-131">6 </span><span class="sxs-lookup"><span data-stu-id="72a1e-131">6</span></span>|<span data-ttu-id="72a1e-132">Длинное нажатие кнопки питания</span><span class="sxs-lookup"><span data-stu-id="72a1e-132">Long power button press</span></span>|
|<span data-ttu-id="72a1e-133">bootError</span><span class="sxs-lookup"><span data-stu-id="72a1e-133">bootError</span></span>|<span data-ttu-id="72a1e-134">7 </span><span class="sxs-lookup"><span data-stu-id="72a1e-134">7</span></span>|<span data-ttu-id="72a1e-135">Ошибка загрузки</span><span class="sxs-lookup"><span data-stu-id="72a1e-135">Boot error</span></span>|
|<span data-ttu-id="72a1e-136">update</span><span class="sxs-lookup"><span data-stu-id="72a1e-136">update</span></span>|<span data-ttu-id="72a1e-137">8 </span><span class="sxs-lookup"><span data-stu-id="72a1e-137">8</span></span>|<span data-ttu-id="72a1e-138">Update</span><span class="sxs-lookup"><span data-stu-id="72a1e-138">Update</span></span>|




