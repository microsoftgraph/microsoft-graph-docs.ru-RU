---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe99f1896a58839d40becc6e899bab2c69e59f46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985960"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="a5920-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="a5920-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="a5920-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5920-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5920-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5920-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5920-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5920-107">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="a5920-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="a5920-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a5920-108">Members</span></span>
|<span data-ttu-id="a5920-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5920-109">Member</span></span>|<span data-ttu-id="a5920-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a5920-110">Value</span></span>|<span data-ttu-id="a5920-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5920-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5920-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a5920-112">notConfigured</span></span>|<span data-ttu-id="a5920-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a5920-113">0</span></span>|<span data-ttu-id="a5920-114">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="a5920-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="a5920-115">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="a5920-115">enableWithUEFILock</span></span>|<span data-ttu-id="a5920-116">1 </span><span class="sxs-lookup"><span data-stu-id="a5920-116">1</span></span>|<span data-ttu-id="a5920-117">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="a5920-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="a5920-118">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="a5920-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="a5920-119">2 </span><span class="sxs-lookup"><span data-stu-id="a5920-119">2</span></span>|<span data-ttu-id="a5920-120">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="a5920-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="a5920-121">отключение</span><span class="sxs-lookup"><span data-stu-id="a5920-121">disable</span></span>|<span data-ttu-id="a5920-122">4</span><span class="sxs-lookup"><span data-stu-id="a5920-122">3</span></span>|<span data-ttu-id="a5920-123">Отключает защиту учетных данных.</span><span class="sxs-lookup"><span data-stu-id="a5920-123">Disables Credential Guard.</span></span> <span data-ttu-id="a5920-124">Это значение ОС по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5920-124">This is the default OS value.</span></span>|






