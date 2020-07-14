---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b02402ff6c6c0373396bd6fca0cad6ded5cb36d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123773"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="76152-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="76152-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="76152-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76152-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76152-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76152-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76152-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76152-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76152-107">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="76152-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="76152-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="76152-108">Members</span></span>
|<span data-ttu-id="76152-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="76152-109">Member</span></span>|<span data-ttu-id="76152-110">Значение</span><span class="sxs-lookup"><span data-stu-id="76152-110">Value</span></span>|<span data-ttu-id="76152-111">Описание</span><span class="sxs-lookup"><span data-stu-id="76152-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76152-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="76152-112">notConfigured</span></span>|<span data-ttu-id="76152-113">нуль</span><span class="sxs-lookup"><span data-stu-id="76152-113">0</span></span>|<span data-ttu-id="76152-114">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="76152-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="76152-115">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="76152-115">enableWithUEFILock</span></span>|<span data-ttu-id="76152-116">1 </span><span class="sxs-lookup"><span data-stu-id="76152-116">1</span></span>|<span data-ttu-id="76152-117">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="76152-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="76152-118">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="76152-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="76152-119">2 </span><span class="sxs-lookup"><span data-stu-id="76152-119">2</span></span>|<span data-ttu-id="76152-120">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="76152-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="76152-121">отключение</span><span class="sxs-lookup"><span data-stu-id="76152-121">disable</span></span>|<span data-ttu-id="76152-122">3 </span><span class="sxs-lookup"><span data-stu-id="76152-122">3</span></span>|<span data-ttu-id="76152-123">Отключает защиту учетных данных.</span><span class="sxs-lookup"><span data-stu-id="76152-123">Disables Credential Guard.</span></span> <span data-ttu-id="76152-124">Это значение ОС по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="76152-124">This is the default OS value.</span></span>|



