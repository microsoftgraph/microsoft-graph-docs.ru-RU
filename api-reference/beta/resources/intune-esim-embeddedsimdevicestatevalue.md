---
title: тип перечисления Ембеддедсимдевицестатевалуе
description: Описывает различные состояния для встроенного кода активации SIM-карты.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a4970e08ff9b305aaf2aad4d82daf994d2010bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568768"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="39f86-103">тип перечисления Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="39f86-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="39f86-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39f86-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f86-106">Описывает различные состояния для встроенного кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="39f86-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="39f86-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="39f86-107">Members</span></span>
|<span data-ttu-id="39f86-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="39f86-108">Member</span></span>|<span data-ttu-id="39f86-109">Значение</span><span class="sxs-lookup"><span data-stu-id="39f86-109">Value</span></span>|<span data-ttu-id="39f86-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39f86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f86-111">Нотевалуатед</span><span class="sxs-lookup"><span data-stu-id="39f86-111">notEvaluated</span></span>|<span data-ttu-id="39f86-112">нуль</span><span class="sxs-lookup"><span data-stu-id="39f86-112">0</span></span>|<span data-ttu-id="39f86-113">Указывает, что встроенный код активации SIM-карты свободен и доступен для назначения устройству.</span><span class="sxs-lookup"><span data-stu-id="39f86-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="39f86-114">сбоев</span><span class="sxs-lookup"><span data-stu-id="39f86-114">failed</span></span>|<span data-ttu-id="39f86-115">1 </span><span class="sxs-lookup"><span data-stu-id="39f86-115">1</span></span>|<span data-ttu-id="39f86-116">Указывает, что службе Intune не удалось доставить этот профиль устройству.</span><span class="sxs-lookup"><span data-stu-id="39f86-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="39f86-117">устанавливать</span><span class="sxs-lookup"><span data-stu-id="39f86-117">installing</span></span>|<span data-ttu-id="39f86-118">2 </span><span class="sxs-lookup"><span data-stu-id="39f86-118">2</span></span>|<span data-ttu-id="39f86-119">Указывает, что встроенный код активации SIM-карты назначен устройству, и устройство устанавливает маркер.</span><span class="sxs-lookup"><span data-stu-id="39f86-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="39f86-120">устанавлива</span><span class="sxs-lookup"><span data-stu-id="39f86-120">installed</span></span>|<span data-ttu-id="39f86-121">3 </span><span class="sxs-lookup"><span data-stu-id="39f86-121">3</span></span>|<span data-ttu-id="39f86-122">Указывает на то, что встроенный код активации SIM-карты успешно установлен на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="39f86-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="39f86-123">удалять</span><span class="sxs-lookup"><span data-stu-id="39f86-123">deleting</span></span>|<span data-ttu-id="39f86-124">4 </span><span class="sxs-lookup"><span data-stu-id="39f86-124">4</span></span>|<span data-ttu-id="39f86-125">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="39f86-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="39f86-126">error</span><span class="sxs-lookup"><span data-stu-id="39f86-126">error</span></span>|<span data-ttu-id="39f86-127">5 </span><span class="sxs-lookup"><span data-stu-id="39f86-127">5</span></span>|<span data-ttu-id="39f86-128">Указывает на наличие ошибки в этом профиле.</span><span class="sxs-lookup"><span data-stu-id="39f86-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="39f86-129">deleted</span><span class="sxs-lookup"><span data-stu-id="39f86-129">deleted</span></span>|<span data-ttu-id="39f86-130">6 </span><span class="sxs-lookup"><span data-stu-id="39f86-130">6</span></span>|<span data-ttu-id="39f86-131">Указывает, что профиль будет удален с устройства.</span><span class="sxs-lookup"><span data-stu-id="39f86-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="39f86-132">Ремоведбюсер</span><span class="sxs-lookup"><span data-stu-id="39f86-132">removedByUser</span></span>|<span data-ttu-id="39f86-133">7 </span><span class="sxs-lookup"><span data-stu-id="39f86-133">7</span></span>|<span data-ttu-id="39f86-134">Указывает, что профиль удаляется с устройства пользователем</span><span class="sxs-lookup"><span data-stu-id="39f86-134">Designates that the profile is removed from the device by the user</span></span>|





