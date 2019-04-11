---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791483"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="972b9-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="972b9-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="972b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="972b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="972b9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="972b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="972b9-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="972b9-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="972b9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="972b9-107">Members</span></span>
|<span data-ttu-id="972b9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="972b9-108">Member</span></span>|<span data-ttu-id="972b9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="972b9-109">Value</span></span>|<span data-ttu-id="972b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="972b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="972b9-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="972b9-111">userDefined</span></span>|<span data-ttu-id="972b9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="972b9-112">0</span></span>|<span data-ttu-id="972b9-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="972b9-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="972b9-114">Нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="972b9-114">notifyDownload</span></span>|<span data-ttu-id="972b9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="972b9-115">1</span></span>|<span data-ttu-id="972b9-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="972b9-116">Notify on download.</span></span>|
|<span data-ttu-id="972b9-117">Аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="972b9-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="972b9-118">2</span><span class="sxs-lookup"><span data-stu-id="972b9-118">2</span></span>|<span data-ttu-id="972b9-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="972b9-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="972b9-120">Аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="972b9-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="972b9-121">4</span><span class="sxs-lookup"><span data-stu-id="972b9-121">3</span></span>|<span data-ttu-id="972b9-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="972b9-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="972b9-123">Аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="972b9-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="972b9-124">SP4</span><span class="sxs-lookup"><span data-stu-id="972b9-124">4</span></span>|<span data-ttu-id="972b9-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="972b9-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="972b9-126">Аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="972b9-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="972b9-127">17:00</span><span class="sxs-lookup"><span data-stu-id="972b9-127">5</span></span>|<span data-ttu-id="972b9-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="972b9-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="972b9-129">Виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="972b9-129">windowsDefault</span></span>|<span data-ttu-id="972b9-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="972b9-130">6</span></span>|<span data-ttu-id="972b9-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="972b9-131">Reset to Windows default value.</span></span>|





