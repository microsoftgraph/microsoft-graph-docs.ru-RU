---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4849f369aa5dd04a68599050aa097b2ac63f5ef1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154784"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="af52b-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="af52b-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="af52b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af52b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af52b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af52b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af52b-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="af52b-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="af52b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="af52b-107">Members</span></span>
|<span data-ttu-id="af52b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="af52b-108">Member</span></span>|<span data-ttu-id="af52b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="af52b-109">Value</span></span>|<span data-ttu-id="af52b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af52b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af52b-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="af52b-111">deviceDefault</span></span>|<span data-ttu-id="af52b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="af52b-112">0</span></span>|<span data-ttu-id="af52b-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="af52b-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="af52b-114">clean</span><span class="sxs-lookup"><span data-stu-id="af52b-114">clean</span></span>|<span data-ttu-id="af52b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="af52b-115">1</span></span>|<span data-ttu-id="af52b-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="af52b-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="af52b-117">папку</span><span class="sxs-lookup"><span data-stu-id="af52b-117">quarantine</span></span>|<span data-ttu-id="af52b-118">2</span><span class="sxs-lookup"><span data-stu-id="af52b-118">2</span></span>|<span data-ttu-id="af52b-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="af52b-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="af52b-120">удалить</span><span class="sxs-lookup"><span data-stu-id="af52b-120">remove</span></span>|<span data-ttu-id="af52b-121">4</span><span class="sxs-lookup"><span data-stu-id="af52b-121">3</span></span>|<span data-ttu-id="af52b-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="af52b-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="af52b-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="af52b-123">allow</span></span>|<span data-ttu-id="af52b-124">4</span><span class="sxs-lookup"><span data-stu-id="af52b-124">4</span></span>|<span data-ttu-id="af52b-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="af52b-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="af52b-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="af52b-126">userDefined</span></span>|<span data-ttu-id="af52b-127">17:00</span><span class="sxs-lookup"><span data-stu-id="af52b-127">5</span></span>|<span data-ttu-id="af52b-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="af52b-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="af52b-129">блок</span><span class="sxs-lookup"><span data-stu-id="af52b-129">block</span></span>|<span data-ttu-id="af52b-130">6</span><span class="sxs-lookup"><span data-stu-id="af52b-130">6</span></span>|<span data-ttu-id="af52b-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="af52b-131">Block the detected threat.</span></span>|




