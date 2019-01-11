---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07a6b410289ea6455d0f6756efa7d1ec4d735ce4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849989"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="50808-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="50808-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="50808-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50808-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50808-105">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="50808-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="50808-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="50808-106">Members</span></span>
|<span data-ttu-id="50808-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="50808-107">Member</span></span>|<span data-ttu-id="50808-108">Значение</span><span class="sxs-lookup"><span data-stu-id="50808-108">Value</span></span>|<span data-ttu-id="50808-109">Описание</span><span class="sxs-lookup"><span data-stu-id="50808-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50808-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="50808-110">userDefined</span></span>|<span data-ttu-id="50808-111">0</span><span class="sxs-lookup"><span data-stu-id="50808-111">0</span></span>|<span data-ttu-id="50808-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="50808-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="50808-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="50808-113">notifyDownload</span></span>|<span data-ttu-id="50808-114">1</span><span class="sxs-lookup"><span data-stu-id="50808-114">1</span></span>|<span data-ttu-id="50808-115">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="50808-115">Notify on download.</span></span>|
|<span data-ttu-id="50808-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="50808-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="50808-117">2</span><span class="sxs-lookup"><span data-stu-id="50808-117">2</span></span>|<span data-ttu-id="50808-118">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50808-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="50808-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="50808-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="50808-120">3</span><span class="sxs-lookup"><span data-stu-id="50808-120">3</span></span>|<span data-ttu-id="50808-121">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="50808-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="50808-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="50808-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="50808-123">4</span><span class="sxs-lookup"><span data-stu-id="50808-123">4</span></span>|<span data-ttu-id="50808-124">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="50808-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="50808-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="50808-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="50808-126">5</span><span class="sxs-lookup"><span data-stu-id="50808-126">5</span></span>|<span data-ttu-id="50808-127">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="50808-127">Auto-install and restart without end-user control</span></span>|



