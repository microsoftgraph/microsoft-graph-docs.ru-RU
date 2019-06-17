---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2fffa3e1b1a5e7efa43d7ce653792247e3ad790
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983633"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="3a59c-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="3a59c-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="3a59c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a59c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a59c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a59c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a59c-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="3a59c-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="3a59c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3a59c-107">Members</span></span>
|<span data-ttu-id="3a59c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3a59c-108">Member</span></span>|<span data-ttu-id="3a59c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3a59c-109">Value</span></span>|<span data-ttu-id="3a59c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3a59c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a59c-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="3a59c-111">userDefined</span></span>|<span data-ttu-id="3a59c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3a59c-112">0</span></span>|<span data-ttu-id="3a59c-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="3a59c-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3a59c-114">Нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="3a59c-114">notifyDownload</span></span>|<span data-ttu-id="3a59c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3a59c-115">1</span></span>|<span data-ttu-id="3a59c-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="3a59c-116">Notify on download.</span></span>|
|<span data-ttu-id="3a59c-117">Аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="3a59c-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="3a59c-118">2</span><span class="sxs-lookup"><span data-stu-id="3a59c-118">2</span></span>|<span data-ttu-id="3a59c-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3a59c-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="3a59c-120">Аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="3a59c-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="3a59c-121">4</span><span class="sxs-lookup"><span data-stu-id="3a59c-121">3</span></span>|<span data-ttu-id="3a59c-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3a59c-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="3a59c-123">Аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="3a59c-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="3a59c-124">SP4</span><span class="sxs-lookup"><span data-stu-id="3a59c-124">4</span></span>|<span data-ttu-id="3a59c-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="3a59c-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="3a59c-126">Аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="3a59c-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="3a59c-127">17:00</span><span class="sxs-lookup"><span data-stu-id="3a59c-127">5</span></span>|<span data-ttu-id="3a59c-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="3a59c-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="3a59c-129">Виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="3a59c-129">windowsDefault</span></span>|<span data-ttu-id="3a59c-130">6 </span><span class="sxs-lookup"><span data-stu-id="3a59c-130">6</span></span>|<span data-ttu-id="3a59c-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3a59c-131">Reset to Windows default value.</span></span>|





