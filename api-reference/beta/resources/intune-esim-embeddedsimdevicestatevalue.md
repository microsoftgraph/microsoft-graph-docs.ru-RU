---
title: тип перечисления Ембеддедсимдевицестатевалуе
description: Описывает различные состояния для встроенного кода активации SIM-карты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a4369a891af8ebdda818a0e7b62d4c8d827d029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326718"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="82f25-103">тип перечисления Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="82f25-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="82f25-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82f25-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82f25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f25-106">Описывает различные состояния для встроенного кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="82f25-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="82f25-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="82f25-107">Members</span></span>
|<span data-ttu-id="82f25-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="82f25-108">Member</span></span>|<span data-ttu-id="82f25-109">Значение</span><span class="sxs-lookup"><span data-stu-id="82f25-109">Value</span></span>|<span data-ttu-id="82f25-110">Описание</span><span class="sxs-lookup"><span data-stu-id="82f25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f25-111">нотевалуатед</span><span class="sxs-lookup"><span data-stu-id="82f25-111">notEvaluated</span></span>|<span data-ttu-id="82f25-112">нуль</span><span class="sxs-lookup"><span data-stu-id="82f25-112">0</span></span>|<span data-ttu-id="82f25-113">Указывает, что встроенный код активации SIM-карты свободен и доступен для назначения устройству.</span><span class="sxs-lookup"><span data-stu-id="82f25-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="82f25-114">сбоев</span><span class="sxs-lookup"><span data-stu-id="82f25-114">failed</span></span>|<span data-ttu-id="82f25-115">1,1</span><span class="sxs-lookup"><span data-stu-id="82f25-115">1</span></span>|<span data-ttu-id="82f25-116">Указывает, что службе Intune не удалось доставить этот профиль устройству.</span><span class="sxs-lookup"><span data-stu-id="82f25-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="82f25-117">устанавливать</span><span class="sxs-lookup"><span data-stu-id="82f25-117">installing</span></span>|<span data-ttu-id="82f25-118">2</span><span class="sxs-lookup"><span data-stu-id="82f25-118">2</span></span>|<span data-ttu-id="82f25-119">Указывает, что встроенный код активации SIM-карты назначен устройству, и устройство устанавливает маркер.</span><span class="sxs-lookup"><span data-stu-id="82f25-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="82f25-120">устанавлива</span><span class="sxs-lookup"><span data-stu-id="82f25-120">installed</span></span>|<span data-ttu-id="82f25-121">4</span><span class="sxs-lookup"><span data-stu-id="82f25-121">3</span></span>|<span data-ttu-id="82f25-122">Указывает на то, что встроенный код активации SIM-карты успешно установлен на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="82f25-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="82f25-123">удалять</span><span class="sxs-lookup"><span data-stu-id="82f25-123">deleting</span></span>|<span data-ttu-id="82f25-124">SP4</span><span class="sxs-lookup"><span data-stu-id="82f25-124">4</span></span>|<span data-ttu-id="82f25-125">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="82f25-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="82f25-126">error</span><span class="sxs-lookup"><span data-stu-id="82f25-126">error</span></span>|<span data-ttu-id="82f25-127">17:00</span><span class="sxs-lookup"><span data-stu-id="82f25-127">5</span></span>|<span data-ttu-id="82f25-128">Указывает на наличие ошибки в этом профиле.</span><span class="sxs-lookup"><span data-stu-id="82f25-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="82f25-129">deleted</span><span class="sxs-lookup"><span data-stu-id="82f25-129">deleted</span></span>|<span data-ttu-id="82f25-130">6 </span><span class="sxs-lookup"><span data-stu-id="82f25-130">6</span></span>|<span data-ttu-id="82f25-131">Указывает, что профиль будет удален с устройства.</span><span class="sxs-lookup"><span data-stu-id="82f25-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="82f25-132">ремоведбюсер</span><span class="sxs-lookup"><span data-stu-id="82f25-132">removedByUser</span></span>|<span data-ttu-id="82f25-133">7 </span><span class="sxs-lookup"><span data-stu-id="82f25-133">7</span></span>|<span data-ttu-id="82f25-134">Указывает, что профиль удаляется с устройства пользователем</span><span class="sxs-lookup"><span data-stu-id="82f25-134">Designates that the profile is removed from the device by the user</span></span>|



