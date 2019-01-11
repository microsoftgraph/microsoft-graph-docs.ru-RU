---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
ms.openlocfilehash: ed84a16dbac493a3e962e37ba246d8d418782a91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852824"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="49ad4-103">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="49ad4-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="49ad4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49ad4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49ad4-105">Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="49ad4-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="49ad4-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="49ad4-106">Members</span></span>
|<span data-ttu-id="49ad4-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="49ad4-107">Member</span></span>|<span data-ttu-id="49ad4-108">Значение</span><span class="sxs-lookup"><span data-stu-id="49ad4-108">Value</span></span>|<span data-ttu-id="49ad4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="49ad4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ad4-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="49ad4-110">deviceDefault</span></span>|<span data-ttu-id="49ad4-111">0</span><span class="sxs-lookup"><span data-stu-id="49ad4-111">0</span></span>|<span data-ttu-id="49ad4-112">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="49ad4-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="49ad4-113">clean</span><span class="sxs-lookup"><span data-stu-id="49ad4-113">clean</span></span>|<span data-ttu-id="49ad4-114">1</span><span class="sxs-lookup"><span data-stu-id="49ad4-114">1</span></span>|<span data-ttu-id="49ad4-115">Очистите обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="49ad4-116">карантин</span><span class="sxs-lookup"><span data-stu-id="49ad4-116">quarantine</span></span>|<span data-ttu-id="49ad4-117">2</span><span class="sxs-lookup"><span data-stu-id="49ad4-117">2</span></span>|<span data-ttu-id="49ad4-118">Карантин обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="49ad4-119">удалить</span><span class="sxs-lookup"><span data-stu-id="49ad4-119">remove</span></span>|<span data-ttu-id="49ad4-120">3</span><span class="sxs-lookup"><span data-stu-id="49ad4-120">3</span></span>|<span data-ttu-id="49ad4-121">Удаление обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="49ad4-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="49ad4-122">allow</span></span>|<span data-ttu-id="49ad4-123">4</span><span class="sxs-lookup"><span data-stu-id="49ad4-123">4</span></span>|<span data-ttu-id="49ad4-124">Разрешить обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="49ad4-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="49ad4-125">userDefined</span></span>|<span data-ttu-id="49ad4-126">5</span><span class="sxs-lookup"><span data-stu-id="49ad4-126">5</span></span>|<span data-ttu-id="49ad4-127">Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="49ad4-128">блок</span><span class="sxs-lookup"><span data-stu-id="49ad4-128">block</span></span>|<span data-ttu-id="49ad4-129">6</span><span class="sxs-lookup"><span data-stu-id="49ad4-129">6</span></span>|<span data-ttu-id="49ad4-130">Блокировка обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="49ad4-130">Block the detected threat.</span></span>|



