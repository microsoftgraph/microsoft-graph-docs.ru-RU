---
title: Тип перечисления deviceGuardVirtualizationBasedSecurityState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6719dc370355c82d18c0a416cba02899ad03e183
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944266"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="fc293-103">Тип перечисления deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="fc293-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="fc293-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc293-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc293-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc293-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc293-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc293-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc293-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fc293-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="fc293-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fc293-108">Members</span></span>
|<span data-ttu-id="fc293-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fc293-109">Member</span></span>|<span data-ttu-id="fc293-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fc293-110">Value</span></span>|<span data-ttu-id="fc293-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc293-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc293-112">под управлением</span><span class="sxs-lookup"><span data-stu-id="fc293-112">running</span></span>|<span data-ttu-id="fc293-113">0</span><span class="sxs-lookup"><span data-stu-id="fc293-113">0</span></span>|<span data-ttu-id="fc293-114">Под управлением</span><span class="sxs-lookup"><span data-stu-id="fc293-114">Running</span></span>|
|<span data-ttu-id="fc293-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="fc293-115">rebootRequired</span></span>|<span data-ttu-id="fc293-116">1</span><span class="sxs-lookup"><span data-stu-id="fc293-116">1</span></span>|<span data-ttu-id="fc293-117">Обязательный корневой</span><span class="sxs-lookup"><span data-stu-id="fc293-117">Root required</span></span>|
|<span data-ttu-id="fc293-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="fc293-118">require64BitArchitecture</span></span>|<span data-ttu-id="fc293-119">2</span><span class="sxs-lookup"><span data-stu-id="fc293-119">2</span></span>|<span data-ttu-id="fc293-120">требуется 64-разрядной архитектуры</span><span class="sxs-lookup"><span data-stu-id="fc293-120">64 bit architecture required</span></span>|
|<span data-ttu-id="fc293-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="fc293-121">notLicensed</span></span>|<span data-ttu-id="fc293-122">3</span><span class="sxs-lookup"><span data-stu-id="fc293-122">3</span></span>|<span data-ttu-id="fc293-123">Нет лицензии</span><span class="sxs-lookup"><span data-stu-id="fc293-123">Not licensed</span></span>|
|<span data-ttu-id="fc293-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fc293-124">notConfigured</span></span>|<span data-ttu-id="fc293-125">4</span><span class="sxs-lookup"><span data-stu-id="fc293-125">4</span></span>|<span data-ttu-id="fc293-126">Не настроен</span><span class="sxs-lookup"><span data-stu-id="fc293-126">Not configured</span></span>|
|<span data-ttu-id="fc293-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="fc293-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="fc293-128">5</span><span class="sxs-lookup"><span data-stu-id="fc293-128">5</span></span>|<span data-ttu-id="fc293-129">Система не соответствует требованиям к оборудованию</span><span class="sxs-lookup"><span data-stu-id="fc293-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="fc293-130">другие</span><span class="sxs-lookup"><span data-stu-id="fc293-130">other</span></span>|<span data-ttu-id="fc293-131">42</span><span class="sxs-lookup"><span data-stu-id="fc293-131">42</span></span>|<span data-ttu-id="fc293-132">Другие.</span><span class="sxs-lookup"><span data-stu-id="fc293-132">Other.</span></span> <span data-ttu-id="fc293-133">Журналы событий в microsoft Windows DeviceGuard имеют более подробных сведений.</span><span class="sxs-lookup"><span data-stu-id="fc293-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





