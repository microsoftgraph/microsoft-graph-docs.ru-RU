---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d4c3fa42d20bcf0540c55975d24aad596c8aebf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407758"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="8e253-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="8e253-103">enrollmentState enum type</span></span>

<span data-ttu-id="8e253-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e253-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e253-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e253-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e253-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e253-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e253-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8e253-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="8e253-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8e253-108">Members</span></span>
|<span data-ttu-id="8e253-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8e253-109">Member</span></span>|<span data-ttu-id="8e253-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8e253-110">Value</span></span>|<span data-ttu-id="8e253-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e253-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e253-112">unknown</span><span class="sxs-lookup"><span data-stu-id="8e253-112">unknown</span></span>|<span data-ttu-id="8e253-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8e253-113">0</span></span>|<span data-ttu-id="8e253-114">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="8e253-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="8e253-115">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="8e253-115">enrolled</span></span>|<span data-ttu-id="8e253-116">1,1</span><span class="sxs-lookup"><span data-stu-id="8e253-116">1</span></span>|<span data-ttu-id="8e253-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="8e253-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="8e253-118">пендингресет</span><span class="sxs-lookup"><span data-stu-id="8e253-118">pendingReset</span></span>|<span data-ttu-id="8e253-119">2</span><span class="sxs-lookup"><span data-stu-id="8e253-119">2</span></span>|<span data-ttu-id="8e253-120">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="8e253-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="8e253-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="8e253-121">failed</span></span>|<span data-ttu-id="8e253-122">4</span><span class="sxs-lookup"><span data-stu-id="8e253-122">3</span></span>|<span data-ttu-id="8e253-123">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="8e253-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="8e253-124">нотконтактед</span><span class="sxs-lookup"><span data-stu-id="8e253-124">notContacted</span></span>|<span data-ttu-id="8e253-125">4 </span><span class="sxs-lookup"><span data-stu-id="8e253-125">4</span></span>|<span data-ttu-id="8e253-126">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="8e253-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="8e253-127">заблокированных</span><span class="sxs-lookup"><span data-stu-id="8e253-127">blocked</span></span>|<span data-ttu-id="8e253-128">5 </span><span class="sxs-lookup"><span data-stu-id="8e253-128">5</span></span>|<span data-ttu-id="8e253-129">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="8e253-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|



