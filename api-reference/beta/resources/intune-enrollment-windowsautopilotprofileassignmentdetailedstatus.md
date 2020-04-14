---
title: тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d681e18ba17e591e3c97833f540c322e6e37903e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358603"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="593be-103">тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="593be-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="593be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="593be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="593be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="593be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="593be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="593be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="593be-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="593be-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="593be-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="593be-108">Members</span></span>
|<span data-ttu-id="593be-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="593be-109">Member</span></span>|<span data-ttu-id="593be-110">Значение</span><span class="sxs-lookup"><span data-stu-id="593be-110">Value</span></span>|<span data-ttu-id="593be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="593be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="593be-112">нет</span><span class="sxs-lookup"><span data-stu-id="593be-112">none</span></span>|<span data-ttu-id="593be-113">нуль</span><span class="sxs-lookup"><span data-stu-id="593be-113">0</span></span>|<span data-ttu-id="593be-114">Нет подробного отчета о состоянии назначения</span><span class="sxs-lookup"><span data-stu-id="593be-114">No assignment detailed status</span></span>|
|<span data-ttu-id="593be-115">хардваререкуирементснотмет</span><span class="sxs-lookup"><span data-stu-id="593be-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="593be-116">1,1</span><span class="sxs-lookup"><span data-stu-id="593be-116">1</span></span>|<span data-ttu-id="593be-117">Требования к оборудованию не выполнены.</span><span class="sxs-lookup"><span data-stu-id="593be-117">Hardware requirements are not met.</span></span> <span data-ttu-id="593be-118">Это может произойти, если устройство с автоматическим развертыванием автоматически пилотного профиля назначено устройству без доверенного платформенного модуля 2,0.</span><span class="sxs-lookup"><span data-stu-id="593be-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="593be-119">сурфацехубпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="593be-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="593be-120">2</span><span class="sxs-lookup"><span data-stu-id="593be-120">2</span></span>|<span data-ttu-id="593be-121">Это может произойти, если для устройства, не Сурфацехуб, назначен профиль автопилота Сурфацехуб.</span><span class="sxs-lookup"><span data-stu-id="593be-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="593be-122">хололенспрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="593be-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="593be-123">4</span><span class="sxs-lookup"><span data-stu-id="593be-123">3</span></span>|<span data-ttu-id="593be-124">Это может произойти, если для устройства, которое не является HoloLens, назначен профиль автопилота HoloLens.</span><span class="sxs-lookup"><span data-stu-id="593be-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="593be-125">виндовспкпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="593be-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="593be-126">4 </span><span class="sxs-lookup"><span data-stu-id="593be-126">4</span></span>|<span data-ttu-id="593be-127">Это может произойти, если для устройства, не Виндовспк, назначен профиль автопилота Виндовспк.</span><span class="sxs-lookup"><span data-stu-id="593be-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



