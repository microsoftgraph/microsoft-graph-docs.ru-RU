---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6be5ce422664d5666fd5c76c3ce51ad8a9d798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027519"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="02b7b-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="02b7b-103">actionState enum type</span></span>

> <span data-ttu-id="02b7b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02b7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b7b-105">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="02b7b-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="02b7b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="02b7b-106">Members</span></span>
|<span data-ttu-id="02b7b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="02b7b-107">Member</span></span>|<span data-ttu-id="02b7b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="02b7b-108">Value</span></span>|<span data-ttu-id="02b7b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02b7b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b7b-110">none</span><span class="sxs-lookup"><span data-stu-id="02b7b-110">none</span></span>|<span data-ttu-id="02b7b-111">нуль</span><span class="sxs-lookup"><span data-stu-id="02b7b-111">0</span></span>|<span data-ttu-id="02b7b-112">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="02b7b-112">Not a valid action state</span></span>|
|<span data-ttu-id="02b7b-113">закончен</span><span class="sxs-lookup"><span data-stu-id="02b7b-113">pending</span></span>|<span data-ttu-id="02b7b-114">1,1</span><span class="sxs-lookup"><span data-stu-id="02b7b-114">1</span></span>|<span data-ttu-id="02b7b-115">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="02b7b-115">Action is pending</span></span>|
|<span data-ttu-id="02b7b-116">закрыт</span><span class="sxs-lookup"><span data-stu-id="02b7b-116">canceled</span></span>|<span data-ttu-id="02b7b-117">2</span><span class="sxs-lookup"><span data-stu-id="02b7b-117">2</span></span>|<span data-ttu-id="02b7b-118">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="02b7b-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="02b7b-119">ASP</span><span class="sxs-lookup"><span data-stu-id="02b7b-119">active</span></span>|<span data-ttu-id="02b7b-120">4</span><span class="sxs-lookup"><span data-stu-id="02b7b-120">3</span></span>|<span data-ttu-id="02b7b-121">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="02b7b-121">Action is active.</span></span>|
|<span data-ttu-id="02b7b-122">done</span><span class="sxs-lookup"><span data-stu-id="02b7b-122">done</span></span>|<span data-ttu-id="02b7b-123">SP4</span><span class="sxs-lookup"><span data-stu-id="02b7b-123">4</span></span>|<span data-ttu-id="02b7b-124">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="02b7b-124">Action completed without errors.</span></span>|
|<span data-ttu-id="02b7b-125">сбоев</span><span class="sxs-lookup"><span data-stu-id="02b7b-125">failed</span></span>|<span data-ttu-id="02b7b-126">17:00</span><span class="sxs-lookup"><span data-stu-id="02b7b-126">5</span></span>|<span data-ttu-id="02b7b-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="02b7b-127">Action failed</span></span>|
|<span data-ttu-id="02b7b-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="02b7b-128">notSupported</span></span>|<span data-ttu-id="02b7b-129">6 </span><span class="sxs-lookup"><span data-stu-id="02b7b-129">6</span></span>|<span data-ttu-id="02b7b-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02b7b-130">Action is not supported.</span></span>|



