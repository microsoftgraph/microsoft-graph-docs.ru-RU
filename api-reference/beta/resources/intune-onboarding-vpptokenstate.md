---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b91090f64340e398bf9d48aff3741941fc0d778a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844837"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="1e0d8-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="1e0d8-103">vppTokenState enum type</span></span>

> <span data-ttu-id="1e0d8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e0d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e0d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e0d8-107">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="1e0d8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1e0d8-108">Members</span></span>
|<span data-ttu-id="1e0d8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1e0d8-109">Member</span></span>|<span data-ttu-id="1e0d8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1e0d8-110">Value</span></span>|<span data-ttu-id="1e0d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0d8-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1e0d8-112">unknown</span></span>|<span data-ttu-id="1e0d8-113">0</span><span class="sxs-lookup"><span data-stu-id="1e0d8-113">0</span></span>|<span data-ttu-id="1e0d8-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-114">Default state.</span></span>|
|<span data-ttu-id="1e0d8-115">допустимый</span><span class="sxs-lookup"><span data-stu-id="1e0d8-115">valid</span></span>|<span data-ttu-id="1e0d8-116">1</span><span class="sxs-lookup"><span data-stu-id="1e0d8-116">1</span></span>|<span data-ttu-id="1e0d8-117">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-117">Token is valid.</span></span>|
|<span data-ttu-id="1e0d8-118">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="1e0d8-118">expired</span></span>|<span data-ttu-id="1e0d8-119">2</span><span class="sxs-lookup"><span data-stu-id="1e0d8-119">2</span></span>|<span data-ttu-id="1e0d8-120">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-120">Token is expired.</span></span>|
|<span data-ttu-id="1e0d8-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="1e0d8-121">invalid</span></span>|<span data-ttu-id="1e0d8-122">3</span><span class="sxs-lookup"><span data-stu-id="1e0d8-122">3</span></span>|<span data-ttu-id="1e0d8-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-123">Token is invalid.</span></span>|
|<span data-ttu-id="1e0d8-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="1e0d8-124">assignedToExternalMDM</span></span>|<span data-ttu-id="1e0d8-125">4</span><span class="sxs-lookup"><span data-stu-id="1e0d8-125">4</span></span>|<span data-ttu-id="1e0d8-126">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="1e0d8-126">Token is managed by another MDM Service.</span></span>|





