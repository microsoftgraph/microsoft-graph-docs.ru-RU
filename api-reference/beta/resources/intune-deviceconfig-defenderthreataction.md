---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781136"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="9cd8c-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="9cd8c-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="9cd8c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cd8c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cd8c-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="9cd8c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9cd8c-107">Members</span></span>
|<span data-ttu-id="9cd8c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9cd8c-108">Member</span></span>|<span data-ttu-id="9cd8c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9cd8c-109">Value</span></span>|<span data-ttu-id="9cd8c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9cd8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cd8c-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9cd8c-111">deviceDefault</span></span>|<span data-ttu-id="9cd8c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9cd8c-112">0</span></span>|<span data-ttu-id="9cd8c-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="9cd8c-114">чистить</span><span class="sxs-lookup"><span data-stu-id="9cd8c-114">clean</span></span>|<span data-ttu-id="9cd8c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9cd8c-115">1</span></span>|<span data-ttu-id="9cd8c-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="9cd8c-117">папку</span><span class="sxs-lookup"><span data-stu-id="9cd8c-117">quarantine</span></span>|<span data-ttu-id="9cd8c-118">2</span><span class="sxs-lookup"><span data-stu-id="9cd8c-118">2</span></span>|<span data-ttu-id="9cd8c-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="9cd8c-120">удалить</span><span class="sxs-lookup"><span data-stu-id="9cd8c-120">remove</span></span>|<span data-ttu-id="9cd8c-121">4</span><span class="sxs-lookup"><span data-stu-id="9cd8c-121">3</span></span>|<span data-ttu-id="9cd8c-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="9cd8c-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="9cd8c-123">allow</span></span>|<span data-ttu-id="9cd8c-124">SP4</span><span class="sxs-lookup"><span data-stu-id="9cd8c-124">4</span></span>|<span data-ttu-id="9cd8c-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="9cd8c-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="9cd8c-126">userDefined</span></span>|<span data-ttu-id="9cd8c-127">17:00</span><span class="sxs-lookup"><span data-stu-id="9cd8c-127">5</span></span>|<span data-ttu-id="9cd8c-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="9cd8c-129">блок</span><span class="sxs-lookup"><span data-stu-id="9cd8c-129">block</span></span>|<span data-ttu-id="9cd8c-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="9cd8c-130">6</span></span>|<span data-ttu-id="9cd8c-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="9cd8c-131">Block the detected threat.</span></span>|





