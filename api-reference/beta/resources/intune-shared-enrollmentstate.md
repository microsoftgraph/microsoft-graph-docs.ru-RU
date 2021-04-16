---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d208f8a4d1097d6698be3175a0b5ae86cf1918d4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866799"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="1c5f7-103">тип enum enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1c5f7-103">enrollmentState enum type</span></span>

<span data-ttu-id="1c5f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c5f7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c5f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c5f7-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="1c5f7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1c5f7-108">Members</span></span>
|<span data-ttu-id="1c5f7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1c5f7-109">Member</span></span>|<span data-ttu-id="1c5f7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1c5f7-110">Value</span></span>|<span data-ttu-id="1c5f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c5f7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1c5f7-112">unknown</span></span>|<span data-ttu-id="1c5f7-113">0</span><span class="sxs-lookup"><span data-stu-id="1c5f7-113">0</span></span>|<span data-ttu-id="1c5f7-114">Состояние регистрации устройства неизвестно</span><span class="sxs-lookup"><span data-stu-id="1c5f7-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="1c5f7-115">зарегистрированный</span><span class="sxs-lookup"><span data-stu-id="1c5f7-115">enrolled</span></span>|<span data-ttu-id="1c5f7-116">1</span><span class="sxs-lookup"><span data-stu-id="1c5f7-116">1</span></span>|<span data-ttu-id="1c5f7-117">Устройство зачислилось.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="1c5f7-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="1c5f7-118">pendingReset</span></span>|<span data-ttu-id="1c5f7-119">2</span><span class="sxs-lookup"><span data-stu-id="1c5f7-119">2</span></span>|<span data-ttu-id="1c5f7-120">Зарегистрирован, но он зарегистрирован через профиль регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="1c5f7-121">не удалось</span><span class="sxs-lookup"><span data-stu-id="1c5f7-121">failed</span></span>|<span data-ttu-id="1c5f7-122">3</span><span class="sxs-lookup"><span data-stu-id="1c5f7-122">3</span></span>|<span data-ttu-id="1c5f7-123">Не зарегистрирован, и есть запись сбоя регистрации.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="1c5f7-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="1c5f7-124">notContacted</span></span>|<span data-ttu-id="1c5f7-125">4 </span><span class="sxs-lookup"><span data-stu-id="1c5f7-125">4</span></span>|<span data-ttu-id="1c5f7-126">Устройство импортируется, но не регистрируется.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="1c5f7-127">заблокировано</span><span class="sxs-lookup"><span data-stu-id="1c5f7-127">blocked</span></span>|<span data-ttu-id="1c5f7-128">5 </span><span class="sxs-lookup"><span data-stu-id="1c5f7-128">5</span></span>|<span data-ttu-id="1c5f7-129">Устройство зарегистрировано как без пользователя, но не может двигаться к регистрации пользователей, так как приложение не удалось установить.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




