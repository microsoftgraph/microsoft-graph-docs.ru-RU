---
title: тип перечисления Усерекспериенцеаналитиксоператингсистемрестарткатегори
description: Категория перезапуска операционной системы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d78328cc9f44dbffca0085890a8c69184c2eac3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080805"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="acd7a-103">тип перечисления Усерекспериенцеаналитиксоператингсистемрестарткатегори</span><span class="sxs-lookup"><span data-stu-id="acd7a-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="acd7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acd7a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acd7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acd7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acd7a-107">Категория перезапуска операционной системы</span><span class="sxs-lookup"><span data-stu-id="acd7a-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="acd7a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="acd7a-108">Members</span></span>
|<span data-ttu-id="acd7a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="acd7a-109">Member</span></span>|<span data-ttu-id="acd7a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="acd7a-110">Value</span></span>|<span data-ttu-id="acd7a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="acd7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acd7a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="acd7a-112">unknown</span></span>|<span data-ttu-id="acd7a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="acd7a-113">0</span></span>|<span data-ttu-id="acd7a-114">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="acd7a-114">Unknown</span></span>|
|<span data-ttu-id="acd7a-115">рестартвисупдате</span><span class="sxs-lookup"><span data-stu-id="acd7a-115">restartWithUpdate</span></span>|<span data-ttu-id="acd7a-116">1 </span><span class="sxs-lookup"><span data-stu-id="acd7a-116">1</span></span>|<span data-ttu-id="acd7a-117">Перезапуск с обновлением</span><span class="sxs-lookup"><span data-stu-id="acd7a-117">Restart with update</span></span>|
|<span data-ttu-id="acd7a-118">рестартвисаутупдате</span><span class="sxs-lookup"><span data-stu-id="acd7a-118">restartWithoutUpdate</span></span>|<span data-ttu-id="acd7a-119">2 </span><span class="sxs-lookup"><span data-stu-id="acd7a-119">2</span></span>|<span data-ttu-id="acd7a-120">Перезагрузка без обновления</span><span class="sxs-lookup"><span data-stu-id="acd7a-120">Restart without update</span></span>|
|<span data-ttu-id="acd7a-121">блуескрин</span><span class="sxs-lookup"><span data-stu-id="acd7a-121">blueScreen</span></span>|<span data-ttu-id="acd7a-122">4</span><span class="sxs-lookup"><span data-stu-id="acd7a-122">3</span></span>|<span data-ttu-id="acd7a-123">Перезагрузка синего экрана</span><span class="sxs-lookup"><span data-stu-id="acd7a-123">Blue screen restart</span></span>|
|<span data-ttu-id="acd7a-124">шутдовнвисупдате</span><span class="sxs-lookup"><span data-stu-id="acd7a-124">shutdownWithUpdate</span></span>|<span data-ttu-id="acd7a-125">4 </span><span class="sxs-lookup"><span data-stu-id="acd7a-125">4</span></span>|<span data-ttu-id="acd7a-126">Завершение работы с обновлением</span><span class="sxs-lookup"><span data-stu-id="acd7a-126">Shutdown with update</span></span>|
|<span data-ttu-id="acd7a-127">шутдовнвисаутупдате</span><span class="sxs-lookup"><span data-stu-id="acd7a-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="acd7a-128">5 </span><span class="sxs-lookup"><span data-stu-id="acd7a-128">5</span></span>|<span data-ttu-id="acd7a-129">Завершение работы без обновления</span><span class="sxs-lookup"><span data-stu-id="acd7a-129">Shutdown without update</span></span>|
|<span data-ttu-id="acd7a-130">лонгповербуттонпресс</span><span class="sxs-lookup"><span data-stu-id="acd7a-130">longPowerButtonPress</span></span>|<span data-ttu-id="acd7a-131">6 </span><span class="sxs-lookup"><span data-stu-id="acd7a-131">6</span></span>|<span data-ttu-id="acd7a-132">Нажатие кнопки длительного энергопотребления</span><span class="sxs-lookup"><span data-stu-id="acd7a-132">Long power button press</span></span>|
|<span data-ttu-id="acd7a-133">бутеррор</span><span class="sxs-lookup"><span data-stu-id="acd7a-133">bootError</span></span>|<span data-ttu-id="acd7a-134">7 </span><span class="sxs-lookup"><span data-stu-id="acd7a-134">7</span></span>|<span data-ttu-id="acd7a-135">Ошибка загрузки</span><span class="sxs-lookup"><span data-stu-id="acd7a-135">Boot error</span></span>|






