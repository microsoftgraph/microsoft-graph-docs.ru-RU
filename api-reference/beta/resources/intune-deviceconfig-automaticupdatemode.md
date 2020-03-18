---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 845fdacfb0b29449e4464ec0eea03924632e861b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795907"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="7bd88-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="7bd88-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="7bd88-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bd88-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bd88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bd88-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="7bd88-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="7bd88-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7bd88-107">Members</span></span>
|<span data-ttu-id="7bd88-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7bd88-108">Member</span></span>|<span data-ttu-id="7bd88-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7bd88-109">Value</span></span>|<span data-ttu-id="7bd88-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd88-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="7bd88-111">userDefined</span></span>|<span data-ttu-id="7bd88-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7bd88-112">0</span></span>|<span data-ttu-id="7bd88-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="7bd88-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7bd88-114">нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="7bd88-114">notifyDownload</span></span>|<span data-ttu-id="7bd88-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7bd88-115">1</span></span>|<span data-ttu-id="7bd88-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="7bd88-116">Notify on download.</span></span>|
|<span data-ttu-id="7bd88-117">аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="7bd88-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="7bd88-118">2</span><span class="sxs-lookup"><span data-stu-id="7bd88-118">2</span></span>|<span data-ttu-id="7bd88-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="7bd88-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="7bd88-120">аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="7bd88-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="7bd88-121">4</span><span class="sxs-lookup"><span data-stu-id="7bd88-121">3</span></span>|<span data-ttu-id="7bd88-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="7bd88-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="7bd88-123">аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="7bd88-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="7bd88-124">4 </span><span class="sxs-lookup"><span data-stu-id="7bd88-124">4</span></span>|<span data-ttu-id="7bd88-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="7bd88-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="7bd88-126">аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="7bd88-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="7bd88-127">5 </span><span class="sxs-lookup"><span data-stu-id="7bd88-127">5</span></span>|<span data-ttu-id="7bd88-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="7bd88-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="7bd88-129">виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="7bd88-129">windowsDefault</span></span>|<span data-ttu-id="7bd88-130">6 </span><span class="sxs-lookup"><span data-stu-id="7bd88-130">6</span></span>|<span data-ttu-id="7bd88-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7bd88-131">Reset to Windows default value.</span></span>|



