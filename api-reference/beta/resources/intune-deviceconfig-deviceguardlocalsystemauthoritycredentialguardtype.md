---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f22336a37c3d10d4e86b3db2af41e8103dcfe33
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774871"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="4cf9b-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="4cf9b-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="4cf9b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cf9b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf9b-106">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="4cf9b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4cf9b-107">Members</span></span>
|<span data-ttu-id="4cf9b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4cf9b-108">Member</span></span>|<span data-ttu-id="4cf9b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4cf9b-109">Value</span></span>|<span data-ttu-id="4cf9b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4cf9b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf9b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4cf9b-111">notConfigured</span></span>|<span data-ttu-id="4cf9b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4cf9b-112">0</span></span>|<span data-ttu-id="4cf9b-113">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="4cf9b-114">Енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="4cf9b-114">enableWithUEFILock</span></span>|<span data-ttu-id="4cf9b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4cf9b-115">1</span></span>|<span data-ttu-id="4cf9b-116">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="4cf9b-117">Енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="4cf9b-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="4cf9b-118">2</span><span class="sxs-lookup"><span data-stu-id="4cf9b-118">2</span></span>|<span data-ttu-id="4cf9b-119">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="4cf9b-119">Turns on Credential Guard without UEFI lock.</span></span>|





