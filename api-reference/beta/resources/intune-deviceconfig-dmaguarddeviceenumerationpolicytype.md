---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e3289a40916d4942980274e2375aefdf6081934c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791970"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="b8f96-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="b8f96-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="b8f96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8f96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8f96-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8f96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8f96-106">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="b8f96-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="b8f96-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8f96-107">Members</span></span>
|<span data-ttu-id="b8f96-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8f96-108">Member</span></span>|<span data-ttu-id="b8f96-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b8f96-109">Value</span></span>|<span data-ttu-id="b8f96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8f96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8f96-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b8f96-111">deviceDefault</span></span>|<span data-ttu-id="b8f96-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b8f96-112">0</span></span>|<span data-ttu-id="b8f96-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b8f96-113">Default value.</span></span> <span data-ttu-id="b8f96-114">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="b8f96-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="b8f96-115">блоккалл</span><span class="sxs-lookup"><span data-stu-id="b8f96-115">blockAll</span></span>|<span data-ttu-id="b8f96-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b8f96-116">1</span></span>|<span data-ttu-id="b8f96-117">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="b8f96-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="b8f96-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="b8f96-118">allowAll</span></span>|<span data-ttu-id="b8f96-119">2</span><span class="sxs-lookup"><span data-stu-id="b8f96-119">2</span></span>|<span data-ttu-id="b8f96-120">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="b8f96-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



