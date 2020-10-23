---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f971b39d1b9ef96d9163c0ac38d8505297c6754f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706928"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="b01ed-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="b01ed-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="b01ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b01ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b01ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b01ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b01ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b01ed-107">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="b01ed-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="b01ed-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b01ed-108">Members</span></span>
|<span data-ttu-id="b01ed-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b01ed-109">Member</span></span>|<span data-ttu-id="b01ed-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b01ed-110">Value</span></span>|<span data-ttu-id="b01ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b01ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b01ed-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="b01ed-112">userDefined</span></span>|<span data-ttu-id="b01ed-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b01ed-113">0</span></span>|<span data-ttu-id="b01ed-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="b01ed-114">Allow the user to set.</span></span>|
|<span data-ttu-id="b01ed-115">ко</span><span class="sxs-lookup"><span data-stu-id="b01ed-115">all</span></span>|<span data-ttu-id="b01ed-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b01ed-116">1</span></span>|<span data-ttu-id="b01ed-117">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="b01ed-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="b01ed-118">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="b01ed-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="b01ed-119">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="b01ed-119">businessReadyOnly</span></span>|<span data-ttu-id="b01ed-120">2</span><span class="sxs-lookup"><span data-stu-id="b01ed-120">2</span></span>|<span data-ttu-id="b01ed-121">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="b01ed-121">Semi-annual Channel.</span></span> <span data-ttu-id="b01ed-122">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="b01ed-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="b01ed-123">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="b01ed-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="b01ed-124">4</span><span class="sxs-lookup"><span data-stu-id="b01ed-124">3</span></span>|<span data-ttu-id="b01ed-125">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="b01ed-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="b01ed-126">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="b01ed-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="b01ed-127">4 </span><span class="sxs-lookup"><span data-stu-id="b01ed-127">4</span></span>|<span data-ttu-id="b01ed-128">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="b01ed-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="b01ed-129">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="b01ed-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="b01ed-130">5 </span><span class="sxs-lookup"><span data-stu-id="b01ed-130">5</span></span>|<span data-ttu-id="b01ed-131">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="b01ed-131">Release Windows Insider build</span></span>|





