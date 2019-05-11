---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed54d34e2830e3477b7c80f3022fe5756e0b349f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940073"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="499d4-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="499d4-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="499d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="499d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="499d4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="499d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="499d4-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="499d4-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="499d4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="499d4-107">Members</span></span>
|<span data-ttu-id="499d4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="499d4-108">Member</span></span>|<span data-ttu-id="499d4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="499d4-109">Value</span></span>|<span data-ttu-id="499d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="499d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499d4-111">none</span><span class="sxs-lookup"><span data-stu-id="499d4-111">none</span></span>|<span data-ttu-id="499d4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="499d4-112">0</span></span>|<span data-ttu-id="499d4-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="499d4-113">Default status.</span></span>|
|<span data-ttu-id="499d4-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="499d4-114">inProgress</span></span>|<span data-ttu-id="499d4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="499d4-115">1</span></span>|<span data-ttu-id="499d4-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="499d4-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="499d4-117">готовы</span><span class="sxs-lookup"><span data-stu-id="499d4-117">completed</span></span>|<span data-ttu-id="499d4-118">2</span><span class="sxs-lookup"><span data-stu-id="499d4-118">2</span></span>|<span data-ttu-id="499d4-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="499d4-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="499d4-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="499d4-120">failed</span></span>|<span data-ttu-id="499d4-121">4</span><span class="sxs-lookup"><span data-stu-id="499d4-121">3</span></span>|<span data-ttu-id="499d4-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="499d4-122">Last Sync failed.</span></span>|




