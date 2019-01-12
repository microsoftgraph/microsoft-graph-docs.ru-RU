---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990854"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="1d45d-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="1d45d-103">actionState enum type</span></span>

> <span data-ttu-id="1d45d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d45d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d45d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d45d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d45d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d45d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d45d-107">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="1d45d-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="1d45d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d45d-108">Members</span></span>
|<span data-ttu-id="1d45d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d45d-109">Member</span></span>|<span data-ttu-id="1d45d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1d45d-110">Value</span></span>|<span data-ttu-id="1d45d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d45d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d45d-112">Нет</span><span class="sxs-lookup"><span data-stu-id="1d45d-112">none</span></span>|<span data-ttu-id="1d45d-113">0</span><span class="sxs-lookup"><span data-stu-id="1d45d-113">0</span></span>|<span data-ttu-id="1d45d-114">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="1d45d-114">Not a valid action state</span></span>|
|<span data-ttu-id="1d45d-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="1d45d-115">pending</span></span>|<span data-ttu-id="1d45d-116">1</span><span class="sxs-lookup"><span data-stu-id="1d45d-116">1</span></span>|<span data-ttu-id="1d45d-117">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="1d45d-117">Action is pending</span></span>|
|<span data-ttu-id="1d45d-118">отменено</span><span class="sxs-lookup"><span data-stu-id="1d45d-118">canceled</span></span>|<span data-ttu-id="1d45d-119">2</span><span class="sxs-lookup"><span data-stu-id="1d45d-119">2</span></span>|<span data-ttu-id="1d45d-120">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="1d45d-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="1d45d-121">активных</span><span class="sxs-lookup"><span data-stu-id="1d45d-121">active</span></span>|<span data-ttu-id="1d45d-122">3</span><span class="sxs-lookup"><span data-stu-id="1d45d-122">3</span></span>|<span data-ttu-id="1d45d-123">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="1d45d-123">Action is active.</span></span>|
|<span data-ttu-id="1d45d-124">done</span><span class="sxs-lookup"><span data-stu-id="1d45d-124">done</span></span>|<span data-ttu-id="1d45d-125">4</span><span class="sxs-lookup"><span data-stu-id="1d45d-125">4</span></span>|<span data-ttu-id="1d45d-126">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="1d45d-126">Action completed without errors.</span></span>|
|<span data-ttu-id="1d45d-127">failed</span><span class="sxs-lookup"><span data-stu-id="1d45d-127">failed</span></span>|<span data-ttu-id="1d45d-128">5</span><span class="sxs-lookup"><span data-stu-id="1d45d-128">5</span></span>|<span data-ttu-id="1d45d-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="1d45d-129">Action failed</span></span>|
|<span data-ttu-id="1d45d-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="1d45d-130">notSupported</span></span>|<span data-ttu-id="1d45d-131">6</span><span class="sxs-lookup"><span data-stu-id="1d45d-131">6</span></span>|<span data-ttu-id="1d45d-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d45d-132">Action is not supported.</span></span>|





