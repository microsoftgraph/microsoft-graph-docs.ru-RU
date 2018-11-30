---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
ms.openlocfilehash: 74d7ea2e0ca2dd03b82b71bea2ab5300214b095d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024658"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="f8a9d-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="f8a9d-103">vppTokenState enum type</span></span>

> <span data-ttu-id="f8a9d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8a9d-105">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="f8a9d-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8a9d-106">Members</span></span>
|<span data-ttu-id="f8a9d-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8a9d-107">Member</span></span>|<span data-ttu-id="f8a9d-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f8a9d-108">Value</span></span>|<span data-ttu-id="f8a9d-109">Description</span><span class="sxs-lookup"><span data-stu-id="f8a9d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a9d-110">unknown</span><span class="sxs-lookup"><span data-stu-id="f8a9d-110">unknown</span></span>|<span data-ttu-id="f8a9d-111">0</span><span class="sxs-lookup"><span data-stu-id="f8a9d-111">0</span></span>|<span data-ttu-id="f8a9d-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-112">Default state.</span></span>|
|<span data-ttu-id="f8a9d-113">допустимый</span><span class="sxs-lookup"><span data-stu-id="f8a9d-113">valid</span></span>|<span data-ttu-id="f8a9d-114">1</span><span class="sxs-lookup"><span data-stu-id="f8a9d-114">1</span></span>|<span data-ttu-id="f8a9d-115">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-115">Token is valid.</span></span>|
|<span data-ttu-id="f8a9d-116">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="f8a9d-116">expired</span></span>|<span data-ttu-id="f8a9d-117">2</span><span class="sxs-lookup"><span data-stu-id="f8a9d-117">2</span></span>|<span data-ttu-id="f8a9d-118">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-118">Token is expired.</span></span>|
|<span data-ttu-id="f8a9d-119">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="f8a9d-119">invalid</span></span>|<span data-ttu-id="f8a9d-120">3</span><span class="sxs-lookup"><span data-stu-id="f8a9d-120">3</span></span>|<span data-ttu-id="f8a9d-121">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-121">Token is invalid.</span></span>|
|<span data-ttu-id="f8a9d-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="f8a9d-122">assignedToExternalMDM</span></span>|<span data-ttu-id="f8a9d-123">4</span><span class="sxs-lookup"><span data-stu-id="f8a9d-123">4</span></span>|<span data-ttu-id="f8a9d-124">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="f8a9d-124">Token is managed by another MDM Service.</span></span>|



