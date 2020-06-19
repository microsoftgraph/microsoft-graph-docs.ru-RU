---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c286785522405946776907a296e475924ba8d4a8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793635"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="62d9e-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="62d9e-103">vppTokenState enum type</span></span>

<span data-ttu-id="62d9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62d9e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d9e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62d9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d9e-107">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="62d9e-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="62d9e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="62d9e-108">Members</span></span>
|<span data-ttu-id="62d9e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="62d9e-109">Member</span></span>|<span data-ttu-id="62d9e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="62d9e-110">Value</span></span>|<span data-ttu-id="62d9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="62d9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d9e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="62d9e-112">unknown</span></span>|<span data-ttu-id="62d9e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="62d9e-113">0</span></span>|<span data-ttu-id="62d9e-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="62d9e-114">Default state.</span></span>|
|<span data-ttu-id="62d9e-115">верно</span><span class="sxs-lookup"><span data-stu-id="62d9e-115">valid</span></span>|<span data-ttu-id="62d9e-116">1 </span><span class="sxs-lookup"><span data-stu-id="62d9e-116">1</span></span>|<span data-ttu-id="62d9e-117">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="62d9e-117">Token is valid.</span></span>|
|<span data-ttu-id="62d9e-118">истек</span><span class="sxs-lookup"><span data-stu-id="62d9e-118">expired</span></span>|<span data-ttu-id="62d9e-119">2</span><span class="sxs-lookup"><span data-stu-id="62d9e-119">2</span></span>|<span data-ttu-id="62d9e-120">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="62d9e-120">Token is expired.</span></span>|
|<span data-ttu-id="62d9e-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="62d9e-121">invalid</span></span>|<span data-ttu-id="62d9e-122">4</span><span class="sxs-lookup"><span data-stu-id="62d9e-122">3</span></span>|<span data-ttu-id="62d9e-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="62d9e-123">Token is invalid.</span></span>|
|<span data-ttu-id="62d9e-124">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="62d9e-124">assignedToExternalMDM</span></span>|<span data-ttu-id="62d9e-125">4 </span><span class="sxs-lookup"><span data-stu-id="62d9e-125">4</span></span>|<span data-ttu-id="62d9e-126">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="62d9e-126">Token is managed by another MDM Service.</span></span>|
|<span data-ttu-id="62d9e-127">дупликателокатионид</span><span class="sxs-lookup"><span data-stu-id="62d9e-127">duplicateLocationId</span></span>|<span data-ttu-id="62d9e-128">5 </span><span class="sxs-lookup"><span data-stu-id="62d9e-128">5</span></span>|<span data-ttu-id="62d9e-129">Маркер связан с тем же расположением, что и другой маркер учетной записи.</span><span class="sxs-lookup"><span data-stu-id="62d9e-129">Token is associated with the same location as another token on the account.</span></span>|



