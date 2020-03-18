---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4674f493bd5c6822e67c968568d547f89fa086c4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770279"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="4f563-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="4f563-103">enrollmentState enum type</span></span>

> <span data-ttu-id="4f563-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f563-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f563-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f563-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f563-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f563-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="4f563-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4f563-107">Members</span></span>
|<span data-ttu-id="4f563-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4f563-108">Member</span></span>|<span data-ttu-id="4f563-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4f563-109">Value</span></span>|<span data-ttu-id="4f563-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f563-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f563-111">unknown</span><span class="sxs-lookup"><span data-stu-id="4f563-111">unknown</span></span>|<span data-ttu-id="4f563-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4f563-112">0</span></span>|<span data-ttu-id="4f563-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4f563-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="4f563-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="4f563-114">enrolled</span></span>|<span data-ttu-id="4f563-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4f563-115">1</span></span>|<span data-ttu-id="4f563-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="4f563-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="4f563-117">пендингресет</span><span class="sxs-lookup"><span data-stu-id="4f563-117">pendingReset</span></span>|<span data-ttu-id="4f563-118">2</span><span class="sxs-lookup"><span data-stu-id="4f563-118">2</span></span>|<span data-ttu-id="4f563-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="4f563-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="4f563-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="4f563-120">failed</span></span>|<span data-ttu-id="4f563-121">4</span><span class="sxs-lookup"><span data-stu-id="4f563-121">3</span></span>|<span data-ttu-id="4f563-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="4f563-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="4f563-123">нотконтактед</span><span class="sxs-lookup"><span data-stu-id="4f563-123">notContacted</span></span>|<span data-ttu-id="4f563-124">4 </span><span class="sxs-lookup"><span data-stu-id="4f563-124">4</span></span>|<span data-ttu-id="4f563-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="4f563-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="4f563-126">заблокированных</span><span class="sxs-lookup"><span data-stu-id="4f563-126">blocked</span></span>|<span data-ttu-id="4f563-127">5 </span><span class="sxs-lookup"><span data-stu-id="4f563-127">5</span></span>|<span data-ttu-id="4f563-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="4f563-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|



