---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01f2e14e11558d79e0e5b420eac6fd0e359a813
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272334"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="b04ce-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="b04ce-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="b04ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b04ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b04ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b04ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b04ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b04ce-107">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="b04ce-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="b04ce-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b04ce-108">Members</span></span>
|<span data-ttu-id="b04ce-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b04ce-109">Member</span></span>|<span data-ttu-id="b04ce-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b04ce-110">Value</span></span>|<span data-ttu-id="b04ce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b04ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b04ce-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="b04ce-112">userDefined</span></span>|<span data-ttu-id="b04ce-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b04ce-113">0</span></span>|<span data-ttu-id="b04ce-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="b04ce-114">Allow the user to set.</span></span>|
|<span data-ttu-id="b04ce-115">ко</span><span class="sxs-lookup"><span data-stu-id="b04ce-115">all</span></span>|<span data-ttu-id="b04ce-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b04ce-116">1</span></span>|<span data-ttu-id="b04ce-117">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="b04ce-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="b04ce-118">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="b04ce-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="b04ce-119">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="b04ce-119">businessReadyOnly</span></span>|<span data-ttu-id="b04ce-120">2</span><span class="sxs-lookup"><span data-stu-id="b04ce-120">2</span></span>|<span data-ttu-id="b04ce-121">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="b04ce-121">Semi-annual Channel.</span></span> <span data-ttu-id="b04ce-122">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="b04ce-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="b04ce-123">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="b04ce-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="b04ce-124">4</span><span class="sxs-lookup"><span data-stu-id="b04ce-124">3</span></span>|<span data-ttu-id="b04ce-125">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="b04ce-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="b04ce-126">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="b04ce-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="b04ce-127">4 </span><span class="sxs-lookup"><span data-stu-id="b04ce-127">4</span></span>|<span data-ttu-id="b04ce-128">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="b04ce-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="b04ce-129">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="b04ce-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="b04ce-130">5 </span><span class="sxs-lookup"><span data-stu-id="b04ce-130">5</span></span>|<span data-ttu-id="b04ce-131">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="b04ce-131">Release Windows Insider build</span></span>|




