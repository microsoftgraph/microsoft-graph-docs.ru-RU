---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00bf6986f37bd5fd1aae4991dbb7eb5b215e4c6e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001546"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="227c8-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="227c8-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="227c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="227c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="227c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227c8-106">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="227c8-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="227c8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="227c8-107">Members</span></span>
|<span data-ttu-id="227c8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="227c8-108">Member</span></span>|<span data-ttu-id="227c8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="227c8-109">Value</span></span>|<span data-ttu-id="227c8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="227c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227c8-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="227c8-111">deviceDefault</span></span>|<span data-ttu-id="227c8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="227c8-112">0</span></span>|<span data-ttu-id="227c8-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="227c8-113">Default value.</span></span> <span data-ttu-id="227c8-114">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="227c8-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="227c8-115">Блоккалл</span><span class="sxs-lookup"><span data-stu-id="227c8-115">blockAll</span></span>|<span data-ttu-id="227c8-116">1,1</span><span class="sxs-lookup"><span data-stu-id="227c8-116">1</span></span>|<span data-ttu-id="227c8-117">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="227c8-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="227c8-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="227c8-118">allowAll</span></span>|<span data-ttu-id="227c8-119">2</span><span class="sxs-lookup"><span data-stu-id="227c8-119">2</span></span>|<span data-ttu-id="227c8-120">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="227c8-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





