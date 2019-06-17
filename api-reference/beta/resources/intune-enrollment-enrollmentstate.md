---
title: тип перечисления Енроллментстате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adb8c668bf3f6d30667417500a5989734167fb5c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992663"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="716ae-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="716ae-103">enrollmentState enum type</span></span>

> <span data-ttu-id="716ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="716ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="716ae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="716ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="716ae-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="716ae-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="716ae-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="716ae-107">Members</span></span>
|<span data-ttu-id="716ae-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="716ae-108">Member</span></span>|<span data-ttu-id="716ae-109">Значение</span><span class="sxs-lookup"><span data-stu-id="716ae-109">Value</span></span>|<span data-ttu-id="716ae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="716ae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="716ae-111">unknown</span><span class="sxs-lookup"><span data-stu-id="716ae-111">unknown</span></span>|<span data-ttu-id="716ae-112">нуль</span><span class="sxs-lookup"><span data-stu-id="716ae-112">0</span></span>|<span data-ttu-id="716ae-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="716ae-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="716ae-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="716ae-114">enrolled</span></span>|<span data-ttu-id="716ae-115">1,1</span><span class="sxs-lookup"><span data-stu-id="716ae-115">1</span></span>|<span data-ttu-id="716ae-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="716ae-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="716ae-117">Пендингресет</span><span class="sxs-lookup"><span data-stu-id="716ae-117">pendingReset</span></span>|<span data-ttu-id="716ae-118">2</span><span class="sxs-lookup"><span data-stu-id="716ae-118">2</span></span>|<span data-ttu-id="716ae-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="716ae-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="716ae-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="716ae-120">failed</span></span>|<span data-ttu-id="716ae-121">4</span><span class="sxs-lookup"><span data-stu-id="716ae-121">3</span></span>|<span data-ttu-id="716ae-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="716ae-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="716ae-123">Нотконтактед</span><span class="sxs-lookup"><span data-stu-id="716ae-123">notContacted</span></span>|<span data-ttu-id="716ae-124">SP4</span><span class="sxs-lookup"><span data-stu-id="716ae-124">4</span></span>|<span data-ttu-id="716ae-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="716ae-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="716ae-126">заблокированных</span><span class="sxs-lookup"><span data-stu-id="716ae-126">blocked</span></span>|<span data-ttu-id="716ae-127">17:00</span><span class="sxs-lookup"><span data-stu-id="716ae-127">5</span></span>|<span data-ttu-id="716ae-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="716ae-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





