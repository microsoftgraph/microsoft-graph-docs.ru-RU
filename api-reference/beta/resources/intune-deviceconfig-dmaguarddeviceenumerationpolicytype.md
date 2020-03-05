---
title: тип перечисления Дмагуарддевицеенумератионполицитипе
description: Возможные значения параметра Дмагуарддевицеенумератионполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03e93e6ad3e5dae8a455bb3ceb9aa65f11dcf2e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526575"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="5151c-103">тип перечисления Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="5151c-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="5151c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5151c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5151c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5151c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5151c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5151c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5151c-107">Возможные значения параметра Дмагуарддевицеенумератионполици.</span><span class="sxs-lookup"><span data-stu-id="5151c-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="5151c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5151c-108">Members</span></span>
|<span data-ttu-id="5151c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5151c-109">Member</span></span>|<span data-ttu-id="5151c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5151c-110">Value</span></span>|<span data-ttu-id="5151c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5151c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5151c-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="5151c-112">deviceDefault</span></span>|<span data-ttu-id="5151c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5151c-113">0</span></span>|<span data-ttu-id="5151c-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5151c-114">Default value.</span></span> <span data-ttu-id="5151c-115">Устройства с перераспределением DMA несовместимые драйверы будут перечисляться только после того, как пользователь разблокирует экран.</span><span class="sxs-lookup"><span data-stu-id="5151c-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="5151c-116">блоккалл</span><span class="sxs-lookup"><span data-stu-id="5151c-116">blockAll</span></span>|<span data-ttu-id="5151c-117">1 </span><span class="sxs-lookup"><span data-stu-id="5151c-117">1</span></span>|<span data-ttu-id="5151c-118">Устройства с пересопоставлением DMA несовместимые драйверы никогда не будут иметь разрешения на запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="5151c-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="5151c-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="5151c-119">allowAll</span></span>|<span data-ttu-id="5151c-120">2 </span><span class="sxs-lookup"><span data-stu-id="5151c-120">2</span></span>|<span data-ttu-id="5151c-121">Все внешние устройства с поддержкой прямого доступа к памяти PCIe будут перечисляться в любое время.</span><span class="sxs-lookup"><span data-stu-id="5151c-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



