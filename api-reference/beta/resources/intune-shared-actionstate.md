---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566320"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="7a95c-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="7a95c-103">actionState enum type</span></span>

> <span data-ttu-id="7a95c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a95c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a95c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a95c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a95c-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="7a95c-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="7a95c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7a95c-107">Members</span></span>
|<span data-ttu-id="7a95c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7a95c-108">Member</span></span>|<span data-ttu-id="7a95c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7a95c-109">Value</span></span>|<span data-ttu-id="7a95c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a95c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a95c-111">Нет</span><span class="sxs-lookup"><span data-stu-id="7a95c-111">none</span></span>|<span data-ttu-id="7a95c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7a95c-112">0</span></span>|<span data-ttu-id="7a95c-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="7a95c-113">Not a valid action state</span></span>|
|<span data-ttu-id="7a95c-114">закончен</span><span class="sxs-lookup"><span data-stu-id="7a95c-114">pending</span></span>|<span data-ttu-id="7a95c-115">1 </span><span class="sxs-lookup"><span data-stu-id="7a95c-115">1</span></span>|<span data-ttu-id="7a95c-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="7a95c-116">Action is pending</span></span>|
|<span data-ttu-id="7a95c-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="7a95c-117">canceled</span></span>|<span data-ttu-id="7a95c-118">2 </span><span class="sxs-lookup"><span data-stu-id="7a95c-118">2</span></span>|<span data-ttu-id="7a95c-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="7a95c-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="7a95c-120">ASP</span><span class="sxs-lookup"><span data-stu-id="7a95c-120">active</span></span>|<span data-ttu-id="7a95c-121">3 </span><span class="sxs-lookup"><span data-stu-id="7a95c-121">3</span></span>|<span data-ttu-id="7a95c-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="7a95c-122">Action is active.</span></span>|
|<span data-ttu-id="7a95c-123">done</span><span class="sxs-lookup"><span data-stu-id="7a95c-123">done</span></span>|<span data-ttu-id="7a95c-124">4 </span><span class="sxs-lookup"><span data-stu-id="7a95c-124">4</span></span>|<span data-ttu-id="7a95c-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="7a95c-125">Action completed without errors.</span></span>|
|<span data-ttu-id="7a95c-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="7a95c-126">failed</span></span>|<span data-ttu-id="7a95c-127">5 </span><span class="sxs-lookup"><span data-stu-id="7a95c-127">5</span></span>|<span data-ttu-id="7a95c-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="7a95c-128">Action failed</span></span>|
|<span data-ttu-id="7a95c-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="7a95c-129">notSupported</span></span>|<span data-ttu-id="7a95c-130">6 </span><span class="sxs-lookup"><span data-stu-id="7a95c-130">6</span></span>|<span data-ttu-id="7a95c-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a95c-131">Action is not supported.</span></span>|





