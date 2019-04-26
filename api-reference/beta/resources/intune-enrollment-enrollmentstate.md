---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4826ae7cc0bfc53338212d812c293e5577d0ae02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579193"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="db987-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="db987-103">enrollmentState enum type</span></span>

> <span data-ttu-id="db987-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db987-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db987-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db987-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db987-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="db987-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="db987-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="db987-107">Members</span></span>
|<span data-ttu-id="db987-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="db987-108">Member</span></span>|<span data-ttu-id="db987-109">Значение</span><span class="sxs-lookup"><span data-stu-id="db987-109">Value</span></span>|<span data-ttu-id="db987-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db987-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db987-111">unknown</span><span class="sxs-lookup"><span data-stu-id="db987-111">unknown</span></span>|<span data-ttu-id="db987-112">нуль</span><span class="sxs-lookup"><span data-stu-id="db987-112">0</span></span>|<span data-ttu-id="db987-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="db987-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="db987-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="db987-114">enrolled</span></span>|<span data-ttu-id="db987-115">1 </span><span class="sxs-lookup"><span data-stu-id="db987-115">1</span></span>|<span data-ttu-id="db987-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="db987-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="db987-117">Пендингресет</span><span class="sxs-lookup"><span data-stu-id="db987-117">pendingReset</span></span>|<span data-ttu-id="db987-118">2 </span><span class="sxs-lookup"><span data-stu-id="db987-118">2</span></span>|<span data-ttu-id="db987-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="db987-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="db987-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="db987-120">failed</span></span>|<span data-ttu-id="db987-121">3 </span><span class="sxs-lookup"><span data-stu-id="db987-121">3</span></span>|<span data-ttu-id="db987-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="db987-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="db987-123">Нотконтактед</span><span class="sxs-lookup"><span data-stu-id="db987-123">notContacted</span></span>|<span data-ttu-id="db987-124">4 </span><span class="sxs-lookup"><span data-stu-id="db987-124">4</span></span>|<span data-ttu-id="db987-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="db987-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="db987-126">заблокированных</span><span class="sxs-lookup"><span data-stu-id="db987-126">blocked</span></span>|<span data-ttu-id="db987-127">5 </span><span class="sxs-lookup"><span data-stu-id="db987-127">5</span></span>|<span data-ttu-id="db987-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="db987-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





