---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 423d90521529193d2debf778f136a38fb8bbfefa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971062"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="26bc3-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="26bc3-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="26bc3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26bc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26bc3-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26bc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26bc3-107">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="26bc3-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="26bc3-108">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="26bc3-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="26bc3-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="26bc3-109">Members</span></span>
|<span data-ttu-id="26bc3-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="26bc3-110">Member</span></span>|<span data-ttu-id="26bc3-111">Значение</span><span class="sxs-lookup"><span data-stu-id="26bc3-111">Value</span></span>|<span data-ttu-id="26bc3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="26bc3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26bc3-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="26bc3-113">notConfigured</span></span>|<span data-ttu-id="26bc3-114">нуль</span><span class="sxs-lookup"><span data-stu-id="26bc3-114">0</span></span>|<span data-ttu-id="26bc3-115">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="26bc3-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="26bc3-116">Блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="26bc3-116">blockedWithUserOverride</span></span>|<span data-ttu-id="26bc3-117">1,1</span><span class="sxs-lookup"><span data-stu-id="26bc3-117">1</span></span>|<span data-ttu-id="26bc3-118">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="26bc3-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="26bc3-119">заблокированных</span><span class="sxs-lookup"><span data-stu-id="26bc3-119">blocked</span></span>|<span data-ttu-id="26bc3-120">2</span><span class="sxs-lookup"><span data-stu-id="26bc3-120">2</span></span>|<span data-ttu-id="26bc3-121">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="26bc3-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





