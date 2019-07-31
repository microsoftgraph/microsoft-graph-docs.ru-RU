---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2eb02ddde8b570a6d68f077ead1123b00e82cfe0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000125"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="a6caf-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="a6caf-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="a6caf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6caf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6caf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6caf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6caf-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="a6caf-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="a6caf-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a6caf-107">Members</span></span>
|<span data-ttu-id="a6caf-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a6caf-108">Member</span></span>|<span data-ttu-id="a6caf-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a6caf-109">Value</span></span>|<span data-ttu-id="a6caf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6caf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6caf-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="a6caf-111">userDefined</span></span>|<span data-ttu-id="a6caf-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a6caf-112">0</span></span>|<span data-ttu-id="a6caf-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="a6caf-113">Allow the user to set.</span></span>|
|<span data-ttu-id="a6caf-114">ко</span><span class="sxs-lookup"><span data-stu-id="a6caf-114">all</span></span>|<span data-ttu-id="a6caf-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a6caf-115">1</span></span>|<span data-ttu-id="a6caf-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="a6caf-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="a6caf-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="a6caf-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="a6caf-118">Бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="a6caf-118">businessReadyOnly</span></span>|<span data-ttu-id="a6caf-119">2</span><span class="sxs-lookup"><span data-stu-id="a6caf-119">2</span></span>|<span data-ttu-id="a6caf-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="a6caf-120">Semi-annual Channel.</span></span> <span data-ttu-id="a6caf-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="a6caf-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="a6caf-122">Виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="a6caf-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="a6caf-123">4</span><span class="sxs-lookup"><span data-stu-id="a6caf-123">3</span></span>|<span data-ttu-id="a6caf-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="a6caf-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="a6caf-125">Виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="a6caf-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="a6caf-126">SP4</span><span class="sxs-lookup"><span data-stu-id="a6caf-126">4</span></span>|<span data-ttu-id="a6caf-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="a6caf-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="a6caf-128">Виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="a6caf-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="a6caf-129">17:00</span><span class="sxs-lookup"><span data-stu-id="a6caf-129">5</span></span>|<span data-ttu-id="a6caf-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="a6caf-130">Release Windows Insider build</span></span>|





