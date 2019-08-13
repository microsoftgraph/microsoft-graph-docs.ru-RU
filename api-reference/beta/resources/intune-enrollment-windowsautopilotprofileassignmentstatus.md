---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da068811f9a0a2d45ee2bc8f4bda2da088ed1065
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327698"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="451ec-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="451ec-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="451ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="451ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="451ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="451ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="451ec-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="451ec-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="451ec-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="451ec-107">Members</span></span>
|<span data-ttu-id="451ec-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="451ec-108">Member</span></span>|<span data-ttu-id="451ec-109">Значение</span><span class="sxs-lookup"><span data-stu-id="451ec-109">Value</span></span>|<span data-ttu-id="451ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="451ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="451ec-111">unknown</span><span class="sxs-lookup"><span data-stu-id="451ec-111">unknown</span></span>|<span data-ttu-id="451ec-112">нуль</span><span class="sxs-lookup"><span data-stu-id="451ec-112">0</span></span>|<span data-ttu-id="451ec-113">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="451ec-113">Unknown assignment status</span></span>|
|<span data-ttu-id="451ec-114">ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="451ec-114">assignedInSync</span></span>|<span data-ttu-id="451ec-115">1,1</span><span class="sxs-lookup"><span data-stu-id="451ec-115">1</span></span>|<span data-ttu-id="451ec-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="451ec-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="451ec-117">ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="451ec-117">assignedOutOfSync</span></span>|<span data-ttu-id="451ec-118">2</span><span class="sxs-lookup"><span data-stu-id="451ec-118">2</span></span>|<span data-ttu-id="451ec-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="451ec-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="451ec-120">ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="451ec-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="451ec-121">4</span><span class="sxs-lookup"><span data-stu-id="451ec-121">3</span></span>|<span data-ttu-id="451ec-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="451ec-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="451ec-123">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="451ec-123">notAssigned</span></span>|<span data-ttu-id="451ec-124">SP4</span><span class="sxs-lookup"><span data-stu-id="451ec-124">4</span></span>|<span data-ttu-id="451ec-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="451ec-125">Not assigned</span></span>|
|<span data-ttu-id="451ec-126">закончен</span><span class="sxs-lookup"><span data-stu-id="451ec-126">pending</span></span>|<span data-ttu-id="451ec-127">17:00</span><span class="sxs-lookup"><span data-stu-id="451ec-127">5</span></span>|<span data-ttu-id="451ec-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="451ec-128">Pending assignment</span></span>|
|<span data-ttu-id="451ec-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="451ec-129">failed</span></span>|<span data-ttu-id="451ec-130">6 </span><span class="sxs-lookup"><span data-stu-id="451ec-130">6</span></span>| <span data-ttu-id="451ec-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="451ec-131">Assignment failed</span></span>|



