---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89d28a07bb2c6abea2e2a10d9b5a0961e5efecff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834029"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="331dd-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="331dd-103">vppTokenState enum type</span></span>

> <span data-ttu-id="331dd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="331dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="331dd-105">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="331dd-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="331dd-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="331dd-106">Members</span></span>
|<span data-ttu-id="331dd-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="331dd-107">Member</span></span>|<span data-ttu-id="331dd-108">Значение</span><span class="sxs-lookup"><span data-stu-id="331dd-108">Value</span></span>|<span data-ttu-id="331dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="331dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="331dd-110">unknown</span><span class="sxs-lookup"><span data-stu-id="331dd-110">unknown</span></span>|<span data-ttu-id="331dd-111">0</span><span class="sxs-lookup"><span data-stu-id="331dd-111">0</span></span>|<span data-ttu-id="331dd-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="331dd-112">Default state.</span></span>|
|<span data-ttu-id="331dd-113">допустимый</span><span class="sxs-lookup"><span data-stu-id="331dd-113">valid</span></span>|<span data-ttu-id="331dd-114">1</span><span class="sxs-lookup"><span data-stu-id="331dd-114">1</span></span>|<span data-ttu-id="331dd-115">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="331dd-115">Token is valid.</span></span>|
|<span data-ttu-id="331dd-116">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="331dd-116">expired</span></span>|<span data-ttu-id="331dd-117">2</span><span class="sxs-lookup"><span data-stu-id="331dd-117">2</span></span>|<span data-ttu-id="331dd-118">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="331dd-118">Token is expired.</span></span>|
|<span data-ttu-id="331dd-119">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="331dd-119">invalid</span></span>|<span data-ttu-id="331dd-120">3</span><span class="sxs-lookup"><span data-stu-id="331dd-120">3</span></span>|<span data-ttu-id="331dd-121">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="331dd-121">Token is invalid.</span></span>|
|<span data-ttu-id="331dd-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="331dd-122">assignedToExternalMDM</span></span>|<span data-ttu-id="331dd-123">4</span><span class="sxs-lookup"><span data-stu-id="331dd-123">4</span></span>|<span data-ttu-id="331dd-124">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="331dd-124">Token is managed by another MDM Service.</span></span>|



