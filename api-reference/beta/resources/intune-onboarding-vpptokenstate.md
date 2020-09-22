---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1789debbbc672d0ee195af788292fd556d25e899
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029332"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="2ba39-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="2ba39-103">vppTokenState enum type</span></span>

<span data-ttu-id="2ba39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ba39-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba39-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ba39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba39-107">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2ba39-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="2ba39-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2ba39-108">Members</span></span>
|<span data-ttu-id="2ba39-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2ba39-109">Member</span></span>|<span data-ttu-id="2ba39-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2ba39-110">Value</span></span>|<span data-ttu-id="2ba39-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba39-112">unknown</span><span class="sxs-lookup"><span data-stu-id="2ba39-112">unknown</span></span>|<span data-ttu-id="2ba39-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2ba39-113">0</span></span>|<span data-ttu-id="2ba39-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2ba39-114">Default state.</span></span>|
|<span data-ttu-id="2ba39-115">верно</span><span class="sxs-lookup"><span data-stu-id="2ba39-115">valid</span></span>|<span data-ttu-id="2ba39-116">1 </span><span class="sxs-lookup"><span data-stu-id="2ba39-116">1</span></span>|<span data-ttu-id="2ba39-117">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="2ba39-117">Token is valid.</span></span>|
|<span data-ttu-id="2ba39-118">истек</span><span class="sxs-lookup"><span data-stu-id="2ba39-118">expired</span></span>|<span data-ttu-id="2ba39-119">2 </span><span class="sxs-lookup"><span data-stu-id="2ba39-119">2</span></span>|<span data-ttu-id="2ba39-120">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="2ba39-120">Token is expired.</span></span>|
|<span data-ttu-id="2ba39-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="2ba39-121">invalid</span></span>|<span data-ttu-id="2ba39-122">4</span><span class="sxs-lookup"><span data-stu-id="2ba39-122">3</span></span>|<span data-ttu-id="2ba39-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="2ba39-123">Token is invalid.</span></span>|
|<span data-ttu-id="2ba39-124">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="2ba39-124">assignedToExternalMDM</span></span>|<span data-ttu-id="2ba39-125">4 </span><span class="sxs-lookup"><span data-stu-id="2ba39-125">4</span></span>|<span data-ttu-id="2ba39-126">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="2ba39-126">Token is managed by another MDM Service.</span></span>|
|<span data-ttu-id="2ba39-127">дупликателокатионид</span><span class="sxs-lookup"><span data-stu-id="2ba39-127">duplicateLocationId</span></span>|<span data-ttu-id="2ba39-128">5 </span><span class="sxs-lookup"><span data-stu-id="2ba39-128">5</span></span>|<span data-ttu-id="2ba39-129">Маркер связан с тем же расположением, что и другой маркер учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2ba39-129">Token is associated with the same location as another token on the account.</span></span>|






