---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
ms.openlocfilehash: a5eb108a3ab26596eec9abe838e3bbfe853d96d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027289"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="a03e6-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="a03e6-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="a03e6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a03e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a03e6-105">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="a03e6-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="a03e6-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a03e6-106">Members</span></span>
|<span data-ttu-id="a03e6-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a03e6-107">Member</span></span>|<span data-ttu-id="a03e6-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a03e6-108">Value</span></span>|<span data-ttu-id="a03e6-109">Description</span><span class="sxs-lookup"><span data-stu-id="a03e6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a03e6-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a03e6-110">deviceDefault</span></span>|<span data-ttu-id="a03e6-111">0</span><span class="sxs-lookup"><span data-stu-id="a03e6-111">0</span></span>|<span data-ttu-id="a03e6-112">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="a03e6-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="a03e6-113">clean</span><span class="sxs-lookup"><span data-stu-id="a03e6-113">clean</span></span>|<span data-ttu-id="a03e6-114">1</span><span class="sxs-lookup"><span data-stu-id="a03e6-114">1</span></span>|<span data-ttu-id="a03e6-115">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="a03e6-116">карантин</span><span class="sxs-lookup"><span data-stu-id="a03e6-116">quarantine</span></span>|<span data-ttu-id="a03e6-117">2</span><span class="sxs-lookup"><span data-stu-id="a03e6-117">2</span></span>|<span data-ttu-id="a03e6-118">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="a03e6-119">удалить</span><span class="sxs-lookup"><span data-stu-id="a03e6-119">remove</span></span>|<span data-ttu-id="a03e6-120">3</span><span class="sxs-lookup"><span data-stu-id="a03e6-120">3</span></span>|<span data-ttu-id="a03e6-121">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="a03e6-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="a03e6-122">allow</span></span>|<span data-ttu-id="a03e6-123">4</span><span class="sxs-lookup"><span data-stu-id="a03e6-123">4</span></span>|<span data-ttu-id="a03e6-124">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="a03e6-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="a03e6-125">userDefined</span></span>|<span data-ttu-id="a03e6-126">5</span><span class="sxs-lookup"><span data-stu-id="a03e6-126">5</span></span>|<span data-ttu-id="a03e6-127">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="a03e6-128">блок</span><span class="sxs-lookup"><span data-stu-id="a03e6-128">block</span></span>|<span data-ttu-id="a03e6-129">6</span><span class="sxs-lookup"><span data-stu-id="a03e6-129">6</span></span>|<span data-ttu-id="a03e6-130">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="a03e6-130">Block the detected threat.</span></span>|



