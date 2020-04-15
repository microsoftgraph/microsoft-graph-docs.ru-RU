---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 673f95c2f1bd6e3e1d0523af91290922b793c91d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451341"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="8c55d-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="8c55d-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="8c55d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c55d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c55d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c55d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c55d-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="8c55d-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="8c55d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8c55d-107">Members</span></span>
|<span data-ttu-id="8c55d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8c55d-108">Member</span></span>|<span data-ttu-id="8c55d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8c55d-109">Value</span></span>|<span data-ttu-id="8c55d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c55d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c55d-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="8c55d-111">userDefined</span></span>|<span data-ttu-id="8c55d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8c55d-112">0</span></span>|<span data-ttu-id="8c55d-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="8c55d-113">Allow the user to set.</span></span>|
|<span data-ttu-id="8c55d-114">ко</span><span class="sxs-lookup"><span data-stu-id="8c55d-114">all</span></span>|<span data-ttu-id="8c55d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8c55d-115">1</span></span>|<span data-ttu-id="8c55d-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="8c55d-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="8c55d-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="8c55d-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="8c55d-118">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="8c55d-118">businessReadyOnly</span></span>|<span data-ttu-id="8c55d-119">2</span><span class="sxs-lookup"><span data-stu-id="8c55d-119">2</span></span>|<span data-ttu-id="8c55d-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="8c55d-120">Semi-annual Channel.</span></span> <span data-ttu-id="8c55d-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="8c55d-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="8c55d-122">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="8c55d-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="8c55d-123">4</span><span class="sxs-lookup"><span data-stu-id="8c55d-123">3</span></span>|<span data-ttu-id="8c55d-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="8c55d-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="8c55d-125">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="8c55d-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="8c55d-126">4 </span><span class="sxs-lookup"><span data-stu-id="8c55d-126">4</span></span>|<span data-ttu-id="8c55d-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="8c55d-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="8c55d-128">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="8c55d-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="8c55d-129">5 </span><span class="sxs-lookup"><span data-stu-id="8c55d-129">5</span></span>|<span data-ttu-id="8c55d-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="8c55d-130">Release Windows Insider build</span></span>|







