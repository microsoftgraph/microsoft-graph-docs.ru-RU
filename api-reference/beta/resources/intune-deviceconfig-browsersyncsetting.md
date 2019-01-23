---
title: Тип перечисления browserSyncSetting
description: Allow(NOT Configured) или prevent(Block) синхронизации параметров браузера Microsoft пограничного сервера. Вариант, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431680"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="95149-104">Тип перечисления browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="95149-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="95149-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="95149-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95149-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95149-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95149-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95149-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95149-108">Allow(NOT Configured) или prevent(Block) синхронизации параметров браузера Microsoft пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="95149-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="95149-109">Вариант, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователя.</span><span class="sxs-lookup"><span data-stu-id="95149-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="95149-110">Элементы</span><span class="sxs-lookup"><span data-stu-id="95149-110">Members</span></span>
|<span data-ttu-id="95149-111">Элемент</span><span class="sxs-lookup"><span data-stu-id="95149-111">Member</span></span>|<span data-ttu-id="95149-112">Значение</span><span class="sxs-lookup"><span data-stu-id="95149-112">Value</span></span>|<span data-ttu-id="95149-113">Описание</span><span class="sxs-lookup"><span data-stu-id="95149-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95149-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="95149-114">notConfigured</span></span>|<span data-ttu-id="95149-115">0</span><span class="sxs-lookup"><span data-stu-id="95149-115">0</span></span>|<span data-ttu-id="95149-116">Значение по умолчанию — разрешить синхронизацию параметров браузера на устройствах.</span><span class="sxs-lookup"><span data-stu-id="95149-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="95149-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="95149-117">blockedWithUserOverride</span></span>|<span data-ttu-id="95149-118">1</span><span class="sxs-lookup"><span data-stu-id="95149-118">1</span></span>|<span data-ttu-id="95149-119">Запретить синхронизацию параметров браузера на устройствах пользователей, разрешить переопределение параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="95149-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="95149-120">заблокировано</span><span class="sxs-lookup"><span data-stu-id="95149-120">blocked</span></span>|<span data-ttu-id="95149-121">2</span><span class="sxs-lookup"><span data-stu-id="95149-121">2</span></span>|<span data-ttu-id="95149-122">Абсолютно запретить синхронизацию параметров браузера на устройствах пользователей.</span><span class="sxs-lookup"><span data-stu-id="95149-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




