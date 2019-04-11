---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779694"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="4a183-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="4a183-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="4a183-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a183-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a183-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a183-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a183-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="4a183-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="4a183-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4a183-107">Members</span></span>
|<span data-ttu-id="4a183-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4a183-108">Member</span></span>|<span data-ttu-id="4a183-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4a183-109">Value</span></span>|<span data-ttu-id="4a183-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a183-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a183-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="4a183-111">userDefined</span></span>|<span data-ttu-id="4a183-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4a183-112">0</span></span>|<span data-ttu-id="4a183-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="4a183-113">Allow the user to set.</span></span>|
|<span data-ttu-id="4a183-114">ко</span><span class="sxs-lookup"><span data-stu-id="4a183-114">all</span></span>|<span data-ttu-id="4a183-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4a183-115">1</span></span>|<span data-ttu-id="4a183-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="4a183-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="4a183-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="4a183-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="4a183-118">Бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="4a183-118">businessReadyOnly</span></span>|<span data-ttu-id="4a183-119">2</span><span class="sxs-lookup"><span data-stu-id="4a183-119">2</span></span>|<span data-ttu-id="4a183-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="4a183-120">Semi-annual Channel.</span></span> <span data-ttu-id="4a183-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="4a183-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="4a183-122">Виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="4a183-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="4a183-123">4</span><span class="sxs-lookup"><span data-stu-id="4a183-123">3</span></span>|<span data-ttu-id="4a183-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="4a183-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="4a183-125">Виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="4a183-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="4a183-126">SP4</span><span class="sxs-lookup"><span data-stu-id="4a183-126">4</span></span>|<span data-ttu-id="4a183-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="4a183-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="4a183-128">Виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="4a183-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="4a183-129">17:00</span><span class="sxs-lookup"><span data-stu-id="4a183-129">5</span></span>|<span data-ttu-id="4a183-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="4a183-130">Release Windows Insider build</span></span>|





