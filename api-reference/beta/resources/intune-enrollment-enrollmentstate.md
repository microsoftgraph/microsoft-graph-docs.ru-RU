---
title: тип перечисления Енроллментстате
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcb039563d9c45a33c4e42344fc8557dfe29b333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159250"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="c0047-103">тип перечисления Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="c0047-103">enrollmentState enum type</span></span>

> <span data-ttu-id="c0047-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0047-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0047-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0047-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0047-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0047-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="c0047-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c0047-107">Members</span></span>
|<span data-ttu-id="c0047-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c0047-108">Member</span></span>|<span data-ttu-id="c0047-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c0047-109">Value</span></span>|<span data-ttu-id="c0047-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0047-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0047-111">unknown</span><span class="sxs-lookup"><span data-stu-id="c0047-111">unknown</span></span>|<span data-ttu-id="c0047-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c0047-112">0</span></span>|<span data-ttu-id="c0047-113">Неизвестное состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="c0047-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="c0047-114">зарегистрированных</span><span class="sxs-lookup"><span data-stu-id="c0047-114">enrolled</span></span>|<span data-ttu-id="c0047-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c0047-115">1</span></span>|<span data-ttu-id="c0047-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c0047-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="c0047-117">Пендингресет</span><span class="sxs-lookup"><span data-stu-id="c0047-117">pendingReset</span></span>|<span data-ttu-id="c0047-118">2</span><span class="sxs-lookup"><span data-stu-id="c0047-118">2</span></span>|<span data-ttu-id="c0047-119">Зарегистрирована, но она зарегистрирована с помощью профиля регистрации, а зарегистрированный профиль отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="c0047-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="c0047-120">failed</span><span class="sxs-lookup"><span data-stu-id="c0047-120">failed</span></span>|<span data-ttu-id="c0047-121">4</span><span class="sxs-lookup"><span data-stu-id="c0047-121">3</span></span>|<span data-ttu-id="c0047-122">Не зарегистрирована и существует запись о сбое регистрации.</span><span class="sxs-lookup"><span data-stu-id="c0047-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="c0047-123">Нотконтактед</span><span class="sxs-lookup"><span data-stu-id="c0047-123">notContacted</span></span>|<span data-ttu-id="c0047-124">4</span><span class="sxs-lookup"><span data-stu-id="c0047-124">4</span></span>|<span data-ttu-id="c0047-125">Устройство импортировано, но не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c0047-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="c0047-126">заблокировано</span><span class="sxs-lookup"><span data-stu-id="c0047-126">blocked</span></span>|<span data-ttu-id="c0047-127">17:00</span><span class="sxs-lookup"><span data-stu-id="c0047-127">5</span></span>|<span data-ttu-id="c0047-128">Устройство зарегистрировано как без пользователя, но заблокировано для перемещения на регистрацию пользователей, так как не удалось установить приложение.</span><span class="sxs-lookup"><span data-stu-id="c0047-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




