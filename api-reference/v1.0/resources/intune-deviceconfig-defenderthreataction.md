---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252317"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="76f91-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="76f91-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="76f91-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76f91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76f91-105">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="76f91-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="76f91-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="76f91-106">Members</span></span>
|<span data-ttu-id="76f91-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="76f91-107">Member</span></span>|<span data-ttu-id="76f91-108">Значение</span><span class="sxs-lookup"><span data-stu-id="76f91-108">Value</span></span>|<span data-ttu-id="76f91-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76f91-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76f91-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="76f91-110">deviceDefault</span></span>|<span data-ttu-id="76f91-111">нуль</span><span class="sxs-lookup"><span data-stu-id="76f91-111">0</span></span>|<span data-ttu-id="76f91-112">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="76f91-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="76f91-113">clean</span><span class="sxs-lookup"><span data-stu-id="76f91-113">clean</span></span>|<span data-ttu-id="76f91-114">1,1</span><span class="sxs-lookup"><span data-stu-id="76f91-114">1</span></span>|<span data-ttu-id="76f91-115">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="76f91-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="76f91-116">папку</span><span class="sxs-lookup"><span data-stu-id="76f91-116">quarantine</span></span>|<span data-ttu-id="76f91-117">2</span><span class="sxs-lookup"><span data-stu-id="76f91-117">2</span></span>|<span data-ttu-id="76f91-118">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="76f91-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="76f91-119">удалить</span><span class="sxs-lookup"><span data-stu-id="76f91-119">remove</span></span>|<span data-ttu-id="76f91-120">4</span><span class="sxs-lookup"><span data-stu-id="76f91-120">3</span></span>|<span data-ttu-id="76f91-121">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="76f91-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="76f91-122">разрешить</span><span class="sxs-lookup"><span data-stu-id="76f91-122">allow</span></span>|<span data-ttu-id="76f91-123">4</span><span class="sxs-lookup"><span data-stu-id="76f91-123">4</span></span>|<span data-ttu-id="76f91-124">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="76f91-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="76f91-125">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="76f91-125">userDefined</span></span>|<span data-ttu-id="76f91-126">17:00</span><span class="sxs-lookup"><span data-stu-id="76f91-126">5</span></span>|<span data-ttu-id="76f91-127">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="76f91-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="76f91-128">блок</span><span class="sxs-lookup"><span data-stu-id="76f91-128">block</span></span>|<span data-ttu-id="76f91-129">6</span><span class="sxs-lookup"><span data-stu-id="76f91-129">6</span></span>|<span data-ttu-id="76f91-130">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="76f91-130">Block the detected threat.</span></span>|



