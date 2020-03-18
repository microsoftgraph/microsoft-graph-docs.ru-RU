---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c9532485213c97ac500057842cdcc3e5cbb6719b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792047"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="b8dff-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="b8dff-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="b8dff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8dff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8dff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8dff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8dff-106">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="b8dff-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="b8dff-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8dff-107">Members</span></span>
|<span data-ttu-id="b8dff-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8dff-108">Member</span></span>|<span data-ttu-id="b8dff-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b8dff-109">Value</span></span>|<span data-ttu-id="b8dff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8dff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8dff-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8dff-111">notConfigured</span></span>|<span data-ttu-id="b8dff-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b8dff-112">0</span></span>|<span data-ttu-id="b8dff-113">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="b8dff-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="b8dff-114">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="b8dff-114">enableWithUEFILock</span></span>|<span data-ttu-id="b8dff-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b8dff-115">1</span></span>|<span data-ttu-id="b8dff-116">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="b8dff-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="b8dff-117">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="b8dff-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="b8dff-118">2</span><span class="sxs-lookup"><span data-stu-id="b8dff-118">2</span></span>|<span data-ttu-id="b8dff-119">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="b8dff-119">Turns on Credential Guard without UEFI lock.</span></span>|



