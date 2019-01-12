---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976648"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="b07be-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="b07be-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="b07be-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b07be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b07be-105">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="b07be-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="b07be-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b07be-106">Members</span></span>
|<span data-ttu-id="b07be-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b07be-107">Member</span></span>|<span data-ttu-id="b07be-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b07be-108">Value</span></span>|<span data-ttu-id="b07be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b07be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07be-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b07be-110">deviceDefault</span></span>|<span data-ttu-id="b07be-111">0</span><span class="sxs-lookup"><span data-stu-id="b07be-111">0</span></span>|<span data-ttu-id="b07be-112">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="b07be-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="b07be-113">clean</span><span class="sxs-lookup"><span data-stu-id="b07be-113">clean</span></span>|<span data-ttu-id="b07be-114">1</span><span class="sxs-lookup"><span data-stu-id="b07be-114">1</span></span>|<span data-ttu-id="b07be-115">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="b07be-116">карантин</span><span class="sxs-lookup"><span data-stu-id="b07be-116">quarantine</span></span>|<span data-ttu-id="b07be-117">2</span><span class="sxs-lookup"><span data-stu-id="b07be-117">2</span></span>|<span data-ttu-id="b07be-118">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="b07be-119">удалить</span><span class="sxs-lookup"><span data-stu-id="b07be-119">remove</span></span>|<span data-ttu-id="b07be-120">3</span><span class="sxs-lookup"><span data-stu-id="b07be-120">3</span></span>|<span data-ttu-id="b07be-121">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="b07be-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="b07be-122">allow</span></span>|<span data-ttu-id="b07be-123">4</span><span class="sxs-lookup"><span data-stu-id="b07be-123">4</span></span>|<span data-ttu-id="b07be-124">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="b07be-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="b07be-125">userDefined</span></span>|<span data-ttu-id="b07be-126">5</span><span class="sxs-lookup"><span data-stu-id="b07be-126">5</span></span>|<span data-ttu-id="b07be-127">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="b07be-128">блок</span><span class="sxs-lookup"><span data-stu-id="b07be-128">block</span></span>|<span data-ttu-id="b07be-129">6</span><span class="sxs-lookup"><span data-stu-id="b07be-129">6</span></span>|<span data-ttu-id="b07be-130">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="b07be-130">Block the detected threat.</span></span>|



