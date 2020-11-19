---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a1ea942a2418f763a6914329dabe26cd0ace1e8a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260765"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="2d5ea-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="2d5ea-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="2d5ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d5ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d5ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d5ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d5ea-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="2d5ea-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d5ea-108">Members</span></span>
|<span data-ttu-id="2d5ea-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d5ea-109">Member</span></span>|<span data-ttu-id="2d5ea-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2d5ea-110">Value</span></span>|<span data-ttu-id="2d5ea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d5ea-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="2d5ea-112">userDefined</span></span>|<span data-ttu-id="2d5ea-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2d5ea-113">0</span></span>|<span data-ttu-id="2d5ea-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2d5ea-115">нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="2d5ea-115">notifyDownload</span></span>|<span data-ttu-id="2d5ea-116">1,1</span><span class="sxs-lookup"><span data-stu-id="2d5ea-116">1</span></span>|<span data-ttu-id="2d5ea-117">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-117">Notify on download.</span></span>|
|<span data-ttu-id="2d5ea-118">аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="2d5ea-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="2d5ea-119">2</span><span class="sxs-lookup"><span data-stu-id="2d5ea-119">2</span></span>|<span data-ttu-id="2d5ea-120">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="2d5ea-121">аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="2d5ea-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="2d5ea-122">4</span><span class="sxs-lookup"><span data-stu-id="2d5ea-122">3</span></span>|<span data-ttu-id="2d5ea-123">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="2d5ea-124">аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="2d5ea-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="2d5ea-125">4 </span><span class="sxs-lookup"><span data-stu-id="2d5ea-125">4</span></span>|<span data-ttu-id="2d5ea-126">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="2d5ea-127">аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="2d5ea-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="2d5ea-128">5 </span><span class="sxs-lookup"><span data-stu-id="2d5ea-128">5</span></span>|<span data-ttu-id="2d5ea-129">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="2d5ea-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="2d5ea-130">виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="2d5ea-130">windowsDefault</span></span>|<span data-ttu-id="2d5ea-131">6 </span><span class="sxs-lookup"><span data-stu-id="2d5ea-131">6</span></span>|<span data-ttu-id="2d5ea-132">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2d5ea-132">Reset to Windows default value.</span></span>|




