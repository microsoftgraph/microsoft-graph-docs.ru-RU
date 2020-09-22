---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2296198c9e433fbaf7d6499eca7737306c581618
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058320"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="bee9c-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="bee9c-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="bee9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bee9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bee9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bee9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bee9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bee9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee9c-107">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="bee9c-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="bee9c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bee9c-108">Members</span></span>
|<span data-ttu-id="bee9c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bee9c-109">Member</span></span>|<span data-ttu-id="bee9c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bee9c-110">Value</span></span>|<span data-ttu-id="bee9c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bee9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee9c-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="bee9c-112">deviceDefault</span></span>|<span data-ttu-id="bee9c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="bee9c-113">0</span></span>|<span data-ttu-id="bee9c-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bee9c-114">Default value.</span></span> <span data-ttu-id="bee9c-115">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="bee9c-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="bee9c-116">блоккалл</span><span class="sxs-lookup"><span data-stu-id="bee9c-116">blockAll</span></span>|<span data-ttu-id="bee9c-117">1 </span><span class="sxs-lookup"><span data-stu-id="bee9c-117">1</span></span>|<span data-ttu-id="bee9c-118">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="bee9c-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="bee9c-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="bee9c-119">allowAll</span></span>|<span data-ttu-id="bee9c-120">2 </span><span class="sxs-lookup"><span data-stu-id="bee9c-120">2</span></span>|<span data-ttu-id="bee9c-121">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="bee9c-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|






