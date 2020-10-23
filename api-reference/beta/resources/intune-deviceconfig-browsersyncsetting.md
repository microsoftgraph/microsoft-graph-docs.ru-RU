---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3bc330373c3578a1bbcf2e6736469c18c926a904
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729828"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="00654-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="00654-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="00654-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00654-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00654-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00654-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00654-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00654-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00654-108">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="00654-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="00654-109">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="00654-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="00654-110">Элементы</span><span class="sxs-lookup"><span data-stu-id="00654-110">Members</span></span>
|<span data-ttu-id="00654-111">Элемент</span><span class="sxs-lookup"><span data-stu-id="00654-111">Member</span></span>|<span data-ttu-id="00654-112">Значение</span><span class="sxs-lookup"><span data-stu-id="00654-112">Value</span></span>|<span data-ttu-id="00654-113">Описание</span><span class="sxs-lookup"><span data-stu-id="00654-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00654-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="00654-114">notConfigured</span></span>|<span data-ttu-id="00654-115">нуль</span><span class="sxs-lookup"><span data-stu-id="00654-115">0</span></span>|<span data-ttu-id="00654-116">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="00654-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="00654-117">блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="00654-117">blockedWithUserOverride</span></span>|<span data-ttu-id="00654-118">1,1</span><span class="sxs-lookup"><span data-stu-id="00654-118">1</span></span>|<span data-ttu-id="00654-119">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="00654-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="00654-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="00654-120">blocked</span></span>|<span data-ttu-id="00654-121">2</span><span class="sxs-lookup"><span data-stu-id="00654-121">2</span></span>|<span data-ttu-id="00654-122">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="00654-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|





