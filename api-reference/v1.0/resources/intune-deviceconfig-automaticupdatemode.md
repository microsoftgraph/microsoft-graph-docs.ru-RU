---
title: тип enum automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b4cd222db425a9a8a2647f2ffbeb6056dddbe1c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755905"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="5c6c6-103">тип enum automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5c6c6-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="5c6c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c6c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c6c6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c6c6-106">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="5c6c6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c6c6-107">Members</span></span>
|<span data-ttu-id="5c6c6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c6c6-108">Member</span></span>|<span data-ttu-id="5c6c6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5c6c6-109">Value</span></span>|<span data-ttu-id="5c6c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c6c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6c6-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="5c6c6-111">userDefined</span></span>|<span data-ttu-id="5c6c6-112">0</span><span class="sxs-lookup"><span data-stu-id="5c6c6-112">0</span></span>|<span data-ttu-id="5c6c6-113">Значение User Defined, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5c6c6-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="5c6c6-114">notifyDownload</span></span>|<span data-ttu-id="5c6c6-115">1</span><span class="sxs-lookup"><span data-stu-id="5c6c6-115">1</span></span>|<span data-ttu-id="5c6c6-116">Уведомление о загрузке.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-116">Notify on download.</span></span>|
|<span data-ttu-id="5c6c6-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5c6c6-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="5c6c6-118">2</span><span class="sxs-lookup"><span data-stu-id="5c6c6-118">2</span></span>|<span data-ttu-id="5c6c6-119">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="5c6c6-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5c6c6-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="5c6c6-121">3</span><span class="sxs-lookup"><span data-stu-id="5c6c6-121">3</span></span>|<span data-ttu-id="5c6c6-122">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="5c6c6-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="5c6c6-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="5c6c6-124">4 </span><span class="sxs-lookup"><span data-stu-id="5c6c6-124">4</span></span>|<span data-ttu-id="5c6c6-125">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="5c6c6-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="5c6c6-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="5c6c6-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="5c6c6-127">5 </span><span class="sxs-lookup"><span data-stu-id="5c6c6-127">5</span></span>|<span data-ttu-id="5c6c6-128">Автоматическая установка и перезапуск без управления конечным пользователем</span><span class="sxs-lookup"><span data-stu-id="5c6c6-128">Auto-install and restart without end-user control</span></span>|




