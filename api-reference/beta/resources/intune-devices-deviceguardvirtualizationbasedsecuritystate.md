---
title: Тип перечисления deviceGuardVirtualizationBasedSecurityState
description: Н/Д
ms.openlocfilehash: 719916717f711fa9230bc111e12d492557329830
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082109"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="cf396-103">Тип перечисления deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="cf396-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="cf396-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf396-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf396-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf396-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf396-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf396-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf396-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cf396-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="cf396-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cf396-108">Members</span></span>
|<span data-ttu-id="cf396-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cf396-109">Member</span></span>|<span data-ttu-id="cf396-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cf396-110">Value</span></span>|<span data-ttu-id="cf396-111">Description</span><span class="sxs-lookup"><span data-stu-id="cf396-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf396-112">под управлением</span><span class="sxs-lookup"><span data-stu-id="cf396-112">running</span></span>|<span data-ttu-id="cf396-113">0</span><span class="sxs-lookup"><span data-stu-id="cf396-113">0</span></span>|<span data-ttu-id="cf396-114">Под управлением</span><span class="sxs-lookup"><span data-stu-id="cf396-114">Running</span></span>|
|<span data-ttu-id="cf396-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="cf396-115">rebootRequired</span></span>|<span data-ttu-id="cf396-116">1</span><span class="sxs-lookup"><span data-stu-id="cf396-116">1</span></span>|<span data-ttu-id="cf396-117">Обязательный корневой</span><span class="sxs-lookup"><span data-stu-id="cf396-117">Root required</span></span>|
|<span data-ttu-id="cf396-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="cf396-118">require64BitArchitecture</span></span>|<span data-ttu-id="cf396-119">2</span><span class="sxs-lookup"><span data-stu-id="cf396-119">2</span></span>|<span data-ttu-id="cf396-120">требуется 64-разрядной архитектуры</span><span class="sxs-lookup"><span data-stu-id="cf396-120">64 bit architecture required</span></span>|
|<span data-ttu-id="cf396-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="cf396-121">notLicensed</span></span>|<span data-ttu-id="cf396-122">3</span><span class="sxs-lookup"><span data-stu-id="cf396-122">3</span></span>|<span data-ttu-id="cf396-123">Нет лицензии</span><span class="sxs-lookup"><span data-stu-id="cf396-123">Not licensed</span></span>|
|<span data-ttu-id="cf396-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cf396-124">notConfigured</span></span>|<span data-ttu-id="cf396-125">4</span><span class="sxs-lookup"><span data-stu-id="cf396-125">4</span></span>|<span data-ttu-id="cf396-126">Не настроен</span><span class="sxs-lookup"><span data-stu-id="cf396-126">Not configured</span></span>|
|<span data-ttu-id="cf396-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="cf396-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="cf396-128">5</span><span class="sxs-lookup"><span data-stu-id="cf396-128">5</span></span>|<span data-ttu-id="cf396-129">Система не соответствует требованиям к оборудованию</span><span class="sxs-lookup"><span data-stu-id="cf396-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="cf396-130">другие</span><span class="sxs-lookup"><span data-stu-id="cf396-130">other</span></span>|<span data-ttu-id="cf396-131">42</span><span class="sxs-lookup"><span data-stu-id="cf396-131">42</span></span>|<span data-ttu-id="cf396-132">Другие.</span><span class="sxs-lookup"><span data-stu-id="cf396-132">Other.</span></span> <span data-ttu-id="cf396-133">Журналы событий в microsoft Windows DeviceGuard имеют более подробных сведений.</span><span class="sxs-lookup"><span data-stu-id="cf396-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





