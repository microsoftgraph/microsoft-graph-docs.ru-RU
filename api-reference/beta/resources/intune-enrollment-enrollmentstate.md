---
title: Тип перечисления enrollmentState
description: Н/Д
ms.openlocfilehash: 8e8e20c0fd04e4da57eddfa7384052a6ab468152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080752"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="98a86-103">Тип перечисления enrollmentState</span><span class="sxs-lookup"><span data-stu-id="98a86-103">enrollmentState enum type</span></span>

> <span data-ttu-id="98a86-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98a86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98a86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98a86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98a86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98a86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98a86-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98a86-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="98a86-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="98a86-108">Members</span></span>
|<span data-ttu-id="98a86-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="98a86-109">Member</span></span>|<span data-ttu-id="98a86-110">Значение</span><span class="sxs-lookup"><span data-stu-id="98a86-110">Value</span></span>|<span data-ttu-id="98a86-111">Description</span><span class="sxs-lookup"><span data-stu-id="98a86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a86-112">unknown</span><span class="sxs-lookup"><span data-stu-id="98a86-112">unknown</span></span>|<span data-ttu-id="98a86-113">0</span><span class="sxs-lookup"><span data-stu-id="98a86-113">0</span></span>|<span data-ttu-id="98a86-114">Состояние регистрации устройства неизвестно</span><span class="sxs-lookup"><span data-stu-id="98a86-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="98a86-115">регистрации</span><span class="sxs-lookup"><span data-stu-id="98a86-115">enrolled</span></span>|<span data-ttu-id="98a86-116">1</span><span class="sxs-lookup"><span data-stu-id="98a86-116">1</span></span>|<span data-ttu-id="98a86-117">Регистрации устройство.</span><span class="sxs-lookup"><span data-stu-id="98a86-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="98a86-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="98a86-118">pendingReset</span></span>|<span data-ttu-id="98a86-119">2</span><span class="sxs-lookup"><span data-stu-id="98a86-119">2</span></span>|<span data-ttu-id="98a86-120">Участвуют, но зарегистрирован посредством профиля регистрации и зарегистрированных профилей отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="98a86-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="98a86-121">failed</span><span class="sxs-lookup"><span data-stu-id="98a86-121">failed</span></span>|<span data-ttu-id="98a86-122">3</span><span class="sxs-lookup"><span data-stu-id="98a86-122">3</span></span>|<span data-ttu-id="98a86-123">Не участвуют и запись сбоя регистрации.</span><span class="sxs-lookup"><span data-stu-id="98a86-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="98a86-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="98a86-124">notContacted</span></span>|<span data-ttu-id="98a86-125">4</span><span class="sxs-lookup"><span data-stu-id="98a86-125">4</span></span>|<span data-ttu-id="98a86-126">Устройство импортировать, но не участвуют.</span><span class="sxs-lookup"><span data-stu-id="98a86-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="98a86-127">заблокировано</span><span class="sxs-lookup"><span data-stu-id="98a86-127">blocked</span></span>|<span data-ttu-id="98a86-128">5</span><span class="sxs-lookup"><span data-stu-id="98a86-128">5</span></span>|<span data-ttu-id="98a86-129">Устройство участвуют как userless, но запретом переход к регистрации пользователя, так как не удается установить приложение.</span><span class="sxs-lookup"><span data-stu-id="98a86-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





