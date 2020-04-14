---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c213567b46c7aea2f91deae8bc8a27d4b0382c7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453182"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="35e0f-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="35e0f-103">actionState enum type</span></span>

<span data-ttu-id="35e0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35e0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35e0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35e0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35e0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35e0f-107">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="35e0f-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="35e0f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="35e0f-108">Members</span></span>
|<span data-ttu-id="35e0f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="35e0f-109">Member</span></span>|<span data-ttu-id="35e0f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="35e0f-110">Value</span></span>|<span data-ttu-id="35e0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35e0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35e0f-112">нет</span><span class="sxs-lookup"><span data-stu-id="35e0f-112">none</span></span>|<span data-ttu-id="35e0f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="35e0f-113">0</span></span>|<span data-ttu-id="35e0f-114">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="35e0f-114">Not a valid action state</span></span>|
|<span data-ttu-id="35e0f-115">закончен</span><span class="sxs-lookup"><span data-stu-id="35e0f-115">pending</span></span>|<span data-ttu-id="35e0f-116">1,1</span><span class="sxs-lookup"><span data-stu-id="35e0f-116">1</span></span>|<span data-ttu-id="35e0f-117">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="35e0f-117">Action is pending</span></span>|
|<span data-ttu-id="35e0f-118">закрыт</span><span class="sxs-lookup"><span data-stu-id="35e0f-118">canceled</span></span>|<span data-ttu-id="35e0f-119">2</span><span class="sxs-lookup"><span data-stu-id="35e0f-119">2</span></span>|<span data-ttu-id="35e0f-120">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="35e0f-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="35e0f-121">ASP</span><span class="sxs-lookup"><span data-stu-id="35e0f-121">active</span></span>|<span data-ttu-id="35e0f-122">4</span><span class="sxs-lookup"><span data-stu-id="35e0f-122">3</span></span>|<span data-ttu-id="35e0f-123">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="35e0f-123">Action is active.</span></span>|
|<span data-ttu-id="35e0f-124">done</span><span class="sxs-lookup"><span data-stu-id="35e0f-124">done</span></span>|<span data-ttu-id="35e0f-125">4 </span><span class="sxs-lookup"><span data-stu-id="35e0f-125">4</span></span>|<span data-ttu-id="35e0f-126">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="35e0f-126">Action completed without errors.</span></span>|
|<span data-ttu-id="35e0f-127">сбоев</span><span class="sxs-lookup"><span data-stu-id="35e0f-127">failed</span></span>|<span data-ttu-id="35e0f-128">5 </span><span class="sxs-lookup"><span data-stu-id="35e0f-128">5</span></span>|<span data-ttu-id="35e0f-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="35e0f-129">Action failed</span></span>|
|<span data-ttu-id="35e0f-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="35e0f-130">notSupported</span></span>|<span data-ttu-id="35e0f-131">6 </span><span class="sxs-lookup"><span data-stu-id="35e0f-131">6</span></span>|<span data-ttu-id="35e0f-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e0f-132">Action is not supported.</span></span>|



