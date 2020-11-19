---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b09e2db8d17777e3896714274ebe26662b288a40
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271872"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="854e7-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="854e7-103">enrollmentState enum type</span></span>

<span data-ttu-id="854e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="854e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="854e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="854e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="854e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="854e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="854e7-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="854e7-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="854e7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="854e7-108">Members</span></span>
|<span data-ttu-id="854e7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="854e7-109">Member</span></span>|<span data-ttu-id="854e7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="854e7-110">Value</span></span>|<span data-ttu-id="854e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="854e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854e7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="854e7-112">unknown</span></span>|<span data-ttu-id="854e7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="854e7-113">0</span></span>|<span data-ttu-id="854e7-114">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="854e7-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="854e7-115">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="854e7-115">enrolled</span></span>|<span data-ttu-id="854e7-116">1,1</span><span class="sxs-lookup"><span data-stu-id="854e7-116">1</span></span>|<span data-ttu-id="854e7-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="854e7-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="854e7-118">пендингресет</span><span class="sxs-lookup"><span data-stu-id="854e7-118">pendingReset</span></span>|<span data-ttu-id="854e7-119">2</span><span class="sxs-lookup"><span data-stu-id="854e7-119">2</span></span>|<span data-ttu-id="854e7-120">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="854e7-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="854e7-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="854e7-121">failed</span></span>|<span data-ttu-id="854e7-122">4</span><span class="sxs-lookup"><span data-stu-id="854e7-122">3</span></span>|<span data-ttu-id="854e7-123">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="854e7-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="854e7-124">нотконтактед</span><span class="sxs-lookup"><span data-stu-id="854e7-124">notContacted</span></span>|<span data-ttu-id="854e7-125">4 </span><span class="sxs-lookup"><span data-stu-id="854e7-125">4</span></span>|<span data-ttu-id="854e7-126">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="854e7-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="854e7-127">заблокированных</span><span class="sxs-lookup"><span data-stu-id="854e7-127">blocked</span></span>|<span data-ttu-id="854e7-128">5 </span><span class="sxs-lookup"><span data-stu-id="854e7-128">5</span></span>|<span data-ttu-id="854e7-129">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="854e7-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




