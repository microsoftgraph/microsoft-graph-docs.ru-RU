---
title: тип перечисления Ембеддедсимдевицестатевалуе
description: Описывает различные состояния для встроенного кода активации SIM-карты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 27e7b9e343d751f0417b7bd5dce3d526c93f131f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736130"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="cc40b-103">тип перечисления Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="cc40b-103">embeddedSIMDeviceStateValue enum type</span></span>

<span data-ttu-id="cc40b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc40b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc40b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc40b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc40b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc40b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc40b-107">Описывает различные состояния для встроенного кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="cc40b-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="cc40b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cc40b-108">Members</span></span>
|<span data-ttu-id="cc40b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cc40b-109">Member</span></span>|<span data-ttu-id="cc40b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cc40b-110">Value</span></span>|<span data-ttu-id="cc40b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc40b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc40b-112">нотевалуатед</span><span class="sxs-lookup"><span data-stu-id="cc40b-112">notEvaluated</span></span>|<span data-ttu-id="cc40b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="cc40b-113">0</span></span>|<span data-ttu-id="cc40b-114">Указывает, что встроенный код активации SIM-карты свободен и доступен для назначения устройству.</span><span class="sxs-lookup"><span data-stu-id="cc40b-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="cc40b-115">сбоев</span><span class="sxs-lookup"><span data-stu-id="cc40b-115">failed</span></span>|<span data-ttu-id="cc40b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="cc40b-116">1</span></span>|<span data-ttu-id="cc40b-117">Указывает, что службе Intune не удалось доставить этот профиль устройству.</span><span class="sxs-lookup"><span data-stu-id="cc40b-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="cc40b-118">устанавливать</span><span class="sxs-lookup"><span data-stu-id="cc40b-118">installing</span></span>|<span data-ttu-id="cc40b-119">2</span><span class="sxs-lookup"><span data-stu-id="cc40b-119">2</span></span>|<span data-ttu-id="cc40b-120">Указывает, что встроенный код активации SIM-карты назначен устройству, и устройство устанавливает маркер.</span><span class="sxs-lookup"><span data-stu-id="cc40b-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="cc40b-121">устанавлива</span><span class="sxs-lookup"><span data-stu-id="cc40b-121">installed</span></span>|<span data-ttu-id="cc40b-122">4</span><span class="sxs-lookup"><span data-stu-id="cc40b-122">3</span></span>|<span data-ttu-id="cc40b-123">Указывает на то, что встроенный код активации SIM-карты успешно установлен на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="cc40b-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="cc40b-124">удалять</span><span class="sxs-lookup"><span data-stu-id="cc40b-124">deleting</span></span>|<span data-ttu-id="cc40b-125">4 </span><span class="sxs-lookup"><span data-stu-id="cc40b-125">4</span></span>|<span data-ttu-id="cc40b-126">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="cc40b-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="cc40b-127">error</span><span class="sxs-lookup"><span data-stu-id="cc40b-127">error</span></span>|<span data-ttu-id="cc40b-128">5 </span><span class="sxs-lookup"><span data-stu-id="cc40b-128">5</span></span>|<span data-ttu-id="cc40b-129">Указывает на наличие ошибки в этом профиле.</span><span class="sxs-lookup"><span data-stu-id="cc40b-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="cc40b-130">deleted</span><span class="sxs-lookup"><span data-stu-id="cc40b-130">deleted</span></span>|<span data-ttu-id="cc40b-131">6 </span><span class="sxs-lookup"><span data-stu-id="cc40b-131">6</span></span>|<span data-ttu-id="cc40b-132">Указывает, что профиль будет удален с устройства.</span><span class="sxs-lookup"><span data-stu-id="cc40b-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="cc40b-133">ремоведбюсер</span><span class="sxs-lookup"><span data-stu-id="cc40b-133">removedByUser</span></span>|<span data-ttu-id="cc40b-134">7 </span><span class="sxs-lookup"><span data-stu-id="cc40b-134">7</span></span>|<span data-ttu-id="cc40b-135">Указывает, что профиль удаляется с устройства пользователем</span><span class="sxs-lookup"><span data-stu-id="cc40b-135">Designates that the profile is removed from the device by the user</span></span>|





