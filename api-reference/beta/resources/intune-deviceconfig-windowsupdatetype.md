---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169162"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="bf06d-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="bf06d-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="bf06d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf06d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf06d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf06d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf06d-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="bf06d-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="bf06d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf06d-107">Members</span></span>
|<span data-ttu-id="bf06d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf06d-108">Member</span></span>|<span data-ttu-id="bf06d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bf06d-109">Value</span></span>|<span data-ttu-id="bf06d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf06d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf06d-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="bf06d-111">userDefined</span></span>|<span data-ttu-id="bf06d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bf06d-112">0</span></span>|<span data-ttu-id="bf06d-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="bf06d-113">Allow the user to set.</span></span>|
|<span data-ttu-id="bf06d-114">all</span><span class="sxs-lookup"><span data-stu-id="bf06d-114">all</span></span>|<span data-ttu-id="bf06d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bf06d-115">1</span></span>|<span data-ttu-id="bf06d-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="bf06d-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="bf06d-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="bf06d-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="bf06d-118">Бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="bf06d-118">businessReadyOnly</span></span>|<span data-ttu-id="bf06d-119">2</span><span class="sxs-lookup"><span data-stu-id="bf06d-119">2</span></span>|<span data-ttu-id="bf06d-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="bf06d-120">Semi-annual Channel.</span></span> <span data-ttu-id="bf06d-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="bf06d-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="bf06d-122">Виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="bf06d-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="bf06d-123">4</span><span class="sxs-lookup"><span data-stu-id="bf06d-123">3</span></span>|<span data-ttu-id="bf06d-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="bf06d-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="bf06d-125">Виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="bf06d-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="bf06d-126">4</span><span class="sxs-lookup"><span data-stu-id="bf06d-126">4</span></span>|<span data-ttu-id="bf06d-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="bf06d-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="bf06d-128">Виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="bf06d-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="bf06d-129">17:00</span><span class="sxs-lookup"><span data-stu-id="bf06d-129">5</span></span>|<span data-ttu-id="bf06d-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="bf06d-130">Release Windows Insider build</span></span>|




