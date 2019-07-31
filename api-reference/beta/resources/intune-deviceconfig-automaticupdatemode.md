---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d5df7cc791947e46b5da11c3162c0c5cf945bdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011472"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="346e1-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="346e1-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="346e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="346e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="346e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="346e1-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="346e1-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="346e1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="346e1-107">Members</span></span>
|<span data-ttu-id="346e1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="346e1-108">Member</span></span>|<span data-ttu-id="346e1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="346e1-109">Value</span></span>|<span data-ttu-id="346e1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="346e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346e1-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="346e1-111">userDefined</span></span>|<span data-ttu-id="346e1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="346e1-112">0</span></span>|<span data-ttu-id="346e1-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="346e1-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="346e1-114">Нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="346e1-114">notifyDownload</span></span>|<span data-ttu-id="346e1-115">1,1</span><span class="sxs-lookup"><span data-stu-id="346e1-115">1</span></span>|<span data-ttu-id="346e1-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="346e1-116">Notify on download.</span></span>|
|<span data-ttu-id="346e1-117">Аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="346e1-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="346e1-118">2</span><span class="sxs-lookup"><span data-stu-id="346e1-118">2</span></span>|<span data-ttu-id="346e1-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="346e1-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="346e1-120">Аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="346e1-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="346e1-121">4</span><span class="sxs-lookup"><span data-stu-id="346e1-121">3</span></span>|<span data-ttu-id="346e1-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="346e1-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="346e1-123">Аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="346e1-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="346e1-124">SP4</span><span class="sxs-lookup"><span data-stu-id="346e1-124">4</span></span>|<span data-ttu-id="346e1-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="346e1-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="346e1-126">Аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="346e1-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="346e1-127">17:00</span><span class="sxs-lookup"><span data-stu-id="346e1-127">5</span></span>|<span data-ttu-id="346e1-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="346e1-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="346e1-129">Виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="346e1-129">windowsDefault</span></span>|<span data-ttu-id="346e1-130">6 </span><span class="sxs-lookup"><span data-stu-id="346e1-130">6</span></span>|<span data-ttu-id="346e1-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="346e1-131">Reset to Windows default value.</span></span>|





