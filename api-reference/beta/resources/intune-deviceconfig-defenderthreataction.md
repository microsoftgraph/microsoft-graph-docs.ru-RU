---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400272"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="570b6-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="570b6-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="570b6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="570b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="570b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="570b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="570b6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="570b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="570b6-107">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="570b6-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="570b6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="570b6-108">Members</span></span>
|<span data-ttu-id="570b6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="570b6-109">Member</span></span>|<span data-ttu-id="570b6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="570b6-110">Value</span></span>|<span data-ttu-id="570b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="570b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="570b6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="570b6-112">deviceDefault</span></span>|<span data-ttu-id="570b6-113">0</span><span class="sxs-lookup"><span data-stu-id="570b6-113">0</span></span>|<span data-ttu-id="570b6-114">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="570b6-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="570b6-115">clean</span><span class="sxs-lookup"><span data-stu-id="570b6-115">clean</span></span>|<span data-ttu-id="570b6-116">1</span><span class="sxs-lookup"><span data-stu-id="570b6-116">1</span></span>|<span data-ttu-id="570b6-117">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="570b6-118">карантин</span><span class="sxs-lookup"><span data-stu-id="570b6-118">quarantine</span></span>|<span data-ttu-id="570b6-119">2</span><span class="sxs-lookup"><span data-stu-id="570b6-119">2</span></span>|<span data-ttu-id="570b6-120">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="570b6-121">удалить</span><span class="sxs-lookup"><span data-stu-id="570b6-121">remove</span></span>|<span data-ttu-id="570b6-122">3</span><span class="sxs-lookup"><span data-stu-id="570b6-122">3</span></span>|<span data-ttu-id="570b6-123">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="570b6-124">Разрешить</span><span class="sxs-lookup"><span data-stu-id="570b6-124">allow</span></span>|<span data-ttu-id="570b6-125">4</span><span class="sxs-lookup"><span data-stu-id="570b6-125">4</span></span>|<span data-ttu-id="570b6-126">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="570b6-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="570b6-127">userDefined</span></span>|<span data-ttu-id="570b6-128">5</span><span class="sxs-lookup"><span data-stu-id="570b6-128">5</span></span>|<span data-ttu-id="570b6-129">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="570b6-130">блок</span><span class="sxs-lookup"><span data-stu-id="570b6-130">block</span></span>|<span data-ttu-id="570b6-131">6</span><span class="sxs-lookup"><span data-stu-id="570b6-131">6</span></span>|<span data-ttu-id="570b6-132">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="570b6-132">Block the detected threat.</span></span>|




