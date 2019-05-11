---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd568bdb4430f61a52577617876a682cc4f7ed99
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940241"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="a964b-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="a964b-103">vppTokenState enum type</span></span>

> <span data-ttu-id="a964b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a964b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a964b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a964b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a964b-106">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a964b-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="a964b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a964b-107">Members</span></span>
|<span data-ttu-id="a964b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a964b-108">Member</span></span>|<span data-ttu-id="a964b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a964b-109">Value</span></span>|<span data-ttu-id="a964b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a964b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a964b-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a964b-111">unknown</span></span>|<span data-ttu-id="a964b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a964b-112">0</span></span>|<span data-ttu-id="a964b-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a964b-113">Default state.</span></span>|
|<span data-ttu-id="a964b-114">верно</span><span class="sxs-lookup"><span data-stu-id="a964b-114">valid</span></span>|<span data-ttu-id="a964b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a964b-115">1</span></span>|<span data-ttu-id="a964b-116">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="a964b-116">Token is valid.</span></span>|
|<span data-ttu-id="a964b-117">истек</span><span class="sxs-lookup"><span data-stu-id="a964b-117">expired</span></span>|<span data-ttu-id="a964b-118">2</span><span class="sxs-lookup"><span data-stu-id="a964b-118">2</span></span>|<span data-ttu-id="a964b-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="a964b-119">Token is expired.</span></span>|
|<span data-ttu-id="a964b-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="a964b-120">invalid</span></span>|<span data-ttu-id="a964b-121">4</span><span class="sxs-lookup"><span data-stu-id="a964b-121">3</span></span>|<span data-ttu-id="a964b-122">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="a964b-122">Token is invalid.</span></span>|
|<span data-ttu-id="a964b-123">Ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="a964b-123">assignedToExternalMDM</span></span>|<span data-ttu-id="a964b-124">SP4</span><span class="sxs-lookup"><span data-stu-id="a964b-124">4</span></span>|<span data-ttu-id="a964b-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="a964b-125">Token is managed by another MDM Service.</span></span>|




