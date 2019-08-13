---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bb093e222dcdef3fff552416b2593f73a7c51e51
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327957"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e58fc-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="e58fc-103">enrollmentState enum type</span></span>

> <span data-ttu-id="e58fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e58fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e58fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e58fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e58fc-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e58fc-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e58fc-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e58fc-107">Members</span></span>
|<span data-ttu-id="e58fc-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e58fc-108">Member</span></span>|<span data-ttu-id="e58fc-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e58fc-109">Value</span></span>|<span data-ttu-id="e58fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e58fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e58fc-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e58fc-111">unknown</span></span>|<span data-ttu-id="e58fc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e58fc-112">0</span></span>|<span data-ttu-id="e58fc-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="e58fc-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e58fc-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="e58fc-114">enrolled</span></span>|<span data-ttu-id="e58fc-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e58fc-115">1</span></span>|<span data-ttu-id="e58fc-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="e58fc-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="e58fc-117">пендингресет</span><span class="sxs-lookup"><span data-stu-id="e58fc-117">pendingReset</span></span>|<span data-ttu-id="e58fc-118">2</span><span class="sxs-lookup"><span data-stu-id="e58fc-118">2</span></span>|<span data-ttu-id="e58fc-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="e58fc-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e58fc-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="e58fc-120">failed</span></span>|<span data-ttu-id="e58fc-121">4</span><span class="sxs-lookup"><span data-stu-id="e58fc-121">3</span></span>|<span data-ttu-id="e58fc-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="e58fc-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e58fc-123">нотконтактед</span><span class="sxs-lookup"><span data-stu-id="e58fc-123">notContacted</span></span>|<span data-ttu-id="e58fc-124">SP4</span><span class="sxs-lookup"><span data-stu-id="e58fc-124">4</span></span>|<span data-ttu-id="e58fc-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="e58fc-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="e58fc-126">заблокированных</span><span class="sxs-lookup"><span data-stu-id="e58fc-126">blocked</span></span>|<span data-ttu-id="e58fc-127">17:00</span><span class="sxs-lookup"><span data-stu-id="e58fc-127">5</span></span>|<span data-ttu-id="e58fc-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="e58fc-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|



