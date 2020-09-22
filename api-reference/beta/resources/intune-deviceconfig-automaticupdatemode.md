---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90366deee96e898d8339d59cb1a49879ba019c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075905"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="a528b-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="a528b-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="a528b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a528b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a528b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a528b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a528b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a528b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a528b-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="a528b-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="a528b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a528b-108">Members</span></span>
|<span data-ttu-id="a528b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a528b-109">Member</span></span>|<span data-ttu-id="a528b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a528b-110">Value</span></span>|<span data-ttu-id="a528b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a528b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a528b-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="a528b-112">userDefined</span></span>|<span data-ttu-id="a528b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a528b-113">0</span></span>|<span data-ttu-id="a528b-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="a528b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a528b-115">нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="a528b-115">notifyDownload</span></span>|<span data-ttu-id="a528b-116">1 </span><span class="sxs-lookup"><span data-stu-id="a528b-116">1</span></span>|<span data-ttu-id="a528b-117">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="a528b-117">Notify on download.</span></span>|
|<span data-ttu-id="a528b-118">аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="a528b-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="a528b-119">2 </span><span class="sxs-lookup"><span data-stu-id="a528b-119">2</span></span>|<span data-ttu-id="a528b-120">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a528b-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="a528b-121">аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="a528b-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="a528b-122">4</span><span class="sxs-lookup"><span data-stu-id="a528b-122">3</span></span>|<span data-ttu-id="a528b-123">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a528b-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="a528b-124">аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="a528b-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="a528b-125">4 </span><span class="sxs-lookup"><span data-stu-id="a528b-125">4</span></span>|<span data-ttu-id="a528b-126">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="a528b-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="a528b-127">аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="a528b-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="a528b-128">5 </span><span class="sxs-lookup"><span data-stu-id="a528b-128">5</span></span>|<span data-ttu-id="a528b-129">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="a528b-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="a528b-130">виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="a528b-130">windowsDefault</span></span>|<span data-ttu-id="a528b-131">6 </span><span class="sxs-lookup"><span data-stu-id="a528b-131">6</span></span>|<span data-ttu-id="a528b-132">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a528b-132">Reset to Windows default value.</span></span>|






