---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f1238c423fc12605c8ca2d3a8828d814a74b288
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701580"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="30654-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="30654-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="30654-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30654-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30654-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30654-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30654-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30654-107">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="30654-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="30654-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="30654-108">Members</span></span>
|<span data-ttu-id="30654-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="30654-109">Member</span></span>|<span data-ttu-id="30654-110">Значение</span><span class="sxs-lookup"><span data-stu-id="30654-110">Value</span></span>|<span data-ttu-id="30654-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30654-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30654-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="30654-112">deviceDefault</span></span>|<span data-ttu-id="30654-113">нуль</span><span class="sxs-lookup"><span data-stu-id="30654-113">0</span></span>|<span data-ttu-id="30654-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="30654-114">Default value.</span></span> <span data-ttu-id="30654-115">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="30654-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="30654-116">блоккалл</span><span class="sxs-lookup"><span data-stu-id="30654-116">blockAll</span></span>|<span data-ttu-id="30654-117">1,1</span><span class="sxs-lookup"><span data-stu-id="30654-117">1</span></span>|<span data-ttu-id="30654-118">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="30654-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="30654-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="30654-119">allowAll</span></span>|<span data-ttu-id="30654-120">2</span><span class="sxs-lookup"><span data-stu-id="30654-120">2</span></span>|<span data-ttu-id="30654-121">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="30654-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





