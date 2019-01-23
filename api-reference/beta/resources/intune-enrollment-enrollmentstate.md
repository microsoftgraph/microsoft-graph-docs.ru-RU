---
title: Тип перечисления enrollmentState
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419109"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="49642-103">Тип перечисления enrollmentState</span><span class="sxs-lookup"><span data-stu-id="49642-103">enrollmentState enum type</span></span>

> <span data-ttu-id="49642-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49642-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49642-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49642-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49642-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49642-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49642-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49642-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="49642-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="49642-108">Members</span></span>
|<span data-ttu-id="49642-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="49642-109">Member</span></span>|<span data-ttu-id="49642-110">Значение</span><span class="sxs-lookup"><span data-stu-id="49642-110">Value</span></span>|<span data-ttu-id="49642-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49642-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49642-112">unknown</span><span class="sxs-lookup"><span data-stu-id="49642-112">unknown</span></span>|<span data-ttu-id="49642-113">0</span><span class="sxs-lookup"><span data-stu-id="49642-113">0</span></span>|<span data-ttu-id="49642-114">Состояние регистрации устройства неизвестно</span><span class="sxs-lookup"><span data-stu-id="49642-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="49642-115">регистрации</span><span class="sxs-lookup"><span data-stu-id="49642-115">enrolled</span></span>|<span data-ttu-id="49642-116">1</span><span class="sxs-lookup"><span data-stu-id="49642-116">1</span></span>|<span data-ttu-id="49642-117">Регистрации устройство.</span><span class="sxs-lookup"><span data-stu-id="49642-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="49642-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="49642-118">pendingReset</span></span>|<span data-ttu-id="49642-119">2</span><span class="sxs-lookup"><span data-stu-id="49642-119">2</span></span>|<span data-ttu-id="49642-120">Участвуют, но зарегистрирован посредством профиля регистрации и зарегистрированных профилей отличается от назначенного профиля.</span><span class="sxs-lookup"><span data-stu-id="49642-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="49642-121">failed</span><span class="sxs-lookup"><span data-stu-id="49642-121">failed</span></span>|<span data-ttu-id="49642-122">3</span><span class="sxs-lookup"><span data-stu-id="49642-122">3</span></span>|<span data-ttu-id="49642-123">Не участвуют и запись сбоя регистрации.</span><span class="sxs-lookup"><span data-stu-id="49642-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="49642-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="49642-124">notContacted</span></span>|<span data-ttu-id="49642-125">4</span><span class="sxs-lookup"><span data-stu-id="49642-125">4</span></span>|<span data-ttu-id="49642-126">Устройство импортировать, но не участвуют.</span><span class="sxs-lookup"><span data-stu-id="49642-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="49642-127">заблокировано</span><span class="sxs-lookup"><span data-stu-id="49642-127">blocked</span></span>|<span data-ttu-id="49642-128">5</span><span class="sxs-lookup"><span data-stu-id="49642-128">5</span></span>|<span data-ttu-id="49642-129">Устройство участвуют как userless, но запретом переход к регистрации пользователя, так как не удается установить приложение.</span><span class="sxs-lookup"><span data-stu-id="49642-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




