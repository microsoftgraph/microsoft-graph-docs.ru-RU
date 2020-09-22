---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d057cf5d052f1fc3043a0b55f4f3ca822f244a7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041458"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="5f567-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="5f567-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="5f567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f567-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f567-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f567-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="5f567-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="5f567-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5f567-107">Members</span></span>
|<span data-ttu-id="5f567-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5f567-108">Member</span></span>|<span data-ttu-id="5f567-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5f567-109">Value</span></span>|<span data-ttu-id="5f567-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f567-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f567-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="5f567-111">deviceDefault</span></span>|<span data-ttu-id="5f567-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5f567-112">0</span></span>|<span data-ttu-id="5f567-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="5f567-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="5f567-114">чистить</span><span class="sxs-lookup"><span data-stu-id="5f567-114">clean</span></span>|<span data-ttu-id="5f567-115">1 </span><span class="sxs-lookup"><span data-stu-id="5f567-115">1</span></span>|<span data-ttu-id="5f567-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="5f567-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="5f567-117">папку</span><span class="sxs-lookup"><span data-stu-id="5f567-117">quarantine</span></span>|<span data-ttu-id="5f567-118">2 </span><span class="sxs-lookup"><span data-stu-id="5f567-118">2</span></span>|<span data-ttu-id="5f567-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5f567-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="5f567-120">удалить</span><span class="sxs-lookup"><span data-stu-id="5f567-120">remove</span></span>|<span data-ttu-id="5f567-121">4</span><span class="sxs-lookup"><span data-stu-id="5f567-121">3</span></span>|<span data-ttu-id="5f567-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5f567-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="5f567-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="5f567-123">allow</span></span>|<span data-ttu-id="5f567-124">4 </span><span class="sxs-lookup"><span data-stu-id="5f567-124">4</span></span>|<span data-ttu-id="5f567-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="5f567-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="5f567-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="5f567-126">userDefined</span></span>|<span data-ttu-id="5f567-127">5 </span><span class="sxs-lookup"><span data-stu-id="5f567-127">5</span></span>|<span data-ttu-id="5f567-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="5f567-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="5f567-129">блок</span><span class="sxs-lookup"><span data-stu-id="5f567-129">block</span></span>|<span data-ttu-id="5f567-130">6 </span><span class="sxs-lookup"><span data-stu-id="5f567-130">6</span></span>|<span data-ttu-id="5f567-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5f567-131">Block the detected threat.</span></span>|









