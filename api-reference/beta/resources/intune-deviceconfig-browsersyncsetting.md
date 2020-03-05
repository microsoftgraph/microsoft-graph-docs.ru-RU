---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55b39f987cb3c2846ead0a1dc1c1f8e0c420399a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527006"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="a3fdf-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="a3fdf-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="a3fdf-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3fdf-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3fdf-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3fdf-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3fdf-108">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="a3fdf-109">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="a3fdf-110">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3fdf-110">Members</span></span>
|<span data-ttu-id="a3fdf-111">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3fdf-111">Member</span></span>|<span data-ttu-id="a3fdf-112">Значение</span><span class="sxs-lookup"><span data-stu-id="a3fdf-112">Value</span></span>|<span data-ttu-id="a3fdf-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a3fdf-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3fdf-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a3fdf-114">notConfigured</span></span>|<span data-ttu-id="a3fdf-115">нуль</span><span class="sxs-lookup"><span data-stu-id="a3fdf-115">0</span></span>|<span data-ttu-id="a3fdf-116">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="a3fdf-117">блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="a3fdf-117">blockedWithUserOverride</span></span>|<span data-ttu-id="a3fdf-118">1 </span><span class="sxs-lookup"><span data-stu-id="a3fdf-118">1</span></span>|<span data-ttu-id="a3fdf-119">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="a3fdf-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="a3fdf-120">blocked</span></span>|<span data-ttu-id="a3fdf-121">2 </span><span class="sxs-lookup"><span data-stu-id="a3fdf-121">2</span></span>|<span data-ttu-id="a3fdf-122">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="a3fdf-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|



