---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 484e7ffbd13234a24be983af1d94e8dca0d55f34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332696"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="6bed5-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="6bed5-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="6bed5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bed5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bed5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bed5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bed5-106">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="6bed5-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="6bed5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6bed5-107">Members</span></span>
|<span data-ttu-id="6bed5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6bed5-108">Member</span></span>|<span data-ttu-id="6bed5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6bed5-109">Value</span></span>|<span data-ttu-id="6bed5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6bed5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bed5-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="6bed5-111">deviceDefault</span></span>|<span data-ttu-id="6bed5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6bed5-112">0</span></span>|<span data-ttu-id="6bed5-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6bed5-113">Default value.</span></span> <span data-ttu-id="6bed5-114">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="6bed5-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="6bed5-115">блоккалл</span><span class="sxs-lookup"><span data-stu-id="6bed5-115">blockAll</span></span>|<span data-ttu-id="6bed5-116">1,1</span><span class="sxs-lookup"><span data-stu-id="6bed5-116">1</span></span>|<span data-ttu-id="6bed5-117">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="6bed5-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="6bed5-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="6bed5-118">allowAll</span></span>|<span data-ttu-id="6bed5-119">2</span><span class="sxs-lookup"><span data-stu-id="6bed5-119">2</span></span>|<span data-ttu-id="6bed5-120">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="6bed5-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



