---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
ms.openlocfilehash: d6a4ccbc9725c230f6abc7bd9ee1e38a30d5d133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074825"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="d15a5-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="d15a5-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="d15a5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d15a5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d15a5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d15a5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d15a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d15a5-107">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="d15a5-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="d15a5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d15a5-108">Members</span></span>
|<span data-ttu-id="d15a5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d15a5-109">Member</span></span>|<span data-ttu-id="d15a5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d15a5-110">Value</span></span>|<span data-ttu-id="d15a5-111">Description</span><span class="sxs-lookup"><span data-stu-id="d15a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d15a5-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d15a5-112">deviceDefault</span></span>|<span data-ttu-id="d15a5-113">0</span><span class="sxs-lookup"><span data-stu-id="d15a5-113">0</span></span>|<span data-ttu-id="d15a5-114">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="d15a5-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="d15a5-115">clean</span><span class="sxs-lookup"><span data-stu-id="d15a5-115">clean</span></span>|<span data-ttu-id="d15a5-116">1</span><span class="sxs-lookup"><span data-stu-id="d15a5-116">1</span></span>|<span data-ttu-id="d15a5-117">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="d15a5-118">карантин</span><span class="sxs-lookup"><span data-stu-id="d15a5-118">quarantine</span></span>|<span data-ttu-id="d15a5-119">2</span><span class="sxs-lookup"><span data-stu-id="d15a5-119">2</span></span>|<span data-ttu-id="d15a5-120">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="d15a5-121">удалить</span><span class="sxs-lookup"><span data-stu-id="d15a5-121">remove</span></span>|<span data-ttu-id="d15a5-122">3</span><span class="sxs-lookup"><span data-stu-id="d15a5-122">3</span></span>|<span data-ttu-id="d15a5-123">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="d15a5-124">Разрешить</span><span class="sxs-lookup"><span data-stu-id="d15a5-124">allow</span></span>|<span data-ttu-id="d15a5-125">4</span><span class="sxs-lookup"><span data-stu-id="d15a5-125">4</span></span>|<span data-ttu-id="d15a5-126">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="d15a5-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="d15a5-127">userDefined</span></span>|<span data-ttu-id="d15a5-128">5</span><span class="sxs-lookup"><span data-stu-id="d15a5-128">5</span></span>|<span data-ttu-id="d15a5-129">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="d15a5-130">блок</span><span class="sxs-lookup"><span data-stu-id="d15a5-130">block</span></span>|<span data-ttu-id="d15a5-131">6</span><span class="sxs-lookup"><span data-stu-id="d15a5-131">6</span></span>|<span data-ttu-id="d15a5-132">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="d15a5-132">Block the detected threat.</span></span>|





