---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260223"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ba531-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="ba531-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="ba531-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba531-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba531-105">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="ba531-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="ba531-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ba531-106">Members</span></span>
|<span data-ttu-id="ba531-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ba531-107">Member</span></span>|<span data-ttu-id="ba531-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ba531-108">Value</span></span>|<span data-ttu-id="ba531-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ba531-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba531-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ba531-110">userDefined</span></span>|<span data-ttu-id="ba531-111">нуль</span><span class="sxs-lookup"><span data-stu-id="ba531-111">0</span></span>|<span data-ttu-id="ba531-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="ba531-112">Allow the user to set.</span></span>|
|<span data-ttu-id="ba531-113">all</span><span class="sxs-lookup"><span data-stu-id="ba531-113">all</span></span>|<span data-ttu-id="ba531-114">1,1</span><span class="sxs-lookup"><span data-stu-id="ba531-114">1</span></span>|<span data-ttu-id="ba531-115">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="ba531-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ba531-116">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="ba531-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ba531-117">Бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="ba531-117">businessReadyOnly</span></span>|<span data-ttu-id="ba531-118">2</span><span class="sxs-lookup"><span data-stu-id="ba531-118">2</span></span>|<span data-ttu-id="ba531-119">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="ba531-119">Semi-annual Channel.</span></span> <span data-ttu-id="ba531-120">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="ba531-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ba531-121">Виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="ba531-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ba531-122">4</span><span class="sxs-lookup"><span data-stu-id="ba531-122">3</span></span>|<span data-ttu-id="ba531-123">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="ba531-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ba531-124">Виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="ba531-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ba531-125">4</span><span class="sxs-lookup"><span data-stu-id="ba531-125">4</span></span>|<span data-ttu-id="ba531-126">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="ba531-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ba531-127">Виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="ba531-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ba531-128">17:00</span><span class="sxs-lookup"><span data-stu-id="ba531-128">5</span></span>|<span data-ttu-id="ba531-129">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="ba531-129">Release Windows Insider build</span></span>|



