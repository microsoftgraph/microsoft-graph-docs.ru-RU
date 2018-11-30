---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
ms.openlocfilehash: 1a18eb87cb4c9162777d16dc866de5f5766c87b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027926"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="beb26-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="beb26-103">actionState enum type</span></span>

> <span data-ttu-id="beb26-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="beb26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beb26-105">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="beb26-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="beb26-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="beb26-106">Members</span></span>
|<span data-ttu-id="beb26-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="beb26-107">Member</span></span>|<span data-ttu-id="beb26-108">Значение</span><span class="sxs-lookup"><span data-stu-id="beb26-108">Value</span></span>|<span data-ttu-id="beb26-109">Description</span><span class="sxs-lookup"><span data-stu-id="beb26-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb26-110">Нет</span><span class="sxs-lookup"><span data-stu-id="beb26-110">none</span></span>|<span data-ttu-id="beb26-111">0</span><span class="sxs-lookup"><span data-stu-id="beb26-111">0</span></span>|<span data-ttu-id="beb26-112">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="beb26-112">Not a valid action state</span></span>|
|<span data-ttu-id="beb26-113">Ожидание</span><span class="sxs-lookup"><span data-stu-id="beb26-113">pending</span></span>|<span data-ttu-id="beb26-114">1</span><span class="sxs-lookup"><span data-stu-id="beb26-114">1</span></span>|<span data-ttu-id="beb26-115">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="beb26-115">Action is pending</span></span>|
|<span data-ttu-id="beb26-116">отменено</span><span class="sxs-lookup"><span data-stu-id="beb26-116">canceled</span></span>|<span data-ttu-id="beb26-117">2</span><span class="sxs-lookup"><span data-stu-id="beb26-117">2</span></span>|<span data-ttu-id="beb26-118">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="beb26-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="beb26-119">активных</span><span class="sxs-lookup"><span data-stu-id="beb26-119">active</span></span>|<span data-ttu-id="beb26-120">3</span><span class="sxs-lookup"><span data-stu-id="beb26-120">3</span></span>|<span data-ttu-id="beb26-121">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="beb26-121">Action is active.</span></span>|
|<span data-ttu-id="beb26-122">done</span><span class="sxs-lookup"><span data-stu-id="beb26-122">done</span></span>|<span data-ttu-id="beb26-123">4</span><span class="sxs-lookup"><span data-stu-id="beb26-123">4</span></span>|<span data-ttu-id="beb26-124">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="beb26-124">Action completed without errors.</span></span>|
|<span data-ttu-id="beb26-125">failed</span><span class="sxs-lookup"><span data-stu-id="beb26-125">failed</span></span>|<span data-ttu-id="beb26-126">5</span><span class="sxs-lookup"><span data-stu-id="beb26-126">5</span></span>|<span data-ttu-id="beb26-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="beb26-127">Action failed</span></span>|
|<span data-ttu-id="beb26-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="beb26-128">notSupported</span></span>|<span data-ttu-id="beb26-129">6</span><span class="sxs-lookup"><span data-stu-id="beb26-129">6</span></span>|<span data-ttu-id="beb26-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb26-130">Action is not supported.</span></span>|



