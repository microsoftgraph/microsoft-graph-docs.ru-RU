---
title: тип enum actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 99b7b189ed0e3f8a66eeaa4c099421b3b13e0989
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612273"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fbf92-103">тип enum actionState</span><span class="sxs-lookup"><span data-stu-id="fbf92-103">actionState enum type</span></span>

<span data-ttu-id="fbf92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbf92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbf92-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbf92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf92-107">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="fbf92-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="fbf92-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fbf92-108">Members</span></span>
|<span data-ttu-id="fbf92-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fbf92-109">Member</span></span>|<span data-ttu-id="fbf92-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fbf92-110">Value</span></span>|<span data-ttu-id="fbf92-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fbf92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf92-112">нет</span><span class="sxs-lookup"><span data-stu-id="fbf92-112">none</span></span>|<span data-ttu-id="fbf92-113">0</span><span class="sxs-lookup"><span data-stu-id="fbf92-113">0</span></span>|<span data-ttu-id="fbf92-114">Не допустимый состояние действия</span><span class="sxs-lookup"><span data-stu-id="fbf92-114">Not a valid action state</span></span>|
|<span data-ttu-id="fbf92-115">ожидание</span><span class="sxs-lookup"><span data-stu-id="fbf92-115">pending</span></span>|<span data-ttu-id="fbf92-116">1</span><span class="sxs-lookup"><span data-stu-id="fbf92-116">1</span></span>|<span data-ttu-id="fbf92-117">Действие ожидается</span><span class="sxs-lookup"><span data-stu-id="fbf92-117">Action is pending</span></span>|
|<span data-ttu-id="fbf92-118">отменено</span><span class="sxs-lookup"><span data-stu-id="fbf92-118">canceled</span></span>|<span data-ttu-id="fbf92-119">2</span><span class="sxs-lookup"><span data-stu-id="fbf92-119">2</span></span>|<span data-ttu-id="fbf92-120">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="fbf92-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="fbf92-121">active</span><span class="sxs-lookup"><span data-stu-id="fbf92-121">active</span></span>|<span data-ttu-id="fbf92-122">3</span><span class="sxs-lookup"><span data-stu-id="fbf92-122">3</span></span>|<span data-ttu-id="fbf92-123">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="fbf92-123">Action is active.</span></span>|
|<span data-ttu-id="fbf92-124">done</span><span class="sxs-lookup"><span data-stu-id="fbf92-124">done</span></span>|<span data-ttu-id="fbf92-125">4 </span><span class="sxs-lookup"><span data-stu-id="fbf92-125">4</span></span>|<span data-ttu-id="fbf92-126">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="fbf92-126">Action completed without errors.</span></span>|
|<span data-ttu-id="fbf92-127">не удалось</span><span class="sxs-lookup"><span data-stu-id="fbf92-127">failed</span></span>|<span data-ttu-id="fbf92-128">5 </span><span class="sxs-lookup"><span data-stu-id="fbf92-128">5</span></span>|<span data-ttu-id="fbf92-129">Действие не удалось</span><span class="sxs-lookup"><span data-stu-id="fbf92-129">Action failed</span></span>|
|<span data-ttu-id="fbf92-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="fbf92-130">notSupported</span></span>|<span data-ttu-id="fbf92-131">6 </span><span class="sxs-lookup"><span data-stu-id="fbf92-131">6</span></span>|<span data-ttu-id="fbf92-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf92-132">Action is not supported.</span></span>|




