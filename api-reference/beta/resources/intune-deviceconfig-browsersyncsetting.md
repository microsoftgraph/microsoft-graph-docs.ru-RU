---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 74803f708fdf9f66c7b903c22cecf23cb06ae8dc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260504"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="b1170-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="b1170-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="b1170-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1170-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1170-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1170-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1170-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1170-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1170-108">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b1170-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b1170-109">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="b1170-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="b1170-110">Элементы</span><span class="sxs-lookup"><span data-stu-id="b1170-110">Members</span></span>
|<span data-ttu-id="b1170-111">Элемент</span><span class="sxs-lookup"><span data-stu-id="b1170-111">Member</span></span>|<span data-ttu-id="b1170-112">Значение</span><span class="sxs-lookup"><span data-stu-id="b1170-112">Value</span></span>|<span data-ttu-id="b1170-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b1170-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1170-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b1170-114">notConfigured</span></span>|<span data-ttu-id="b1170-115">нуль</span><span class="sxs-lookup"><span data-stu-id="b1170-115">0</span></span>|<span data-ttu-id="b1170-116">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="b1170-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="b1170-117">блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="b1170-117">blockedWithUserOverride</span></span>|<span data-ttu-id="b1170-118">1,1</span><span class="sxs-lookup"><span data-stu-id="b1170-118">1</span></span>|<span data-ttu-id="b1170-119">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="b1170-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="b1170-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="b1170-120">blocked</span></span>|<span data-ttu-id="b1170-121">2</span><span class="sxs-lookup"><span data-stu-id="b1170-121">2</span></span>|<span data-ttu-id="b1170-122">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="b1170-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




