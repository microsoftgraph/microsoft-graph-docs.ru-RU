---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b139112db8a106dfa57c7d3ddb98e2415294914b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091378"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f9c31-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="f9c31-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="f9c31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9c31-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9c31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9c31-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="f9c31-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="f9c31-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f9c31-107">Members</span></span>
|<span data-ttu-id="f9c31-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f9c31-108">Member</span></span>|<span data-ttu-id="f9c31-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f9c31-109">Value</span></span>|<span data-ttu-id="f9c31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9c31-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="f9c31-111">userDefined</span></span>|<span data-ttu-id="f9c31-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f9c31-112">0</span></span>|<span data-ttu-id="f9c31-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="f9c31-113">Allow the user to set.</span></span>|
|<span data-ttu-id="f9c31-114">ко</span><span class="sxs-lookup"><span data-stu-id="f9c31-114">all</span></span>|<span data-ttu-id="f9c31-115">1 </span><span class="sxs-lookup"><span data-stu-id="f9c31-115">1</span></span>|<span data-ttu-id="f9c31-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="f9c31-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f9c31-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="f9c31-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f9c31-118">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="f9c31-118">businessReadyOnly</span></span>|<span data-ttu-id="f9c31-119">2 </span><span class="sxs-lookup"><span data-stu-id="f9c31-119">2</span></span>|<span data-ttu-id="f9c31-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="f9c31-120">Semi-annual Channel.</span></span> <span data-ttu-id="f9c31-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="f9c31-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f9c31-122">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="f9c31-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f9c31-123">4</span><span class="sxs-lookup"><span data-stu-id="f9c31-123">3</span></span>|<span data-ttu-id="f9c31-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="f9c31-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f9c31-125">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="f9c31-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f9c31-126">4 </span><span class="sxs-lookup"><span data-stu-id="f9c31-126">4</span></span>|<span data-ttu-id="f9c31-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="f9c31-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f9c31-128">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="f9c31-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f9c31-129">5 </span><span class="sxs-lookup"><span data-stu-id="f9c31-129">5</span></span>|<span data-ttu-id="f9c31-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="f9c31-130">Release Windows Insider build</span></span>|









