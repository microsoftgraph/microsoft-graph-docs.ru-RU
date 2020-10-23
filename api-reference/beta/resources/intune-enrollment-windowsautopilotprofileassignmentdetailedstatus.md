---
title: тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 542f9191452077194092955f35b0e5fb332ae05d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728916"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="15d9e-103">тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="15d9e-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="15d9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15d9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15d9e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15d9e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15d9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15d9e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="15d9e-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="15d9e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="15d9e-108">Members</span></span>
|<span data-ttu-id="15d9e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="15d9e-109">Member</span></span>|<span data-ttu-id="15d9e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="15d9e-110">Value</span></span>|<span data-ttu-id="15d9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15d9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15d9e-112">none</span><span class="sxs-lookup"><span data-stu-id="15d9e-112">none</span></span>|<span data-ttu-id="15d9e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="15d9e-113">0</span></span>|<span data-ttu-id="15d9e-114">Нет подробного отчета о состоянии назначения</span><span class="sxs-lookup"><span data-stu-id="15d9e-114">No assignment detailed status</span></span>|
|<span data-ttu-id="15d9e-115">хардваререкуирементснотмет</span><span class="sxs-lookup"><span data-stu-id="15d9e-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="15d9e-116">1,1</span><span class="sxs-lookup"><span data-stu-id="15d9e-116">1</span></span>|<span data-ttu-id="15d9e-117">Требования к оборудованию не выполнены.</span><span class="sxs-lookup"><span data-stu-id="15d9e-117">Hardware requirements are not met.</span></span> <span data-ttu-id="15d9e-118">Это может произойти, если устройство с автоматическим развертыванием автоматически пилотного профиля назначено устройству без доверенного платформенного модуля 2,0.</span><span class="sxs-lookup"><span data-stu-id="15d9e-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="15d9e-119">сурфацехубпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="15d9e-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="15d9e-120">2</span><span class="sxs-lookup"><span data-stu-id="15d9e-120">2</span></span>|<span data-ttu-id="15d9e-121">Это может произойти, если для устройства, не Сурфацехуб, назначен профиль автопилота Сурфацехуб.</span><span class="sxs-lookup"><span data-stu-id="15d9e-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="15d9e-122">хололенспрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="15d9e-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="15d9e-123">4</span><span class="sxs-lookup"><span data-stu-id="15d9e-123">3</span></span>|<span data-ttu-id="15d9e-124">Это может произойти, если для устройства, которое не является HoloLens, назначен профиль автопилота HoloLens.</span><span class="sxs-lookup"><span data-stu-id="15d9e-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="15d9e-125">виндовспкпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="15d9e-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="15d9e-126">4 </span><span class="sxs-lookup"><span data-stu-id="15d9e-126">4</span></span>|<span data-ttu-id="15d9e-127">Это может произойти, если для устройства, не Виндовспк, назначен профиль автопилота Виндовспк.</span><span class="sxs-lookup"><span data-stu-id="15d9e-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|





