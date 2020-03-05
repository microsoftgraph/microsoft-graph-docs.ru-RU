---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97f04bbf16d93602be466e4dc5fe4986cc26319e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530138"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="f6223-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="f6223-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="f6223-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6223-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6223-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6223-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6223-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6223-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6223-107">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="f6223-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="f6223-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f6223-108">Members</span></span>
|<span data-ttu-id="f6223-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f6223-109">Member</span></span>|<span data-ttu-id="f6223-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f6223-110">Value</span></span>|<span data-ttu-id="f6223-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f6223-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6223-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f6223-112">notConfigured</span></span>|<span data-ttu-id="f6223-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f6223-113">0</span></span>|<span data-ttu-id="f6223-114">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="f6223-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="f6223-115">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="f6223-115">enableWithUEFILock</span></span>|<span data-ttu-id="f6223-116">1 </span><span class="sxs-lookup"><span data-stu-id="f6223-116">1</span></span>|<span data-ttu-id="f6223-117">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="f6223-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="f6223-118">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="f6223-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="f6223-119">2 </span><span class="sxs-lookup"><span data-stu-id="f6223-119">2</span></span>|<span data-ttu-id="f6223-120">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="f6223-120">Turns on Credential Guard without UEFI lock.</span></span>|



