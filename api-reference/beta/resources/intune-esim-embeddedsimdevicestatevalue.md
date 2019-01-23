---
title: Тип перечисления embeddedSIMDeviceStateValue
description: Описание различных состояний для внедренного код активации диспетчера установки.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421328"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="abd6b-103">Тип перечисления embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="abd6b-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="abd6b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abd6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="abd6b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abd6b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abd6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abd6b-107">Описание различных состояний для внедренного код активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="abd6b-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="abd6b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="abd6b-108">Members</span></span>
|<span data-ttu-id="abd6b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="abd6b-109">Member</span></span>|<span data-ttu-id="abd6b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="abd6b-110">Value</span></span>|<span data-ttu-id="abd6b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="abd6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abd6b-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="abd6b-112">notEvaluated</span></span>|<span data-ttu-id="abd6b-113">0</span><span class="sxs-lookup"><span data-stu-id="abd6b-113">0</span></span>|<span data-ttu-id="abd6b-114">Определяет, что встроенный код активации диспетчера установки, бесплатное и доступно для назначения устройства.</span><span class="sxs-lookup"><span data-stu-id="abd6b-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="abd6b-115">failed</span><span class="sxs-lookup"><span data-stu-id="abd6b-115">failed</span></span>|<span data-ttu-id="abd6b-116">1</span><span class="sxs-lookup"><span data-stu-id="abd6b-116">1</span></span>|<span data-ttu-id="abd6b-117">Указывает, что служба Intune не удалось доставить этот профиль с устройством.</span><span class="sxs-lookup"><span data-stu-id="abd6b-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="abd6b-118">Установка</span><span class="sxs-lookup"><span data-stu-id="abd6b-118">installing</span></span>|<span data-ttu-id="abd6b-119">2</span><span class="sxs-lookup"><span data-stu-id="abd6b-119">2</span></span>|<span data-ttu-id="abd6b-120">Определяет, что встроенный код активации диспетчера установки была назначена устройства и устройства выполняется установка маркер.</span><span class="sxs-lookup"><span data-stu-id="abd6b-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="abd6b-121">установлен</span><span class="sxs-lookup"><span data-stu-id="abd6b-121">installed</span></span>|<span data-ttu-id="abd6b-122">3</span><span class="sxs-lookup"><span data-stu-id="abd6b-122">3</span></span>|<span data-ttu-id="abd6b-123">Определяет, что внедренный код активации диспетчера установки был успешно установлен на устройстве конечного.</span><span class="sxs-lookup"><span data-stu-id="abd6b-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="abd6b-124">удаление</span><span class="sxs-lookup"><span data-stu-id="abd6b-124">deleting</span></span>|<span data-ttu-id="abd6b-125">4</span><span class="sxs-lookup"><span data-stu-id="abd6b-125">4</span></span>|<span data-ttu-id="abd6b-126">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="abd6b-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="abd6b-127">error</span><span class="sxs-lookup"><span data-stu-id="abd6b-127">error</span></span>|<span data-ttu-id="abd6b-128">5</span><span class="sxs-lookup"><span data-stu-id="abd6b-128">5</span></span>|<span data-ttu-id="abd6b-129">Определяет, что, ошибка с этим профилем.</span><span class="sxs-lookup"><span data-stu-id="abd6b-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="abd6b-130">deleted</span><span class="sxs-lookup"><span data-stu-id="abd6b-130">deleted</span></span>|<span data-ttu-id="abd6b-131">6</span><span class="sxs-lookup"><span data-stu-id="abd6b-131">6</span></span>|<span data-ttu-id="abd6b-132">Определяет, что профиль будет удален из устройства.</span><span class="sxs-lookup"><span data-stu-id="abd6b-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="abd6b-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="abd6b-133">removedByUser</span></span>|<span data-ttu-id="abd6b-134">7</span><span class="sxs-lookup"><span data-stu-id="abd6b-134">7</span></span>|<span data-ttu-id="abd6b-135">Указывает, что профиль было удалено пользователем с устройства</span><span class="sxs-lookup"><span data-stu-id="abd6b-135">Designates that the profile is removed from the device by the user</span></span>|




