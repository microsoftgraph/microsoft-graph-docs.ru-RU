---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: fb54523f2817da328854e57a6672045e46ceb266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938085"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="bb596-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="bb596-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="bb596-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb596-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb596-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb596-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb596-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb596-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb596-107">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="bb596-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="bb596-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bb596-108">Members</span></span>
|<span data-ttu-id="bb596-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bb596-109">Member</span></span>|<span data-ttu-id="bb596-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bb596-110">Value</span></span>|<span data-ttu-id="bb596-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb596-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb596-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bb596-112">deviceDefault</span></span>|<span data-ttu-id="bb596-113">0</span><span class="sxs-lookup"><span data-stu-id="bb596-113">0</span></span>|<span data-ttu-id="bb596-114">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="bb596-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="bb596-115">clean</span><span class="sxs-lookup"><span data-stu-id="bb596-115">clean</span></span>|<span data-ttu-id="bb596-116">1</span><span class="sxs-lookup"><span data-stu-id="bb596-116">1</span></span>|<span data-ttu-id="bb596-117">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="bb596-118">карантин</span><span class="sxs-lookup"><span data-stu-id="bb596-118">quarantine</span></span>|<span data-ttu-id="bb596-119">2</span><span class="sxs-lookup"><span data-stu-id="bb596-119">2</span></span>|<span data-ttu-id="bb596-120">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="bb596-121">удалить</span><span class="sxs-lookup"><span data-stu-id="bb596-121">remove</span></span>|<span data-ttu-id="bb596-122">3</span><span class="sxs-lookup"><span data-stu-id="bb596-122">3</span></span>|<span data-ttu-id="bb596-123">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="bb596-124">Разрешить</span><span class="sxs-lookup"><span data-stu-id="bb596-124">allow</span></span>|<span data-ttu-id="bb596-125">4</span><span class="sxs-lookup"><span data-stu-id="bb596-125">4</span></span>|<span data-ttu-id="bb596-126">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="bb596-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="bb596-127">userDefined</span></span>|<span data-ttu-id="bb596-128">5</span><span class="sxs-lookup"><span data-stu-id="bb596-128">5</span></span>|<span data-ttu-id="bb596-129">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="bb596-130">блок</span><span class="sxs-lookup"><span data-stu-id="bb596-130">block</span></span>|<span data-ttu-id="bb596-131">6</span><span class="sxs-lookup"><span data-stu-id="bb596-131">6</span></span>|<span data-ttu-id="bb596-132">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="bb596-132">Block the detected threat.</span></span>|





