---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 99b7b189ed0e3f8a66eeaa4c099421b3b13e0989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271977"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="223f5-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="223f5-103">actionState enum type</span></span>

<span data-ttu-id="223f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="223f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="223f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="223f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="223f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="223f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="223f5-107">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="223f5-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="223f5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="223f5-108">Members</span></span>
|<span data-ttu-id="223f5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="223f5-109">Member</span></span>|<span data-ttu-id="223f5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="223f5-110">Value</span></span>|<span data-ttu-id="223f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="223f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="223f5-112">Нет</span><span class="sxs-lookup"><span data-stu-id="223f5-112">none</span></span>|<span data-ttu-id="223f5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="223f5-113">0</span></span>|<span data-ttu-id="223f5-114">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="223f5-114">Not a valid action state</span></span>|
|<span data-ttu-id="223f5-115">закончен</span><span class="sxs-lookup"><span data-stu-id="223f5-115">pending</span></span>|<span data-ttu-id="223f5-116">1,1</span><span class="sxs-lookup"><span data-stu-id="223f5-116">1</span></span>|<span data-ttu-id="223f5-117">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="223f5-117">Action is pending</span></span>|
|<span data-ttu-id="223f5-118">закрыт</span><span class="sxs-lookup"><span data-stu-id="223f5-118">canceled</span></span>|<span data-ttu-id="223f5-119">2</span><span class="sxs-lookup"><span data-stu-id="223f5-119">2</span></span>|<span data-ttu-id="223f5-120">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="223f5-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="223f5-121">ASP</span><span class="sxs-lookup"><span data-stu-id="223f5-121">active</span></span>|<span data-ttu-id="223f5-122">4</span><span class="sxs-lookup"><span data-stu-id="223f5-122">3</span></span>|<span data-ttu-id="223f5-123">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="223f5-123">Action is active.</span></span>|
|<span data-ttu-id="223f5-124">done</span><span class="sxs-lookup"><span data-stu-id="223f5-124">done</span></span>|<span data-ttu-id="223f5-125">4 </span><span class="sxs-lookup"><span data-stu-id="223f5-125">4</span></span>|<span data-ttu-id="223f5-126">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="223f5-126">Action completed without errors.</span></span>|
|<span data-ttu-id="223f5-127">сбоев</span><span class="sxs-lookup"><span data-stu-id="223f5-127">failed</span></span>|<span data-ttu-id="223f5-128">5 </span><span class="sxs-lookup"><span data-stu-id="223f5-128">5</span></span>|<span data-ttu-id="223f5-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="223f5-129">Action failed</span></span>|
|<span data-ttu-id="223f5-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="223f5-130">notSupported</span></span>|<span data-ttu-id="223f5-131">6 </span><span class="sxs-lookup"><span data-stu-id="223f5-131">6</span></span>|<span data-ttu-id="223f5-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="223f5-132">Action is not supported.</span></span>|




