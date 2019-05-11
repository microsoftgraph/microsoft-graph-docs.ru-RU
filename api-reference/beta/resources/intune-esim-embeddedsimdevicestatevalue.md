---
title: тип перечисления Ембеддедсимдевицестатевалуе
description: Описывает различные состояния для встроенного кода активации SIM-карты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1144db582b7e6aa5f38043797cd15f3b009d4d1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941319"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="4a9e7-103">тип перечисления Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="4a9e7-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="4a9e7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a9e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a9e7-106">Описывает различные состояния для встроенного кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="4a9e7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4a9e7-107">Members</span></span>
|<span data-ttu-id="4a9e7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4a9e7-108">Member</span></span>|<span data-ttu-id="4a9e7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4a9e7-109">Value</span></span>|<span data-ttu-id="4a9e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a9e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a9e7-111">Нотевалуатед</span><span class="sxs-lookup"><span data-stu-id="4a9e7-111">notEvaluated</span></span>|<span data-ttu-id="4a9e7-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4a9e7-112">0</span></span>|<span data-ttu-id="4a9e7-113">Указывает, что встроенный код активации SIM-карты свободен и доступен для назначения устройству.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="4a9e7-114">сбоев</span><span class="sxs-lookup"><span data-stu-id="4a9e7-114">failed</span></span>|<span data-ttu-id="4a9e7-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4a9e7-115">1</span></span>|<span data-ttu-id="4a9e7-116">Указывает, что службе Intune не удалось доставить этот профиль устройству.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="4a9e7-117">устанавливать</span><span class="sxs-lookup"><span data-stu-id="4a9e7-117">installing</span></span>|<span data-ttu-id="4a9e7-118">2</span><span class="sxs-lookup"><span data-stu-id="4a9e7-118">2</span></span>|<span data-ttu-id="4a9e7-119">Указывает, что встроенный код активации SIM-карты назначен устройству, и устройство устанавливает маркер.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="4a9e7-120">устанавлива</span><span class="sxs-lookup"><span data-stu-id="4a9e7-120">installed</span></span>|<span data-ttu-id="4a9e7-121">4</span><span class="sxs-lookup"><span data-stu-id="4a9e7-121">3</span></span>|<span data-ttu-id="4a9e7-122">Указывает на то, что встроенный код активации SIM-карты успешно установлен на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="4a9e7-123">удалять</span><span class="sxs-lookup"><span data-stu-id="4a9e7-123">deleting</span></span>|<span data-ttu-id="4a9e7-124">SP4</span><span class="sxs-lookup"><span data-stu-id="4a9e7-124">4</span></span>|<span data-ttu-id="4a9e7-125">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="4a9e7-126">error</span><span class="sxs-lookup"><span data-stu-id="4a9e7-126">error</span></span>|<span data-ttu-id="4a9e7-127">17:00</span><span class="sxs-lookup"><span data-stu-id="4a9e7-127">5</span></span>|<span data-ttu-id="4a9e7-128">Указывает на наличие ошибки в этом профиле.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="4a9e7-129">deleted</span><span class="sxs-lookup"><span data-stu-id="4a9e7-129">deleted</span></span>|<span data-ttu-id="4a9e7-130">6 </span><span class="sxs-lookup"><span data-stu-id="4a9e7-130">6</span></span>|<span data-ttu-id="4a9e7-131">Указывает, что профиль будет удален с устройства.</span><span class="sxs-lookup"><span data-stu-id="4a9e7-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="4a9e7-132">Ремоведбюсер</span><span class="sxs-lookup"><span data-stu-id="4a9e7-132">removedByUser</span></span>|<span data-ttu-id="4a9e7-133">7 </span><span class="sxs-lookup"><span data-stu-id="4a9e7-133">7</span></span>|<span data-ttu-id="4a9e7-134">Указывает, что профиль удаляется с устройства пользователем</span><span class="sxs-lookup"><span data-stu-id="4a9e7-134">Designates that the profile is removed from the device by the user</span></span>|




