---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080587"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="13569-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="13569-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="13569-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13569-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13569-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13569-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13569-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="13569-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13569-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="13569-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="13569-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="13569-108">Members</span></span>
|<span data-ttu-id="13569-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="13569-109">Member</span></span>|<span data-ttu-id="13569-110">Значение</span><span class="sxs-lookup"><span data-stu-id="13569-110">Value</span></span>|<span data-ttu-id="13569-111">Description</span><span class="sxs-lookup"><span data-stu-id="13569-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13569-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="13569-112">userDefined</span></span>|<span data-ttu-id="13569-113">0</span><span class="sxs-lookup"><span data-stu-id="13569-113">0</span></span>|<span data-ttu-id="13569-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="13569-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="13569-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="13569-115">notifyDownload</span></span>|<span data-ttu-id="13569-116">1</span><span class="sxs-lookup"><span data-stu-id="13569-116">1</span></span>|<span data-ttu-id="13569-117">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="13569-117">Notify on download.</span></span>|
|<span data-ttu-id="13569-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="13569-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="13569-119">2</span><span class="sxs-lookup"><span data-stu-id="13569-119">2</span></span>|<span data-ttu-id="13569-120">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="13569-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="13569-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="13569-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="13569-122">3</span><span class="sxs-lookup"><span data-stu-id="13569-122">3</span></span>|<span data-ttu-id="13569-123">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="13569-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="13569-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="13569-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="13569-125">4</span><span class="sxs-lookup"><span data-stu-id="13569-125">4</span></span>|<span data-ttu-id="13569-126">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="13569-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="13569-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="13569-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="13569-128">5</span><span class="sxs-lookup"><span data-stu-id="13569-128">5</span></span>|<span data-ttu-id="13569-129">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="13569-129">Auto-install and restart without end-user control</span></span>|





