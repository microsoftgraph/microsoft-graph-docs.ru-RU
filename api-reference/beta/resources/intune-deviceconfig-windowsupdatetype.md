---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35b117b1a64650a475d392ffadf81769d3b0b08b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978670"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="b0227-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="b0227-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="b0227-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0227-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0227-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0227-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0227-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="b0227-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="b0227-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b0227-107">Members</span></span>
|<span data-ttu-id="b0227-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b0227-108">Member</span></span>|<span data-ttu-id="b0227-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b0227-109">Value</span></span>|<span data-ttu-id="b0227-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0227-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0227-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="b0227-111">userDefined</span></span>|<span data-ttu-id="b0227-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b0227-112">0</span></span>|<span data-ttu-id="b0227-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="b0227-113">Allow the user to set.</span></span>|
|<span data-ttu-id="b0227-114">ко</span><span class="sxs-lookup"><span data-stu-id="b0227-114">all</span></span>|<span data-ttu-id="b0227-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b0227-115">1</span></span>|<span data-ttu-id="b0227-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="b0227-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="b0227-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="b0227-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="b0227-118">Бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="b0227-118">businessReadyOnly</span></span>|<span data-ttu-id="b0227-119">2</span><span class="sxs-lookup"><span data-stu-id="b0227-119">2</span></span>|<span data-ttu-id="b0227-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="b0227-120">Semi-annual Channel.</span></span> <span data-ttu-id="b0227-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="b0227-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="b0227-122">Виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="b0227-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="b0227-123">4</span><span class="sxs-lookup"><span data-stu-id="b0227-123">3</span></span>|<span data-ttu-id="b0227-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="b0227-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="b0227-125">Виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="b0227-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="b0227-126">SP4</span><span class="sxs-lookup"><span data-stu-id="b0227-126">4</span></span>|<span data-ttu-id="b0227-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="b0227-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="b0227-128">Виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="b0227-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="b0227-129">17:00</span><span class="sxs-lookup"><span data-stu-id="b0227-129">5</span></span>|<span data-ttu-id="b0227-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="b0227-130">Release Windows Insider build</span></span>|





