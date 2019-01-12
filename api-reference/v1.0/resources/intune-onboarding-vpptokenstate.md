---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6bdeb73b6491f3960ce30db91a35d06c0f8ffaf1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986665"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="87160-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="87160-103">vppTokenState enum type</span></span>

> <span data-ttu-id="87160-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87160-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87160-105">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="87160-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="87160-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="87160-106">Members</span></span>
|<span data-ttu-id="87160-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="87160-107">Member</span></span>|<span data-ttu-id="87160-108">Значение</span><span class="sxs-lookup"><span data-stu-id="87160-108">Value</span></span>|<span data-ttu-id="87160-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87160-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87160-110">unknown</span><span class="sxs-lookup"><span data-stu-id="87160-110">unknown</span></span>|<span data-ttu-id="87160-111">0</span><span class="sxs-lookup"><span data-stu-id="87160-111">0</span></span>|<span data-ttu-id="87160-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="87160-112">Default state.</span></span>|
|<span data-ttu-id="87160-113">допустимый</span><span class="sxs-lookup"><span data-stu-id="87160-113">valid</span></span>|<span data-ttu-id="87160-114">1</span><span class="sxs-lookup"><span data-stu-id="87160-114">1</span></span>|<span data-ttu-id="87160-115">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="87160-115">Token is valid.</span></span>|
|<span data-ttu-id="87160-116">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="87160-116">expired</span></span>|<span data-ttu-id="87160-117">2</span><span class="sxs-lookup"><span data-stu-id="87160-117">2</span></span>|<span data-ttu-id="87160-118">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="87160-118">Token is expired.</span></span>|
|<span data-ttu-id="87160-119">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="87160-119">invalid</span></span>|<span data-ttu-id="87160-120">3</span><span class="sxs-lookup"><span data-stu-id="87160-120">3</span></span>|<span data-ttu-id="87160-121">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="87160-121">Token is invalid.</span></span>|
|<span data-ttu-id="87160-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="87160-122">assignedToExternalMDM</span></span>|<span data-ttu-id="87160-123">4</span><span class="sxs-lookup"><span data-stu-id="87160-123">4</span></span>|<span data-ttu-id="87160-124">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="87160-124">Token is managed by another MDM Service.</span></span>|



