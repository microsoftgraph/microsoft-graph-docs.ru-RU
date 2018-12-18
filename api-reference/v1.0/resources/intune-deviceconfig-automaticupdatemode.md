---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346993"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="fb184-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="fb184-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="fb184-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb184-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb184-105">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="fb184-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="fb184-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="fb184-106">Members</span></span>
|<span data-ttu-id="fb184-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="fb184-107">Member</span></span>|<span data-ttu-id="fb184-108">Значение</span><span class="sxs-lookup"><span data-stu-id="fb184-108">Value</span></span>|<span data-ttu-id="fb184-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fb184-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb184-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="fb184-110">userDefined</span></span>|<span data-ttu-id="fb184-111">0</span><span class="sxs-lookup"><span data-stu-id="fb184-111">0</span></span>|<span data-ttu-id="fb184-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="fb184-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="fb184-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="fb184-113">notifyDownload</span></span>|<span data-ttu-id="fb184-114">1</span><span class="sxs-lookup"><span data-stu-id="fb184-114">1</span></span>|<span data-ttu-id="fb184-115">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="fb184-115">Notify on download.</span></span>|
|<span data-ttu-id="fb184-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="fb184-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="fb184-117">2</span><span class="sxs-lookup"><span data-stu-id="fb184-117">2</span></span>|<span data-ttu-id="fb184-118">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="fb184-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="fb184-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="fb184-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="fb184-120">3</span><span class="sxs-lookup"><span data-stu-id="fb184-120">3</span></span>|<span data-ttu-id="fb184-121">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="fb184-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="fb184-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="fb184-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="fb184-123">4</span><span class="sxs-lookup"><span data-stu-id="fb184-123">4</span></span>|<span data-ttu-id="fb184-124">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="fb184-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="fb184-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="fb184-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="fb184-126">5</span><span class="sxs-lookup"><span data-stu-id="fb184-126">5</span></span>|<span data-ttu-id="fb184-127">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="fb184-127">Auto-install and restart without end-user control</span></span>|



