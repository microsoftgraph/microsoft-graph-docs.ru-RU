---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8e2148cccbb891b1c139abd9d15ba424b3b3e9b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967380"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="3625f-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="3625f-103">vppTokenState enum type</span></span>

> <span data-ttu-id="3625f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3625f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3625f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3625f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3625f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3625f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3625f-107">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="3625f-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="3625f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3625f-108">Members</span></span>
|<span data-ttu-id="3625f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3625f-109">Member</span></span>|<span data-ttu-id="3625f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3625f-110">Value</span></span>|<span data-ttu-id="3625f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3625f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3625f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3625f-112">unknown</span></span>|<span data-ttu-id="3625f-113">0</span><span class="sxs-lookup"><span data-stu-id="3625f-113">0</span></span>|<span data-ttu-id="3625f-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3625f-114">Default state.</span></span>|
|<span data-ttu-id="3625f-115">допустимый</span><span class="sxs-lookup"><span data-stu-id="3625f-115">valid</span></span>|<span data-ttu-id="3625f-116">1</span><span class="sxs-lookup"><span data-stu-id="3625f-116">1</span></span>|<span data-ttu-id="3625f-117">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="3625f-117">Token is valid.</span></span>|
|<span data-ttu-id="3625f-118">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="3625f-118">expired</span></span>|<span data-ttu-id="3625f-119">2</span><span class="sxs-lookup"><span data-stu-id="3625f-119">2</span></span>|<span data-ttu-id="3625f-120">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="3625f-120">Token is expired.</span></span>|
|<span data-ttu-id="3625f-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="3625f-121">invalid</span></span>|<span data-ttu-id="3625f-122">3</span><span class="sxs-lookup"><span data-stu-id="3625f-122">3</span></span>|<span data-ttu-id="3625f-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="3625f-123">Token is invalid.</span></span>|
|<span data-ttu-id="3625f-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="3625f-124">assignedToExternalMDM</span></span>|<span data-ttu-id="3625f-125">4</span><span class="sxs-lookup"><span data-stu-id="3625f-125">4</span></span>|<span data-ttu-id="3625f-126">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="3625f-126">Token is managed by another MDM Service.</span></span>|





