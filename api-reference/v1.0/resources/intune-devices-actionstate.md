---
title: тип enum actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f805b39ac3954981c368ac79e566d3dc4fc218c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760218"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="9fe8a-103">тип enum actionState</span><span class="sxs-lookup"><span data-stu-id="9fe8a-103">actionState enum type</span></span>

<span data-ttu-id="9fe8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fe8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fe8a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fe8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fe8a-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="9fe8a-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="9fe8a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9fe8a-107">Members</span></span>
|<span data-ttu-id="9fe8a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9fe8a-108">Member</span></span>|<span data-ttu-id="9fe8a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9fe8a-109">Value</span></span>|<span data-ttu-id="9fe8a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe8a-111">нет</span><span class="sxs-lookup"><span data-stu-id="9fe8a-111">none</span></span>|<span data-ttu-id="9fe8a-112">0</span><span class="sxs-lookup"><span data-stu-id="9fe8a-112">0</span></span>|<span data-ttu-id="9fe8a-113">Не допустимый состояние действия</span><span class="sxs-lookup"><span data-stu-id="9fe8a-113">Not a valid action state</span></span>|
|<span data-ttu-id="9fe8a-114">ожидание</span><span class="sxs-lookup"><span data-stu-id="9fe8a-114">pending</span></span>|<span data-ttu-id="9fe8a-115">1</span><span class="sxs-lookup"><span data-stu-id="9fe8a-115">1</span></span>|<span data-ttu-id="9fe8a-116">Действие ожидается</span><span class="sxs-lookup"><span data-stu-id="9fe8a-116">Action is pending</span></span>|
|<span data-ttu-id="9fe8a-117">отменено</span><span class="sxs-lookup"><span data-stu-id="9fe8a-117">canceled</span></span>|<span data-ttu-id="9fe8a-118">2</span><span class="sxs-lookup"><span data-stu-id="9fe8a-118">2</span></span>|<span data-ttu-id="9fe8a-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="9fe8a-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="9fe8a-120">active</span><span class="sxs-lookup"><span data-stu-id="9fe8a-120">active</span></span>|<span data-ttu-id="9fe8a-121">3</span><span class="sxs-lookup"><span data-stu-id="9fe8a-121">3</span></span>|<span data-ttu-id="9fe8a-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="9fe8a-122">Action is active.</span></span>|
|<span data-ttu-id="9fe8a-123">done</span><span class="sxs-lookup"><span data-stu-id="9fe8a-123">done</span></span>|<span data-ttu-id="9fe8a-124">4 </span><span class="sxs-lookup"><span data-stu-id="9fe8a-124">4</span></span>|<span data-ttu-id="9fe8a-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="9fe8a-125">Action completed without errors.</span></span>|
|<span data-ttu-id="9fe8a-126">не удалось</span><span class="sxs-lookup"><span data-stu-id="9fe8a-126">failed</span></span>|<span data-ttu-id="9fe8a-127">5 </span><span class="sxs-lookup"><span data-stu-id="9fe8a-127">5</span></span>|<span data-ttu-id="9fe8a-128">Действие не удалось</span><span class="sxs-lookup"><span data-stu-id="9fe8a-128">Action failed</span></span>|
|<span data-ttu-id="9fe8a-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="9fe8a-129">notSupported</span></span>|<span data-ttu-id="9fe8a-130">6 </span><span class="sxs-lookup"><span data-stu-id="9fe8a-130">6</span></span>|<span data-ttu-id="9fe8a-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fe8a-131">Action is not supported.</span></span>|




