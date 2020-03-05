---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d44c4db05be66f568ba5c0b9182a6d2ab509088
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527067"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="ada26-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="ada26-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="ada26-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ada26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ada26-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ada26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ada26-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ada26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ada26-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="ada26-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="ada26-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ada26-108">Members</span></span>
|<span data-ttu-id="ada26-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ada26-109">Member</span></span>|<span data-ttu-id="ada26-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ada26-110">Value</span></span>|<span data-ttu-id="ada26-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ada26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada26-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ada26-112">userDefined</span></span>|<span data-ttu-id="ada26-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ada26-113">0</span></span>|<span data-ttu-id="ada26-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="ada26-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ada26-115">нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="ada26-115">notifyDownload</span></span>|<span data-ttu-id="ada26-116">1 </span><span class="sxs-lookup"><span data-stu-id="ada26-116">1</span></span>|<span data-ttu-id="ada26-117">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="ada26-117">Notify on download.</span></span>|
|<span data-ttu-id="ada26-118">аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="ada26-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="ada26-119">2 </span><span class="sxs-lookup"><span data-stu-id="ada26-119">2</span></span>|<span data-ttu-id="ada26-120">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ada26-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="ada26-121">аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="ada26-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="ada26-122">3 </span><span class="sxs-lookup"><span data-stu-id="ada26-122">3</span></span>|<span data-ttu-id="ada26-123">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ada26-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="ada26-124">аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="ada26-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="ada26-125">4 </span><span class="sxs-lookup"><span data-stu-id="ada26-125">4</span></span>|<span data-ttu-id="ada26-126">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="ada26-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="ada26-127">аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="ada26-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="ada26-128">5 </span><span class="sxs-lookup"><span data-stu-id="ada26-128">5</span></span>|<span data-ttu-id="ada26-129">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="ada26-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="ada26-130">виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="ada26-130">windowsDefault</span></span>|<span data-ttu-id="ada26-131">6 </span><span class="sxs-lookup"><span data-stu-id="ada26-131">6</span></span>|<span data-ttu-id="ada26-132">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ada26-132">Reset to Windows default value.</span></span>|



