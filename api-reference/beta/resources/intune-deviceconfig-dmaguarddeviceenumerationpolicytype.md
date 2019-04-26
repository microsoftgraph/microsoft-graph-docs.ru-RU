---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6910172ef4ab733b09d837dcc9a7196893402ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567160"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="84011-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="84011-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="84011-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84011-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84011-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84011-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84011-106">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="84011-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="84011-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="84011-107">Members</span></span>
|<span data-ttu-id="84011-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="84011-108">Member</span></span>|<span data-ttu-id="84011-109">Значение</span><span class="sxs-lookup"><span data-stu-id="84011-109">Value</span></span>|<span data-ttu-id="84011-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84011-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84011-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="84011-111">deviceDefault</span></span>|<span data-ttu-id="84011-112">нуль</span><span class="sxs-lookup"><span data-stu-id="84011-112">0</span></span>|<span data-ttu-id="84011-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="84011-113">Default value.</span></span> <span data-ttu-id="84011-114">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="84011-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="84011-115">Блоккалл</span><span class="sxs-lookup"><span data-stu-id="84011-115">blockAll</span></span>|<span data-ttu-id="84011-116">1 </span><span class="sxs-lookup"><span data-stu-id="84011-116">1</span></span>|<span data-ttu-id="84011-117">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="84011-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="84011-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="84011-118">allowAll</span></span>|<span data-ttu-id="84011-119">2 </span><span class="sxs-lookup"><span data-stu-id="84011-119">2</span></span>|<span data-ttu-id="84011-120">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="84011-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





