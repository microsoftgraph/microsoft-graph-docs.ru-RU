---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
ms.openlocfilehash: 7180364063a48e1b0eeb2778ed4def7c0d3930a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078047"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="f1744-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="f1744-103">vppTokenState enum type</span></span>

> <span data-ttu-id="f1744-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1744-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1744-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1744-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1744-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1744-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1744-107">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="f1744-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="f1744-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f1744-108">Members</span></span>
|<span data-ttu-id="f1744-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1744-109">Member</span></span>|<span data-ttu-id="f1744-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f1744-110">Value</span></span>|<span data-ttu-id="f1744-111">Description</span><span class="sxs-lookup"><span data-stu-id="f1744-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1744-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f1744-112">unknown</span></span>|<span data-ttu-id="f1744-113">0</span><span class="sxs-lookup"><span data-stu-id="f1744-113">0</span></span>|<span data-ttu-id="f1744-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f1744-114">Default state.</span></span>|
|<span data-ttu-id="f1744-115">допустимый</span><span class="sxs-lookup"><span data-stu-id="f1744-115">valid</span></span>|<span data-ttu-id="f1744-116">1</span><span class="sxs-lookup"><span data-stu-id="f1744-116">1</span></span>|<span data-ttu-id="f1744-117">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="f1744-117">Token is valid.</span></span>|
|<span data-ttu-id="f1744-118">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="f1744-118">expired</span></span>|<span data-ttu-id="f1744-119">2</span><span class="sxs-lookup"><span data-stu-id="f1744-119">2</span></span>|<span data-ttu-id="f1744-120">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="f1744-120">Token is expired.</span></span>|
|<span data-ttu-id="f1744-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="f1744-121">invalid</span></span>|<span data-ttu-id="f1744-122">3</span><span class="sxs-lookup"><span data-stu-id="f1744-122">3</span></span>|<span data-ttu-id="f1744-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="f1744-123">Token is invalid.</span></span>|
|<span data-ttu-id="f1744-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="f1744-124">assignedToExternalMDM</span></span>|<span data-ttu-id="f1744-125">4</span><span class="sxs-lookup"><span data-stu-id="f1744-125">4</span></span>|<span data-ttu-id="f1744-126">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="f1744-126">Token is managed by another MDM Service.</span></span>|





