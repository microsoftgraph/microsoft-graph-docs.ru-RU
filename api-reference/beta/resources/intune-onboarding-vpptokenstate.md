---
title: Тип перечисления vppTokenState
description: Возможные состояния, связанный с маркером покупки программы корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d0c4ee7ae0b8e35f97a18d0958a2456cab40a10
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416162"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="85bb1-103">Тип перечисления vppTokenState</span><span class="sxs-lookup"><span data-stu-id="85bb1-103">vppTokenState enum type</span></span>

> <span data-ttu-id="85bb1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85bb1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85bb1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85bb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85bb1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85bb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85bb1-107">Возможные состояния, связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="85bb1-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="85bb1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="85bb1-108">Members</span></span>
|<span data-ttu-id="85bb1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="85bb1-109">Member</span></span>|<span data-ttu-id="85bb1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="85bb1-110">Value</span></span>|<span data-ttu-id="85bb1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85bb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85bb1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="85bb1-112">unknown</span></span>|<span data-ttu-id="85bb1-113">0</span><span class="sxs-lookup"><span data-stu-id="85bb1-113">0</span></span>|<span data-ttu-id="85bb1-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="85bb1-114">Default state.</span></span>|
|<span data-ttu-id="85bb1-115">допустимый</span><span class="sxs-lookup"><span data-stu-id="85bb1-115">valid</span></span>|<span data-ttu-id="85bb1-116">1</span><span class="sxs-lookup"><span data-stu-id="85bb1-116">1</span></span>|<span data-ttu-id="85bb1-117">Маркер действителен.</span><span class="sxs-lookup"><span data-stu-id="85bb1-117">Token is valid.</span></span>|
|<span data-ttu-id="85bb1-118">истек срок действия</span><span class="sxs-lookup"><span data-stu-id="85bb1-118">expired</span></span>|<span data-ttu-id="85bb1-119">2</span><span class="sxs-lookup"><span data-stu-id="85bb1-119">2</span></span>|<span data-ttu-id="85bb1-120">Истек срок действия маркера.</span><span class="sxs-lookup"><span data-stu-id="85bb1-120">Token is expired.</span></span>|
|<span data-ttu-id="85bb1-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="85bb1-121">invalid</span></span>|<span data-ttu-id="85bb1-122">3</span><span class="sxs-lookup"><span data-stu-id="85bb1-122">3</span></span>|<span data-ttu-id="85bb1-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="85bb1-123">Token is invalid.</span></span>|
|<span data-ttu-id="85bb1-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="85bb1-124">assignedToExternalMDM</span></span>|<span data-ttu-id="85bb1-125">4</span><span class="sxs-lookup"><span data-stu-id="85bb1-125">4</span></span>|<span data-ttu-id="85bb1-126">Маркер управляется другой MDM службы.</span><span class="sxs-lookup"><span data-stu-id="85bb1-126">Token is managed by another MDM Service.</span></span>|




