---
title: тип перечисления Ембеддедсимдевицестатевалуе
description: Описывает различные состояния для встроенного кода активации SIM-карты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb2ab50e9c91f801cc38723a58bed2867c71b347
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528205"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="dbf7e-103">тип перечисления Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="dbf7e-103">embeddedSIMDeviceStateValue enum type</span></span>

<span data-ttu-id="dbf7e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dbf7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbf7e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbf7e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf7e-107">Описывает различные состояния для встроенного кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="dbf7e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dbf7e-108">Members</span></span>
|<span data-ttu-id="dbf7e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dbf7e-109">Member</span></span>|<span data-ttu-id="dbf7e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dbf7e-110">Value</span></span>|<span data-ttu-id="dbf7e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf7e-112">нотевалуатед</span><span class="sxs-lookup"><span data-stu-id="dbf7e-112">notEvaluated</span></span>|<span data-ttu-id="dbf7e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="dbf7e-113">0</span></span>|<span data-ttu-id="dbf7e-114">Указывает, что встроенный код активации SIM-карты свободен и доступен для назначения устройству.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="dbf7e-115">сбоев</span><span class="sxs-lookup"><span data-stu-id="dbf7e-115">failed</span></span>|<span data-ttu-id="dbf7e-116">1 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-116">1</span></span>|<span data-ttu-id="dbf7e-117">Указывает, что службе Intune не удалось доставить этот профиль устройству.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="dbf7e-118">устанавливать</span><span class="sxs-lookup"><span data-stu-id="dbf7e-118">installing</span></span>|<span data-ttu-id="dbf7e-119">2 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-119">2</span></span>|<span data-ttu-id="dbf7e-120">Указывает, что встроенный код активации SIM-карты назначен устройству, и устройство устанавливает маркер.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="dbf7e-121">устанавлива</span><span class="sxs-lookup"><span data-stu-id="dbf7e-121">installed</span></span>|<span data-ttu-id="dbf7e-122">3 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-122">3</span></span>|<span data-ttu-id="dbf7e-123">Указывает на то, что встроенный код активации SIM-карты успешно установлен на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="dbf7e-124">удалять</span><span class="sxs-lookup"><span data-stu-id="dbf7e-124">deleting</span></span>|<span data-ttu-id="dbf7e-125">4 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-125">4</span></span>|<span data-ttu-id="dbf7e-126">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="dbf7e-127">error</span><span class="sxs-lookup"><span data-stu-id="dbf7e-127">error</span></span>|<span data-ttu-id="dbf7e-128">5 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-128">5</span></span>|<span data-ttu-id="dbf7e-129">Указывает на наличие ошибки в этом профиле.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="dbf7e-130">deleted</span><span class="sxs-lookup"><span data-stu-id="dbf7e-130">deleted</span></span>|<span data-ttu-id="dbf7e-131">6 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-131">6</span></span>|<span data-ttu-id="dbf7e-132">Указывает, что профиль будет удален с устройства.</span><span class="sxs-lookup"><span data-stu-id="dbf7e-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="dbf7e-133">ремоведбюсер</span><span class="sxs-lookup"><span data-stu-id="dbf7e-133">removedByUser</span></span>|<span data-ttu-id="dbf7e-134">7 </span><span class="sxs-lookup"><span data-stu-id="dbf7e-134">7</span></span>|<span data-ttu-id="dbf7e-135">Указывает, что профиль удаляется с устройства пользователем</span><span class="sxs-lookup"><span data-stu-id="dbf7e-135">Designates that the profile is removed from the device by the user</span></span>|



