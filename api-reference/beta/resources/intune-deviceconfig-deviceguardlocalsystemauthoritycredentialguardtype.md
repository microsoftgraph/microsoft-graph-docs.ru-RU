---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 827b2ba5dac0862ba206a4a742313912f45ceb58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332878"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="64443-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="64443-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="64443-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64443-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64443-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64443-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64443-106">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="64443-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="64443-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="64443-107">Members</span></span>
|<span data-ttu-id="64443-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="64443-108">Member</span></span>|<span data-ttu-id="64443-109">Значение</span><span class="sxs-lookup"><span data-stu-id="64443-109">Value</span></span>|<span data-ttu-id="64443-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64443-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64443-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="64443-111">notConfigured</span></span>|<span data-ttu-id="64443-112">нуль</span><span class="sxs-lookup"><span data-stu-id="64443-112">0</span></span>|<span data-ttu-id="64443-113">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="64443-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="64443-114">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="64443-114">enableWithUEFILock</span></span>|<span data-ttu-id="64443-115">1,1</span><span class="sxs-lookup"><span data-stu-id="64443-115">1</span></span>|<span data-ttu-id="64443-116">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="64443-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="64443-117">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="64443-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="64443-118">2</span><span class="sxs-lookup"><span data-stu-id="64443-118">2</span></span>|<span data-ttu-id="64443-119">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="64443-119">Turns on Credential Guard without UEFI lock.</span></span>|



