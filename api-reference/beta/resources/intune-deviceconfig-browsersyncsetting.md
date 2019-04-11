---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f08031e970f56c071a4dd01af0542bd56924edd5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789747"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="d9ddb-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="d9ddb-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="d9ddb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9ddb-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ddb-107">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="d9ddb-108">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="d9ddb-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="d9ddb-109">Members</span></span>
|<span data-ttu-id="d9ddb-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="d9ddb-110">Member</span></span>|<span data-ttu-id="d9ddb-111">Значение</span><span class="sxs-lookup"><span data-stu-id="d9ddb-111">Value</span></span>|<span data-ttu-id="d9ddb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ddb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ddb-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d9ddb-113">notConfigured</span></span>|<span data-ttu-id="d9ddb-114">нуль</span><span class="sxs-lookup"><span data-stu-id="d9ddb-114">0</span></span>|<span data-ttu-id="d9ddb-115">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="d9ddb-116">Блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="d9ddb-116">blockedWithUserOverride</span></span>|<span data-ttu-id="d9ddb-117">1,1</span><span class="sxs-lookup"><span data-stu-id="d9ddb-117">1</span></span>|<span data-ttu-id="d9ddb-118">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="d9ddb-119">заблокированных</span><span class="sxs-lookup"><span data-stu-id="d9ddb-119">blocked</span></span>|<span data-ttu-id="d9ddb-120">2</span><span class="sxs-lookup"><span data-stu-id="d9ddb-120">2</span></span>|<span data-ttu-id="d9ddb-121">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="d9ddb-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





