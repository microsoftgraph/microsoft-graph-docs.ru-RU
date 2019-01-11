---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871941"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="6358a-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="6358a-103">actionState enum type</span></span>

> <span data-ttu-id="6358a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6358a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6358a-105">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="6358a-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="6358a-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6358a-106">Members</span></span>
|<span data-ttu-id="6358a-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6358a-107">Member</span></span>|<span data-ttu-id="6358a-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6358a-108">Value</span></span>|<span data-ttu-id="6358a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6358a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6358a-110">Нет</span><span class="sxs-lookup"><span data-stu-id="6358a-110">none</span></span>|<span data-ttu-id="6358a-111">0</span><span class="sxs-lookup"><span data-stu-id="6358a-111">0</span></span>|<span data-ttu-id="6358a-112">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="6358a-112">Not a valid action state</span></span>|
|<span data-ttu-id="6358a-113">Ожидание</span><span class="sxs-lookup"><span data-stu-id="6358a-113">pending</span></span>|<span data-ttu-id="6358a-114">1</span><span class="sxs-lookup"><span data-stu-id="6358a-114">1</span></span>|<span data-ttu-id="6358a-115">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="6358a-115">Action is pending</span></span>|
|<span data-ttu-id="6358a-116">отменено</span><span class="sxs-lookup"><span data-stu-id="6358a-116">canceled</span></span>|<span data-ttu-id="6358a-117">2</span><span class="sxs-lookup"><span data-stu-id="6358a-117">2</span></span>|<span data-ttu-id="6358a-118">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="6358a-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="6358a-119">активных</span><span class="sxs-lookup"><span data-stu-id="6358a-119">active</span></span>|<span data-ttu-id="6358a-120">3</span><span class="sxs-lookup"><span data-stu-id="6358a-120">3</span></span>|<span data-ttu-id="6358a-121">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="6358a-121">Action is active.</span></span>|
|<span data-ttu-id="6358a-122">done</span><span class="sxs-lookup"><span data-stu-id="6358a-122">done</span></span>|<span data-ttu-id="6358a-123">4</span><span class="sxs-lookup"><span data-stu-id="6358a-123">4</span></span>|<span data-ttu-id="6358a-124">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="6358a-124">Action completed without errors.</span></span>|
|<span data-ttu-id="6358a-125">failed</span><span class="sxs-lookup"><span data-stu-id="6358a-125">failed</span></span>|<span data-ttu-id="6358a-126">5</span><span class="sxs-lookup"><span data-stu-id="6358a-126">5</span></span>|<span data-ttu-id="6358a-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="6358a-127">Action failed</span></span>|
|<span data-ttu-id="6358a-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="6358a-128">notSupported</span></span>|<span data-ttu-id="6358a-129">6</span><span class="sxs-lookup"><span data-stu-id="6358a-129">6</span></span>|<span data-ttu-id="6358a-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6358a-130">Action is not supported.</span></span>|



