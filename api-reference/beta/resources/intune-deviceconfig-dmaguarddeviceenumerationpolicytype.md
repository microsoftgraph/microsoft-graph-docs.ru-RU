---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c46f7e49ad9d9ef31af4ee2d783f171b08c09f1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946884"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="e3100-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="e3100-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="e3100-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3100-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3100-106">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="e3100-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="e3100-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e3100-107">Members</span></span>
|<span data-ttu-id="e3100-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e3100-108">Member</span></span>|<span data-ttu-id="e3100-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e3100-109">Value</span></span>|<span data-ttu-id="e3100-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e3100-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3100-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="e3100-111">deviceDefault</span></span>|<span data-ttu-id="e3100-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e3100-112">0</span></span>|<span data-ttu-id="e3100-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e3100-113">Default value.</span></span> <span data-ttu-id="e3100-114">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="e3100-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="e3100-115">Блоккалл</span><span class="sxs-lookup"><span data-stu-id="e3100-115">blockAll</span></span>|<span data-ttu-id="e3100-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e3100-116">1</span></span>|<span data-ttu-id="e3100-117">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="e3100-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="e3100-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="e3100-118">allowAll</span></span>|<span data-ttu-id="e3100-119">2</span><span class="sxs-lookup"><span data-stu-id="e3100-119">2</span></span>|<span data-ttu-id="e3100-120">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="e3100-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




