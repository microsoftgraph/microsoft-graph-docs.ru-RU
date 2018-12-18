---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
ms.openlocfilehash: e034f9712e2ef40b40b209935ed96f07b35cdbb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321184"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="b3402-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b3402-103">vppTokenState enum type</span></span>

> <span data-ttu-id="b3402-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3402-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3402-105">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="b3402-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="b3402-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b3402-106">Members</span></span>
|<span data-ttu-id="b3402-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b3402-107">Member</span></span>|<span data-ttu-id="b3402-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b3402-108">Value</span></span>|<span data-ttu-id="b3402-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3402-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3402-110">unknown</span><span class="sxs-lookup"><span data-stu-id="b3402-110">unknown</span></span>|<span data-ttu-id="b3402-111">0</span><span class="sxs-lookup"><span data-stu-id="b3402-111">0</span></span>|<span data-ttu-id="b3402-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b3402-112">Default state.</span></span>|
|<span data-ttu-id="b3402-113">допустимый</span><span class="sxs-lookup"><span data-stu-id="b3402-113">valid</span></span>|<span data-ttu-id="b3402-114">1</span><span class="sxs-lookup"><span data-stu-id="b3402-114">1</span></span>|<span data-ttu-id="b3402-115">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="b3402-115">Token is valid.</span></span>|
|<span data-ttu-id="b3402-116">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="b3402-116">expired</span></span>|<span data-ttu-id="b3402-117">2</span><span class="sxs-lookup"><span data-stu-id="b3402-117">2</span></span>|<span data-ttu-id="b3402-118">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="b3402-118">Token is expired.</span></span>|
|<span data-ttu-id="b3402-119">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="b3402-119">invalid</span></span>|<span data-ttu-id="b3402-120">3</span><span class="sxs-lookup"><span data-stu-id="b3402-120">3</span></span>|<span data-ttu-id="b3402-121">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="b3402-121">Token is invalid.</span></span>|
|<span data-ttu-id="b3402-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="b3402-122">assignedToExternalMDM</span></span>|<span data-ttu-id="b3402-123">4</span><span class="sxs-lookup"><span data-stu-id="b3402-123">4</span></span>|<span data-ttu-id="b3402-124">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="b3402-124">Token is managed by another MDM Service.</span></span>|



