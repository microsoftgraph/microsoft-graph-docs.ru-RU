---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 53b0ccc5f4605d888a056c8093e7d286441bc244
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756539"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e622f-103">тип enum enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e622f-103">enrollmentState enum type</span></span>

<span data-ttu-id="e622f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e622f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e622f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e622f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e622f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e622f-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e622f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e622f-107">Members</span></span>
|<span data-ttu-id="e622f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e622f-108">Member</span></span>|<span data-ttu-id="e622f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e622f-109">Value</span></span>|<span data-ttu-id="e622f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e622f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e622f-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e622f-111">unknown</span></span>|<span data-ttu-id="e622f-112">0</span><span class="sxs-lookup"><span data-stu-id="e622f-112">0</span></span>|<span data-ttu-id="e622f-113">Состояние регистрации устройства неизвестно</span><span class="sxs-lookup"><span data-stu-id="e622f-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e622f-114">зарегистрированный</span><span class="sxs-lookup"><span data-stu-id="e622f-114">enrolled</span></span>|<span data-ttu-id="e622f-115">1</span><span class="sxs-lookup"><span data-stu-id="e622f-115">1</span></span>|<span data-ttu-id="e622f-116">Устройство зачислилось.</span><span class="sxs-lookup"><span data-stu-id="e622f-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="e622f-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="e622f-117">pendingReset</span></span>|<span data-ttu-id="e622f-118">2</span><span class="sxs-lookup"><span data-stu-id="e622f-118">2</span></span>|<span data-ttu-id="e622f-119">Зарегистрирован, но он зарегистрирован через профиль регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="e622f-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e622f-120">не удалось</span><span class="sxs-lookup"><span data-stu-id="e622f-120">failed</span></span>|<span data-ttu-id="e622f-121">3</span><span class="sxs-lookup"><span data-stu-id="e622f-121">3</span></span>|<span data-ttu-id="e622f-122">Не зарегистрирован, и есть запись сбоя регистрации.</span><span class="sxs-lookup"><span data-stu-id="e622f-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e622f-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="e622f-123">notContacted</span></span>|<span data-ttu-id="e622f-124">4 </span><span class="sxs-lookup"><span data-stu-id="e622f-124">4</span></span>|<span data-ttu-id="e622f-125">Устройство импортируется, но не регистрируется.</span><span class="sxs-lookup"><span data-stu-id="e622f-125">Device is imported but not enrolled.</span></span>|




