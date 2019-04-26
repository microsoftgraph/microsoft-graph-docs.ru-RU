---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548462"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="3d2e5-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="3d2e5-103">actionState enum type</span></span>

> <span data-ttu-id="3d2e5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d2e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d2e5-105">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="3d2e5-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="3d2e5-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="3d2e5-106">Members</span></span>
|<span data-ttu-id="3d2e5-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="3d2e5-107">Member</span></span>|<span data-ttu-id="3d2e5-108">Значение</span><span class="sxs-lookup"><span data-stu-id="3d2e5-108">Value</span></span>|<span data-ttu-id="3d2e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d2e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d2e5-110">Нет</span><span class="sxs-lookup"><span data-stu-id="3d2e5-110">none</span></span>|<span data-ttu-id="3d2e5-111">нуль</span><span class="sxs-lookup"><span data-stu-id="3d2e5-111">0</span></span>|<span data-ttu-id="3d2e5-112">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="3d2e5-112">Not a valid action state</span></span>|
|<span data-ttu-id="3d2e5-113">закончен</span><span class="sxs-lookup"><span data-stu-id="3d2e5-113">pending</span></span>|<span data-ttu-id="3d2e5-114">1 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-114">1</span></span>|<span data-ttu-id="3d2e5-115">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="3d2e5-115">Action is pending</span></span>|
|<span data-ttu-id="3d2e5-116">закрыт</span><span class="sxs-lookup"><span data-stu-id="3d2e5-116">canceled</span></span>|<span data-ttu-id="3d2e5-117">2 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-117">2</span></span>|<span data-ttu-id="3d2e5-118">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="3d2e5-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="3d2e5-119">ASP</span><span class="sxs-lookup"><span data-stu-id="3d2e5-119">active</span></span>|<span data-ttu-id="3d2e5-120">3 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-120">3</span></span>|<span data-ttu-id="3d2e5-121">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="3d2e5-121">Action is active.</span></span>|
|<span data-ttu-id="3d2e5-122">done</span><span class="sxs-lookup"><span data-stu-id="3d2e5-122">done</span></span>|<span data-ttu-id="3d2e5-123">4 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-123">4</span></span>|<span data-ttu-id="3d2e5-124">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="3d2e5-124">Action completed without errors.</span></span>|
|<span data-ttu-id="3d2e5-125">сбоев</span><span class="sxs-lookup"><span data-stu-id="3d2e5-125">failed</span></span>|<span data-ttu-id="3d2e5-126">5 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-126">5</span></span>|<span data-ttu-id="3d2e5-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="3d2e5-127">Action failed</span></span>|
|<span data-ttu-id="3d2e5-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="3d2e5-128">notSupported</span></span>|<span data-ttu-id="3d2e5-129">6 </span><span class="sxs-lookup"><span data-stu-id="3d2e5-129">6</span></span>|<span data-ttu-id="3d2e5-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d2e5-130">Action is not supported.</span></span>|



