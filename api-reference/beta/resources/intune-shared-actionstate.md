---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421615"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e0766-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="e0766-103">actionState enum type</span></span>

> <span data-ttu-id="e0766-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0766-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0766-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0766-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0766-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0766-107">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="e0766-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="e0766-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e0766-108">Members</span></span>
|<span data-ttu-id="e0766-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e0766-109">Member</span></span>|<span data-ttu-id="e0766-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e0766-110">Value</span></span>|<span data-ttu-id="e0766-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0766-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0766-112">none</span><span class="sxs-lookup"><span data-stu-id="e0766-112">none</span></span>|<span data-ttu-id="e0766-113">0</span><span class="sxs-lookup"><span data-stu-id="e0766-113">0</span></span>|<span data-ttu-id="e0766-114">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="e0766-114">Not a valid action state</span></span>|
|<span data-ttu-id="e0766-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="e0766-115">pending</span></span>|<span data-ttu-id="e0766-116">1</span><span class="sxs-lookup"><span data-stu-id="e0766-116">1</span></span>|<span data-ttu-id="e0766-117">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="e0766-117">Action is pending</span></span>|
|<span data-ttu-id="e0766-118">отменено</span><span class="sxs-lookup"><span data-stu-id="e0766-118">canceled</span></span>|<span data-ttu-id="e0766-119">2</span><span class="sxs-lookup"><span data-stu-id="e0766-119">2</span></span>|<span data-ttu-id="e0766-120">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="e0766-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="e0766-121">активных</span><span class="sxs-lookup"><span data-stu-id="e0766-121">active</span></span>|<span data-ttu-id="e0766-122">3</span><span class="sxs-lookup"><span data-stu-id="e0766-122">3</span></span>|<span data-ttu-id="e0766-123">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="e0766-123">Action is active.</span></span>|
|<span data-ttu-id="e0766-124">done</span><span class="sxs-lookup"><span data-stu-id="e0766-124">done</span></span>|<span data-ttu-id="e0766-125">4</span><span class="sxs-lookup"><span data-stu-id="e0766-125">4</span></span>|<span data-ttu-id="e0766-126">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="e0766-126">Action completed without errors.</span></span>|
|<span data-ttu-id="e0766-127">failed</span><span class="sxs-lookup"><span data-stu-id="e0766-127">failed</span></span>|<span data-ttu-id="e0766-128">5</span><span class="sxs-lookup"><span data-stu-id="e0766-128">5</span></span>|<span data-ttu-id="e0766-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="e0766-129">Action failed</span></span>|
|<span data-ttu-id="e0766-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="e0766-130">notSupported</span></span>|<span data-ttu-id="e0766-131">6</span><span class="sxs-lookup"><span data-stu-id="e0766-131">6</span></span>|<span data-ttu-id="e0766-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0766-132">Action is not supported.</span></span>|




