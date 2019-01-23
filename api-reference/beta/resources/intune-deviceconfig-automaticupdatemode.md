---
title: Тип перечисления automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402638"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c5c7c-103">Тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="c5c7c-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="c5c7c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5c7c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5c7c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c7c-107">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="c5c7c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5c7c-108">Members</span></span>
|<span data-ttu-id="c5c7c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5c7c-109">Member</span></span>|<span data-ttu-id="c5c7c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c5c7c-110">Value</span></span>|<span data-ttu-id="c5c7c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c7c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c7c-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="c5c7c-112">userDefined</span></span>|<span data-ttu-id="c5c7c-113">0</span><span class="sxs-lookup"><span data-stu-id="c5c7c-113">0</span></span>|<span data-ttu-id="c5c7c-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c5c7c-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="c5c7c-115">notifyDownload</span></span>|<span data-ttu-id="c5c7c-116">1</span><span class="sxs-lookup"><span data-stu-id="c5c7c-116">1</span></span>|<span data-ttu-id="c5c7c-117">Уведомите при загрузке.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-117">Notify on download.</span></span>|
|<span data-ttu-id="c5c7c-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c5c7c-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c5c7c-119">2</span><span class="sxs-lookup"><span data-stu-id="c5c7c-119">2</span></span>|<span data-ttu-id="c5c7c-120">Автоматическая установка с во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c5c7c-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c5c7c-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c5c7c-122">3</span><span class="sxs-lookup"><span data-stu-id="c5c7c-122">3</span></span>|<span data-ttu-id="c5c7c-123">Установить и перезагрузите во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c5c7c-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c5c7c-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c5c7c-125">4</span><span class="sxs-lookup"><span data-stu-id="c5c7c-125">4</span></span>|<span data-ttu-id="c5c7c-126">Установить и перезагрузите компьютер в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c5c7c-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c5c7c-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c5c7c-128">5</span><span class="sxs-lookup"><span data-stu-id="c5c7c-128">5</span></span>|<span data-ttu-id="c5c7c-129">Установить и перезапустите без управления конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="c5c7c-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="c5c7c-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="c5c7c-130">windowsDefault</span></span>|<span data-ttu-id="c5c7c-131">6</span><span class="sxs-lookup"><span data-stu-id="c5c7c-131">6</span></span>|<span data-ttu-id="c5c7c-132">Сброс Windows по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c5c7c-132">Reset to Windows default value.</span></span>|




