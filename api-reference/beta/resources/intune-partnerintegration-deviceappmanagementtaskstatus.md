---
title: тип перечисления Девицеаппманажементтаскстатус
description: Состояние задачи управления приложениями для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6fe8bd73920b1c4a71fb1bd98f28342ddeccde8b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301160"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="0db25-103">тип перечисления Девицеаппманажементтаскстатус</span><span class="sxs-lookup"><span data-stu-id="0db25-103">deviceAppManagementTaskStatus enum type</span></span>

<span data-ttu-id="0db25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0db25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0db25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db25-107">Состояние задачи управления приложениями для устройств.</span><span class="sxs-lookup"><span data-stu-id="0db25-107">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="0db25-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0db25-108">Members</span></span>
|<span data-ttu-id="0db25-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0db25-109">Member</span></span>|<span data-ttu-id="0db25-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0db25-110">Value</span></span>|<span data-ttu-id="0db25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0db25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db25-112">unknown</span><span class="sxs-lookup"><span data-stu-id="0db25-112">unknown</span></span>|<span data-ttu-id="0db25-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0db25-113">0</span></span>|<span data-ttu-id="0db25-114">Состояние не определено.</span><span class="sxs-lookup"><span data-stu-id="0db25-114">State is undefined.</span></span>|
|<span data-ttu-id="0db25-115">закончен</span><span class="sxs-lookup"><span data-stu-id="0db25-115">pending</span></span>|<span data-ttu-id="0db25-116">1,1</span><span class="sxs-lookup"><span data-stu-id="0db25-116">1</span></span>|<span data-ttu-id="0db25-117">Задача готова к просмотру.</span><span class="sxs-lookup"><span data-stu-id="0db25-117">The task is ready for review.</span></span>|
|<span data-ttu-id="0db25-118">ASP</span><span class="sxs-lookup"><span data-stu-id="0db25-118">active</span></span>|<span data-ttu-id="0db25-119">2</span><span class="sxs-lookup"><span data-stu-id="0db25-119">2</span></span>|<span data-ttu-id="0db25-120">Задача принята и работает над.</span><span class="sxs-lookup"><span data-stu-id="0db25-120">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="0db25-121">готовы</span><span class="sxs-lookup"><span data-stu-id="0db25-121">completed</span></span>|<span data-ttu-id="0db25-122">4</span><span class="sxs-lookup"><span data-stu-id="0db25-122">3</span></span>|<span data-ttu-id="0db25-123">Трудозатраты завершены.</span><span class="sxs-lookup"><span data-stu-id="0db25-123">The work is complete.</span></span>|
|<span data-ttu-id="0db25-124">клоняет</span><span class="sxs-lookup"><span data-stu-id="0db25-124">rejected</span></span>|<span data-ttu-id="0db25-125">4 </span><span class="sxs-lookup"><span data-stu-id="0db25-125">4</span></span>|<span data-ttu-id="0db25-126">Задача отклонена.</span><span class="sxs-lookup"><span data-stu-id="0db25-126">The task was rejected.</span></span>|




