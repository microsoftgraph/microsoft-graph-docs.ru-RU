---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4d063858501bb8741000234bde8ade8d33550c9f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359743"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="720a3-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="720a3-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="720a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="720a3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="720a3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="720a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="720a3-107">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="720a3-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="720a3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="720a3-108">Members</span></span>
|<span data-ttu-id="720a3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="720a3-109">Member</span></span>|<span data-ttu-id="720a3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="720a3-110">Value</span></span>|<span data-ttu-id="720a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="720a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="720a3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="720a3-112">notConfigured</span></span>|<span data-ttu-id="720a3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="720a3-113">0</span></span>|<span data-ttu-id="720a3-114">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="720a3-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="720a3-115">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="720a3-115">enableWithUEFILock</span></span>|<span data-ttu-id="720a3-116">1,1</span><span class="sxs-lookup"><span data-stu-id="720a3-116">1</span></span>|<span data-ttu-id="720a3-117">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="720a3-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="720a3-118">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="720a3-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="720a3-119">2</span><span class="sxs-lookup"><span data-stu-id="720a3-119">2</span></span>|<span data-ttu-id="720a3-120">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="720a3-120">Turns on Credential Guard without UEFI lock.</span></span>|



