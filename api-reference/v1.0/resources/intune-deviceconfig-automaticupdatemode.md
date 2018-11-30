---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024853"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c11f8-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="c11f8-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="c11f8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c11f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c11f8-105">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="c11f8-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="c11f8-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c11f8-106">Members</span></span>
|<span data-ttu-id="c11f8-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c11f8-107">Member</span></span>|<span data-ttu-id="c11f8-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c11f8-108">Value</span></span>|<span data-ttu-id="c11f8-109">Description</span><span class="sxs-lookup"><span data-stu-id="c11f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c11f8-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="c11f8-110">userDefined</span></span>|<span data-ttu-id="c11f8-111">0</span><span class="sxs-lookup"><span data-stu-id="c11f8-111">0</span></span>|<span data-ttu-id="c11f8-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="c11f8-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c11f8-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="c11f8-113">notifyDownload</span></span>|<span data-ttu-id="c11f8-114">1</span><span class="sxs-lookup"><span data-stu-id="c11f8-114">1</span></span>|<span data-ttu-id="c11f8-115">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="c11f8-115">Notify on download.</span></span>|
|<span data-ttu-id="c11f8-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c11f8-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c11f8-117">2</span><span class="sxs-lookup"><span data-stu-id="c11f8-117">2</span></span>|<span data-ttu-id="c11f8-118">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="c11f8-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c11f8-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c11f8-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c11f8-120">3</span><span class="sxs-lookup"><span data-stu-id="c11f8-120">3</span></span>|<span data-ttu-id="c11f8-121">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="c11f8-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c11f8-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c11f8-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c11f8-123">4</span><span class="sxs-lookup"><span data-stu-id="c11f8-123">4</span></span>|<span data-ttu-id="c11f8-124">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="c11f8-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c11f8-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c11f8-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c11f8-126">5</span><span class="sxs-lookup"><span data-stu-id="c11f8-126">5</span></span>|<span data-ttu-id="c11f8-127">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="c11f8-127">Auto-install and restart without end-user control</span></span>|



