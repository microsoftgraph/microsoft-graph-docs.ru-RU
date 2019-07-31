---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f394b02eac7e54c7e74a1c6954d6e3a7414e1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999187"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="ea9f3-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="ea9f3-103">enrollmentState enum type</span></span>

> <span data-ttu-id="ea9f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea9f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea9f3-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="ea9f3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ea9f3-107">Members</span></span>
|<span data-ttu-id="ea9f3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ea9f3-108">Member</span></span>|<span data-ttu-id="ea9f3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ea9f3-109">Value</span></span>|<span data-ttu-id="ea9f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ea9f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea9f3-111">unknown</span><span class="sxs-lookup"><span data-stu-id="ea9f3-111">unknown</span></span>|<span data-ttu-id="ea9f3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ea9f3-112">0</span></span>|<span data-ttu-id="ea9f3-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="ea9f3-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="ea9f3-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="ea9f3-114">enrolled</span></span>|<span data-ttu-id="ea9f3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ea9f3-115">1</span></span>|<span data-ttu-id="ea9f3-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="ea9f3-117">Пендингресет</span><span class="sxs-lookup"><span data-stu-id="ea9f3-117">pendingReset</span></span>|<span data-ttu-id="ea9f3-118">2</span><span class="sxs-lookup"><span data-stu-id="ea9f3-118">2</span></span>|<span data-ttu-id="ea9f3-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="ea9f3-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="ea9f3-120">failed</span></span>|<span data-ttu-id="ea9f3-121">4</span><span class="sxs-lookup"><span data-stu-id="ea9f3-121">3</span></span>|<span data-ttu-id="ea9f3-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="ea9f3-123">Нотконтактед</span><span class="sxs-lookup"><span data-stu-id="ea9f3-123">notContacted</span></span>|<span data-ttu-id="ea9f3-124">SP4</span><span class="sxs-lookup"><span data-stu-id="ea9f3-124">4</span></span>|<span data-ttu-id="ea9f3-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="ea9f3-126">заблокированных</span><span class="sxs-lookup"><span data-stu-id="ea9f3-126">blocked</span></span>|<span data-ttu-id="ea9f3-127">17:00</span><span class="sxs-lookup"><span data-stu-id="ea9f3-127">5</span></span>|<span data-ttu-id="ea9f3-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="ea9f3-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





