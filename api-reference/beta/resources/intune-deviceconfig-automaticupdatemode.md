---
title: тип перечисления свойства automaticupdatemode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bba7addc5ae3b7942c3e52e1d8989100e27b2831
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156786"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="ab1f4-103">тип перечисления свойства automaticupdatemode</span><span class="sxs-lookup"><span data-stu-id="ab1f4-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="ab1f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab1f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab1f4-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="ab1f4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ab1f4-107">Members</span></span>
|<span data-ttu-id="ab1f4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ab1f4-108">Member</span></span>|<span data-ttu-id="ab1f4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ab1f4-109">Value</span></span>|<span data-ttu-id="ab1f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab1f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab1f4-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ab1f4-111">userDefined</span></span>|<span data-ttu-id="ab1f4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ab1f4-112">0</span></span>|<span data-ttu-id="ab1f4-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ab1f4-114">Нотифидовнлоад</span><span class="sxs-lookup"><span data-stu-id="ab1f4-114">notifyDownload</span></span>|<span data-ttu-id="ab1f4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ab1f4-115">1</span></span>|<span data-ttu-id="ab1f4-116">Уведомлять при скачивании.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-116">Notify on download.</span></span>|
|<span data-ttu-id="ab1f4-117">Аутоинсталлатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="ab1f4-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="ab1f4-118">2</span><span class="sxs-lookup"><span data-stu-id="ab1f4-118">2</span></span>|<span data-ttu-id="ab1f4-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="ab1f4-120">Аутоинсталландребутатмаинтенанцетиме</span><span class="sxs-lookup"><span data-stu-id="ab1f4-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="ab1f4-121">4</span><span class="sxs-lookup"><span data-stu-id="ab1f4-121">3</span></span>|<span data-ttu-id="ab1f4-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="ab1f4-123">Аутоинсталландребутатсчедуледтиме</span><span class="sxs-lookup"><span data-stu-id="ab1f4-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="ab1f4-124">4</span><span class="sxs-lookup"><span data-stu-id="ab1f4-124">4</span></span>|<span data-ttu-id="ab1f4-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="ab1f4-126">Аутоинсталландребутвисаутендусерконтрол</span><span class="sxs-lookup"><span data-stu-id="ab1f4-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="ab1f4-127">17:00</span><span class="sxs-lookup"><span data-stu-id="ab1f4-127">5</span></span>|<span data-ttu-id="ab1f4-128">Автоматическая установка и перезапуск без управления конечными пользователями</span><span class="sxs-lookup"><span data-stu-id="ab1f4-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="ab1f4-129">Виндовсдефаулт</span><span class="sxs-lookup"><span data-stu-id="ab1f4-129">windowsDefault</span></span>|<span data-ttu-id="ab1f4-130">6</span><span class="sxs-lookup"><span data-stu-id="ab1f4-130">6</span></span>|<span data-ttu-id="ab1f4-131">Сбросьте значение параметра Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ab1f4-131">Reset to Windows default value.</span></span>|




