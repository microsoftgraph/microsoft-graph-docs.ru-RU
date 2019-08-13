---
title: тип перечисления Бровсерсинксеттинг
description: Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge. Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5e8bb7c99f0bd4bf33474671ff6535be938be2fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333774"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="d344b-104">тип перечисления Бровсерсинксеттинг</span><span class="sxs-lookup"><span data-stu-id="d344b-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="d344b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d344b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d344b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d344b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d344b-107">Разрешить (не настраивать) или запретить (блокировать) синхронизацию параметров браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d344b-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="d344b-108">Параметр, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователей.</span><span class="sxs-lookup"><span data-stu-id="d344b-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="d344b-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="d344b-109">Members</span></span>
|<span data-ttu-id="d344b-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="d344b-110">Member</span></span>|<span data-ttu-id="d344b-111">Значение</span><span class="sxs-lookup"><span data-stu-id="d344b-111">Value</span></span>|<span data-ttu-id="d344b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d344b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d344b-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d344b-113">notConfigured</span></span>|<span data-ttu-id="d344b-114">нуль</span><span class="sxs-lookup"><span data-stu-id="d344b-114">0</span></span>|<span data-ttu-id="d344b-115">По умолчанию — разрешить синхронизацию параметров браузера на разных устройствах.</span><span class="sxs-lookup"><span data-stu-id="d344b-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="d344b-116">блоккедвисусероверриде</span><span class="sxs-lookup"><span data-stu-id="d344b-116">blockedWithUserOverride</span></span>|<span data-ttu-id="d344b-117">1,1</span><span class="sxs-lookup"><span data-stu-id="d344b-117">1</span></span>|<span data-ttu-id="d344b-118">Запретить синхронизацию параметров браузера на устройствах пользователя, разрешить переопределение параметров пользователем.</span><span class="sxs-lookup"><span data-stu-id="d344b-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="d344b-119">заблокированных</span><span class="sxs-lookup"><span data-stu-id="d344b-119">blocked</span></span>|<span data-ttu-id="d344b-120">2</span><span class="sxs-lookup"><span data-stu-id="d344b-120">2</span></span>|<span data-ttu-id="d344b-121">Абсолютно запретите синхронизацию параметров браузера для пользовательских устройств.</span><span class="sxs-lookup"><span data-stu-id="d344b-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|



