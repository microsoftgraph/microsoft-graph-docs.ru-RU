---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3e78e5762c1d59d882973a44f69482fcb21998f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527685"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="503e2-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="503e2-103">vppTokenState enum type</span></span>

<span data-ttu-id="503e2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="503e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="503e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="503e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503e2-107">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="503e2-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="503e2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="503e2-108">Members</span></span>
|<span data-ttu-id="503e2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="503e2-109">Member</span></span>|<span data-ttu-id="503e2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="503e2-110">Value</span></span>|<span data-ttu-id="503e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="503e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503e2-112">unknown</span><span class="sxs-lookup"><span data-stu-id="503e2-112">unknown</span></span>|<span data-ttu-id="503e2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="503e2-113">0</span></span>|<span data-ttu-id="503e2-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="503e2-114">Default state.</span></span>|
|<span data-ttu-id="503e2-115">верно</span><span class="sxs-lookup"><span data-stu-id="503e2-115">valid</span></span>|<span data-ttu-id="503e2-116">1 </span><span class="sxs-lookup"><span data-stu-id="503e2-116">1</span></span>|<span data-ttu-id="503e2-117">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="503e2-117">Token is valid.</span></span>|
|<span data-ttu-id="503e2-118">истек</span><span class="sxs-lookup"><span data-stu-id="503e2-118">expired</span></span>|<span data-ttu-id="503e2-119">2 </span><span class="sxs-lookup"><span data-stu-id="503e2-119">2</span></span>|<span data-ttu-id="503e2-120">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="503e2-120">Token is expired.</span></span>|
|<span data-ttu-id="503e2-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="503e2-121">invalid</span></span>|<span data-ttu-id="503e2-122">3 </span><span class="sxs-lookup"><span data-stu-id="503e2-122">3</span></span>|<span data-ttu-id="503e2-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="503e2-123">Token is invalid.</span></span>|
|<span data-ttu-id="503e2-124">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="503e2-124">assignedToExternalMDM</span></span>|<span data-ttu-id="503e2-125">4 </span><span class="sxs-lookup"><span data-stu-id="503e2-125">4</span></span>|<span data-ttu-id="503e2-126">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="503e2-126">Token is managed by another MDM Service.</span></span>|



