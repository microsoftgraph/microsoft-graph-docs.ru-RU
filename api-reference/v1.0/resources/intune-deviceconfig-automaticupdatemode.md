---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987862"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="2e6a1-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2e6a1-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="2e6a1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e6a1-105">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="2e6a1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="2e6a1-106">Members</span></span>
|<span data-ttu-id="2e6a1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="2e6a1-107">Member</span></span>|<span data-ttu-id="2e6a1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="2e6a1-108">Value</span></span>|<span data-ttu-id="2e6a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e6a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e6a1-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="2e6a1-110">userDefined</span></span>|<span data-ttu-id="2e6a1-111">0</span><span class="sxs-lookup"><span data-stu-id="2e6a1-111">0</span></span>|<span data-ttu-id="2e6a1-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2e6a1-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="2e6a1-113">notifyDownload</span></span>|<span data-ttu-id="2e6a1-114">1</span><span class="sxs-lookup"><span data-stu-id="2e6a1-114">1</span></span>|<span data-ttu-id="2e6a1-115">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-115">Notify on download.</span></span>|
|<span data-ttu-id="2e6a1-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="2e6a1-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="2e6a1-117">2</span><span class="sxs-lookup"><span data-stu-id="2e6a1-117">2</span></span>|<span data-ttu-id="2e6a1-118">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="2e6a1-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="2e6a1-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="2e6a1-120">3</span><span class="sxs-lookup"><span data-stu-id="2e6a1-120">3</span></span>|<span data-ttu-id="2e6a1-121">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="2e6a1-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="2e6a1-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="2e6a1-123">4</span><span class="sxs-lookup"><span data-stu-id="2e6a1-123">4</span></span>|<span data-ttu-id="2e6a1-124">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="2e6a1-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="2e6a1-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="2e6a1-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="2e6a1-126">5</span><span class="sxs-lookup"><span data-stu-id="2e6a1-126">5</span></span>|<span data-ttu-id="2e6a1-127">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="2e6a1-127">Auto-install and restart without end-user control</span></span>|



