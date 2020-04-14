---
title: тип перечисления Девицеаппманажементтаскстатус
description: Состояние задачи управления приложениями для устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7d3c27b874b97912daa249b365fd4015677cc746
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446668"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="70115-103">тип перечисления Девицеаппманажементтаскстатус</span><span class="sxs-lookup"><span data-stu-id="70115-103">deviceAppManagementTaskStatus enum type</span></span>

<span data-ttu-id="70115-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70115-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70115-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70115-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70115-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70115-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70115-107">Состояние задачи управления приложениями для устройств.</span><span class="sxs-lookup"><span data-stu-id="70115-107">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="70115-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="70115-108">Members</span></span>
|<span data-ttu-id="70115-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="70115-109">Member</span></span>|<span data-ttu-id="70115-110">Значение</span><span class="sxs-lookup"><span data-stu-id="70115-110">Value</span></span>|<span data-ttu-id="70115-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70115-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70115-112">unknown</span><span class="sxs-lookup"><span data-stu-id="70115-112">unknown</span></span>|<span data-ttu-id="70115-113">нуль</span><span class="sxs-lookup"><span data-stu-id="70115-113">0</span></span>|<span data-ttu-id="70115-114">Состояние не определено.</span><span class="sxs-lookup"><span data-stu-id="70115-114">State is undefined.</span></span>|
|<span data-ttu-id="70115-115">закончен</span><span class="sxs-lookup"><span data-stu-id="70115-115">pending</span></span>|<span data-ttu-id="70115-116">1,1</span><span class="sxs-lookup"><span data-stu-id="70115-116">1</span></span>|<span data-ttu-id="70115-117">Задача готова к просмотру.</span><span class="sxs-lookup"><span data-stu-id="70115-117">The task is ready for review.</span></span>|
|<span data-ttu-id="70115-118">ASP</span><span class="sxs-lookup"><span data-stu-id="70115-118">active</span></span>|<span data-ttu-id="70115-119">2</span><span class="sxs-lookup"><span data-stu-id="70115-119">2</span></span>|<span data-ttu-id="70115-120">Задача принята и работает над.</span><span class="sxs-lookup"><span data-stu-id="70115-120">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="70115-121">готовы</span><span class="sxs-lookup"><span data-stu-id="70115-121">completed</span></span>|<span data-ttu-id="70115-122">4</span><span class="sxs-lookup"><span data-stu-id="70115-122">3</span></span>|<span data-ttu-id="70115-123">Трудозатраты завершены.</span><span class="sxs-lookup"><span data-stu-id="70115-123">The work is complete.</span></span>|
|<span data-ttu-id="70115-124">клоняет</span><span class="sxs-lookup"><span data-stu-id="70115-124">rejected</span></span>|<span data-ttu-id="70115-125">4 </span><span class="sxs-lookup"><span data-stu-id="70115-125">4</span></span>|<span data-ttu-id="70115-126">Задача отклонена.</span><span class="sxs-lookup"><span data-stu-id="70115-126">The task was rejected.</span></span>|



