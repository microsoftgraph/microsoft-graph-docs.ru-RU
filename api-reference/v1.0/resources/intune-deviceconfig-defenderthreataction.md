---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0195176f322230b3164856575880b9dadc24bce0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031782"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="e5c1c-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="e5c1c-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="e5c1c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5c1c-105">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="e5c1c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e5c1c-106">Members</span></span>
|<span data-ttu-id="e5c1c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e5c1c-107">Member</span></span>|<span data-ttu-id="e5c1c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e5c1c-108">Value</span></span>|<span data-ttu-id="e5c1c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e5c1c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5c1c-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="e5c1c-110">deviceDefault</span></span>|<span data-ttu-id="e5c1c-111">нуль</span><span class="sxs-lookup"><span data-stu-id="e5c1c-111">0</span></span>|<span data-ttu-id="e5c1c-112">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="e5c1c-113">чистить</span><span class="sxs-lookup"><span data-stu-id="e5c1c-113">clean</span></span>|<span data-ttu-id="e5c1c-114">1,1</span><span class="sxs-lookup"><span data-stu-id="e5c1c-114">1</span></span>|<span data-ttu-id="e5c1c-115">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="e5c1c-116">папку</span><span class="sxs-lookup"><span data-stu-id="e5c1c-116">quarantine</span></span>|<span data-ttu-id="e5c1c-117">2</span><span class="sxs-lookup"><span data-stu-id="e5c1c-117">2</span></span>|<span data-ttu-id="e5c1c-118">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="e5c1c-119">удалить</span><span class="sxs-lookup"><span data-stu-id="e5c1c-119">remove</span></span>|<span data-ttu-id="e5c1c-120">4</span><span class="sxs-lookup"><span data-stu-id="e5c1c-120">3</span></span>|<span data-ttu-id="e5c1c-121">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="e5c1c-122">разрешить</span><span class="sxs-lookup"><span data-stu-id="e5c1c-122">allow</span></span>|<span data-ttu-id="e5c1c-123">SP4</span><span class="sxs-lookup"><span data-stu-id="e5c1c-123">4</span></span>|<span data-ttu-id="e5c1c-124">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="e5c1c-125">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="e5c1c-125">userDefined</span></span>|<span data-ttu-id="e5c1c-126">17:00</span><span class="sxs-lookup"><span data-stu-id="e5c1c-126">5</span></span>|<span data-ttu-id="e5c1c-127">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="e5c1c-128">блок</span><span class="sxs-lookup"><span data-stu-id="e5c1c-128">block</span></span>|<span data-ttu-id="e5c1c-129">6 </span><span class="sxs-lookup"><span data-stu-id="e5c1c-129">6</span></span>|<span data-ttu-id="e5c1c-130">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="e5c1c-130">Block the detected threat.</span></span>|



