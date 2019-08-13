---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8d64f3af656a03bd02ecba5db2fbdab288f3693
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333886"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="49e17-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="49e17-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="49e17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49e17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49e17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49e17-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="49e17-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="49e17-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="49e17-107">Members</span></span>
|<span data-ttu-id="49e17-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="49e17-108">Member</span></span>|<span data-ttu-id="49e17-109">Значение</span><span class="sxs-lookup"><span data-stu-id="49e17-109">Value</span></span>|<span data-ttu-id="49e17-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49e17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e17-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="49e17-111">userDefined</span></span>|<span data-ttu-id="49e17-112">нуль</span><span class="sxs-lookup"><span data-stu-id="49e17-112">0</span></span>|<span data-ttu-id="49e17-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="49e17-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="49e17-114">нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="49e17-114">notifyDownload</span></span>|<span data-ttu-id="49e17-115">1,1</span><span class="sxs-lookup"><span data-stu-id="49e17-115">1</span></span>|<span data-ttu-id="49e17-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="49e17-116">Notify on download.</span></span>|
|<span data-ttu-id="49e17-117">аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="49e17-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="49e17-118">2</span><span class="sxs-lookup"><span data-stu-id="49e17-118">2</span></span>|<span data-ttu-id="49e17-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="49e17-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="49e17-120">аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="49e17-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="49e17-121">4</span><span class="sxs-lookup"><span data-stu-id="49e17-121">3</span></span>|<span data-ttu-id="49e17-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="49e17-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="49e17-123">аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="49e17-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="49e17-124">SP4</span><span class="sxs-lookup"><span data-stu-id="49e17-124">4</span></span>|<span data-ttu-id="49e17-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="49e17-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="49e17-126">аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="49e17-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="49e17-127">17:00</span><span class="sxs-lookup"><span data-stu-id="49e17-127">5</span></span>|<span data-ttu-id="49e17-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="49e17-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="49e17-129">виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="49e17-129">windowsDefault</span></span>|<span data-ttu-id="49e17-130">6 </span><span class="sxs-lookup"><span data-stu-id="49e17-130">6</span></span>|<span data-ttu-id="49e17-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="49e17-131">Reset to Windows default value.</span></span>|



