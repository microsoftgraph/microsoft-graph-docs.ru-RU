---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913270"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="9e28e-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="9e28e-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="9e28e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e28e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e28e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e28e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e28e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9e28e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e28e-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="9e28e-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="9e28e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9e28e-108">Members</span></span>
|<span data-ttu-id="9e28e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9e28e-109">Member</span></span>|<span data-ttu-id="9e28e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9e28e-110">Value</span></span>|<span data-ttu-id="9e28e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9e28e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e28e-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="9e28e-112">userDefined</span></span>|<span data-ttu-id="9e28e-113">0</span><span class="sxs-lookup"><span data-stu-id="9e28e-113">0</span></span>|<span data-ttu-id="9e28e-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="9e28e-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9e28e-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="9e28e-115">notifyDownload</span></span>|<span data-ttu-id="9e28e-116">1</span><span class="sxs-lookup"><span data-stu-id="9e28e-116">1</span></span>|<span data-ttu-id="9e28e-117">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="9e28e-117">Notify on download.</span></span>|
|<span data-ttu-id="9e28e-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="9e28e-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="9e28e-119">2</span><span class="sxs-lookup"><span data-stu-id="9e28e-119">2</span></span>|<span data-ttu-id="9e28e-120">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="9e28e-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="9e28e-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="9e28e-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="9e28e-122">3</span><span class="sxs-lookup"><span data-stu-id="9e28e-122">3</span></span>|<span data-ttu-id="9e28e-123">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="9e28e-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="9e28e-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="9e28e-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="9e28e-125">4</span><span class="sxs-lookup"><span data-stu-id="9e28e-125">4</span></span>|<span data-ttu-id="9e28e-126">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="9e28e-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="9e28e-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="9e28e-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="9e28e-128">5</span><span class="sxs-lookup"><span data-stu-id="9e28e-128">5</span></span>|<span data-ttu-id="9e28e-129">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="9e28e-129">Auto-install and restart without end-user control</span></span>|





