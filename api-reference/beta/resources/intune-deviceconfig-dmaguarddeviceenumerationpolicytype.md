---
title: Тип перечисления dmaGuardDeviceEnumerationPolicyType
description: Возможные значения DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430778"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="4578c-103">Тип перечисления dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="4578c-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="4578c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4578c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4578c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4578c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4578c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4578c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4578c-107">Возможные значения DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="4578c-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="4578c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4578c-108">Members</span></span>
|<span data-ttu-id="4578c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4578c-109">Member</span></span>|<span data-ttu-id="4578c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4578c-110">Value</span></span>|<span data-ttu-id="4578c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4578c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4578c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4578c-112">deviceDefault</span></span>|<span data-ttu-id="4578c-113">0</span><span class="sxs-lookup"><span data-stu-id="4578c-113">0</span></span>|<span data-ttu-id="4578c-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4578c-114">Default value.</span></span> <span data-ttu-id="4578c-115">Устройства с DMA сопоставление несовместимые драйверы будут перечислены только после пользователь разблокирует экрана.</span><span class="sxs-lookup"><span data-stu-id="4578c-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="4578c-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="4578c-116">blockAll</span></span>|<span data-ttu-id="4578c-117">1</span><span class="sxs-lookup"><span data-stu-id="4578c-117">1</span></span>|<span data-ttu-id="4578c-118">Устройства с DMA сопоставление драйверы, несовместимые с никогда не смогут запуск и выполнение DMA в любое время.</span><span class="sxs-lookup"><span data-stu-id="4578c-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="4578c-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="4578c-119">allowAll</span></span>|<span data-ttu-id="4578c-120">2</span><span class="sxs-lookup"><span data-stu-id="4578c-120">2</span></span>|<span data-ttu-id="4578c-121">Все внешние DMA PCIe устройств с поддержкой будут перечислены в любое время.</span><span class="sxs-lookup"><span data-stu-id="4578c-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




