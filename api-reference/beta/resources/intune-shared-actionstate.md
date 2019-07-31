---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c561f3ea046423e26daeb544d92b89a98e4bc55b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967520"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="4bdeb-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="4bdeb-103">actionState enum type</span></span>

> <span data-ttu-id="4bdeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bdeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bdeb-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="4bdeb-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="4bdeb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4bdeb-107">Members</span></span>
|<span data-ttu-id="4bdeb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4bdeb-108">Member</span></span>|<span data-ttu-id="4bdeb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4bdeb-109">Value</span></span>|<span data-ttu-id="4bdeb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdeb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bdeb-111">none</span><span class="sxs-lookup"><span data-stu-id="4bdeb-111">none</span></span>|<span data-ttu-id="4bdeb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4bdeb-112">0</span></span>|<span data-ttu-id="4bdeb-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="4bdeb-113">Not a valid action state</span></span>|
|<span data-ttu-id="4bdeb-114">закончен</span><span class="sxs-lookup"><span data-stu-id="4bdeb-114">pending</span></span>|<span data-ttu-id="4bdeb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4bdeb-115">1</span></span>|<span data-ttu-id="4bdeb-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="4bdeb-116">Action is pending</span></span>|
|<span data-ttu-id="4bdeb-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="4bdeb-117">canceled</span></span>|<span data-ttu-id="4bdeb-118">2</span><span class="sxs-lookup"><span data-stu-id="4bdeb-118">2</span></span>|<span data-ttu-id="4bdeb-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="4bdeb-120">ASP</span><span class="sxs-lookup"><span data-stu-id="4bdeb-120">active</span></span>|<span data-ttu-id="4bdeb-121">4</span><span class="sxs-lookup"><span data-stu-id="4bdeb-121">3</span></span>|<span data-ttu-id="4bdeb-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-122">Action is active.</span></span>|
|<span data-ttu-id="4bdeb-123">done</span><span class="sxs-lookup"><span data-stu-id="4bdeb-123">done</span></span>|<span data-ttu-id="4bdeb-124">SP4</span><span class="sxs-lookup"><span data-stu-id="4bdeb-124">4</span></span>|<span data-ttu-id="4bdeb-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-125">Action completed without errors.</span></span>|
|<span data-ttu-id="4bdeb-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="4bdeb-126">failed</span></span>|<span data-ttu-id="4bdeb-127">17:00</span><span class="sxs-lookup"><span data-stu-id="4bdeb-127">5</span></span>|<span data-ttu-id="4bdeb-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="4bdeb-128">Action failed</span></span>|
|<span data-ttu-id="4bdeb-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="4bdeb-129">notSupported</span></span>|<span data-ttu-id="4bdeb-130">6 </span><span class="sxs-lookup"><span data-stu-id="4bdeb-130">6</span></span>|<span data-ttu-id="4bdeb-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bdeb-131">Action is not supported.</span></span>|





