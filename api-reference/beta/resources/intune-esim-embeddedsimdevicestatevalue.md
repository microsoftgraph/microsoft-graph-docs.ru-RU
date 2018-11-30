---
title: Тип перечисления embeddedSIMDeviceStateValue
description: Описание различных состояний для внедренного код активации диспетчера установки.
ms.openlocfilehash: c0b1cffedcae18dab4c1d23a2691cafa8709c0ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075923"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="b6e29-103">Тип перечисления embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="b6e29-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="b6e29-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6e29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6e29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6e29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6e29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6e29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6e29-107">Описание различных состояний для внедренного код активации диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="b6e29-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="b6e29-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b6e29-108">Members</span></span>
|<span data-ttu-id="b6e29-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b6e29-109">Member</span></span>|<span data-ttu-id="b6e29-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b6e29-110">Value</span></span>|<span data-ttu-id="b6e29-111">Description</span><span class="sxs-lookup"><span data-stu-id="b6e29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e29-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="b6e29-112">notEvaluated</span></span>|<span data-ttu-id="b6e29-113">0</span><span class="sxs-lookup"><span data-stu-id="b6e29-113">0</span></span>|<span data-ttu-id="b6e29-114">Определяет, что встроенный код активации диспетчера установки, бесплатное и доступно для назначения устройства.</span><span class="sxs-lookup"><span data-stu-id="b6e29-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="b6e29-115">failed</span><span class="sxs-lookup"><span data-stu-id="b6e29-115">failed</span></span>|<span data-ttu-id="b6e29-116">1</span><span class="sxs-lookup"><span data-stu-id="b6e29-116">1</span></span>|<span data-ttu-id="b6e29-117">Указывает, что служба Intune не удалось доставить этот профиль с устройством.</span><span class="sxs-lookup"><span data-stu-id="b6e29-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="b6e29-118">Установка</span><span class="sxs-lookup"><span data-stu-id="b6e29-118">installing</span></span>|<span data-ttu-id="b6e29-119">2</span><span class="sxs-lookup"><span data-stu-id="b6e29-119">2</span></span>|<span data-ttu-id="b6e29-120">Определяет, что встроенный код активации диспетчера установки была назначена устройства и устройства выполняется установка маркер.</span><span class="sxs-lookup"><span data-stu-id="b6e29-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="b6e29-121">установлен</span><span class="sxs-lookup"><span data-stu-id="b6e29-121">installed</span></span>|<span data-ttu-id="b6e29-122">3</span><span class="sxs-lookup"><span data-stu-id="b6e29-122">3</span></span>|<span data-ttu-id="b6e29-123">Определяет, что внедренный код активации диспетчера установки был успешно установлен на устройстве конечного.</span><span class="sxs-lookup"><span data-stu-id="b6e29-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="b6e29-124">удаление</span><span class="sxs-lookup"><span data-stu-id="b6e29-124">deleting</span></span>|<span data-ttu-id="b6e29-125">4</span><span class="sxs-lookup"><span data-stu-id="b6e29-125">4</span></span>|<span data-ttu-id="b6e29-126">Указывает, что служба Intune пытается удалить профиль с устройства.</span><span class="sxs-lookup"><span data-stu-id="b6e29-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="b6e29-127">error</span><span class="sxs-lookup"><span data-stu-id="b6e29-127">error</span></span>|<span data-ttu-id="b6e29-128">5</span><span class="sxs-lookup"><span data-stu-id="b6e29-128">5</span></span>|<span data-ttu-id="b6e29-129">Определяет, что, ошибка с этим профилем.</span><span class="sxs-lookup"><span data-stu-id="b6e29-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="b6e29-130">deleted</span><span class="sxs-lookup"><span data-stu-id="b6e29-130">deleted</span></span>|<span data-ttu-id="b6e29-131">6</span><span class="sxs-lookup"><span data-stu-id="b6e29-131">6</span></span>|<span data-ttu-id="b6e29-132">Определяет, что профиль будет удален из устройства.</span><span class="sxs-lookup"><span data-stu-id="b6e29-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="b6e29-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="b6e29-133">removedByUser</span></span>|<span data-ttu-id="b6e29-134">7</span><span class="sxs-lookup"><span data-stu-id="b6e29-134">7</span></span>|<span data-ttu-id="b6e29-135">Указывает, что профиль было удалено пользователем с устройства</span><span class="sxs-lookup"><span data-stu-id="b6e29-135">Designates that the profile is removed from the device by the user</span></span>|





