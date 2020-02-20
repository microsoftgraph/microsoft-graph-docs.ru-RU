---
title: тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 418670dd5f334b169d43022a9908c2a39f279b60
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163901"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="87c7f-103">тип перечисления Виндовсаутопилотпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="87c7f-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

> <span data-ttu-id="87c7f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87c7f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87c7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87c7f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="87c7f-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="87c7f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="87c7f-107">Members</span></span>
|<span data-ttu-id="87c7f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="87c7f-108">Member</span></span>|<span data-ttu-id="87c7f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="87c7f-109">Value</span></span>|<span data-ttu-id="87c7f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87c7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87c7f-111">нет</span><span class="sxs-lookup"><span data-stu-id="87c7f-111">none</span></span>|<span data-ttu-id="87c7f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="87c7f-112">0</span></span>|<span data-ttu-id="87c7f-113">Нет подробного отчета о состоянии назначения</span><span class="sxs-lookup"><span data-stu-id="87c7f-113">No assignment detailed status</span></span>|
|<span data-ttu-id="87c7f-114">хардваререкуирементснотмет</span><span class="sxs-lookup"><span data-stu-id="87c7f-114">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="87c7f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="87c7f-115">1</span></span>|<span data-ttu-id="87c7f-116">Требования к оборудованию не выполнены.</span><span class="sxs-lookup"><span data-stu-id="87c7f-116">Hardware requirements are not met.</span></span> <span data-ttu-id="87c7f-117">Это может произойти, если устройство с автоматическим развертыванием автоматически пилотного профиля назначено устройству без доверенного платформенного модуля 2,0.</span><span class="sxs-lookup"><span data-stu-id="87c7f-117">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="87c7f-118">сурфацехубпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="87c7f-118">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="87c7f-119">2</span><span class="sxs-lookup"><span data-stu-id="87c7f-119">2</span></span>|<span data-ttu-id="87c7f-120">Это может произойти, если для устройства, не Сурфацехуб, назначен профиль автопилота Сурфацехуб.</span><span class="sxs-lookup"><span data-stu-id="87c7f-120">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="87c7f-121">хололенспрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="87c7f-121">holoLensProfileNotSupported</span></span>|<span data-ttu-id="87c7f-122">4</span><span class="sxs-lookup"><span data-stu-id="87c7f-122">3</span></span>|<span data-ttu-id="87c7f-123">Это может произойти, если для устройства, которое не является HoloLens, назначен профиль автопилота HoloLens.</span><span class="sxs-lookup"><span data-stu-id="87c7f-123">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="87c7f-124">виндовспкпрофиленотсуппортед</span><span class="sxs-lookup"><span data-stu-id="87c7f-124">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="87c7f-125">SP4</span><span class="sxs-lookup"><span data-stu-id="87c7f-125">4</span></span>|<span data-ttu-id="87c7f-126">Это может произойти, если для устройства, не Виндовспк, назначен профиль автопилота Виндовспк.</span><span class="sxs-lookup"><span data-stu-id="87c7f-126">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



