---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21979c33bc1dcc06b83f9169341aa67ca516f066
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446825"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="234c0-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="234c0-103">vppTokenState enum type</span></span>

<span data-ttu-id="234c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="234c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="234c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="234c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="234c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="234c0-107">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="234c0-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="234c0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="234c0-108">Members</span></span>
|<span data-ttu-id="234c0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="234c0-109">Member</span></span>|<span data-ttu-id="234c0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="234c0-110">Value</span></span>|<span data-ttu-id="234c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="234c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="234c0-112">unknown</span><span class="sxs-lookup"><span data-stu-id="234c0-112">unknown</span></span>|<span data-ttu-id="234c0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="234c0-113">0</span></span>|<span data-ttu-id="234c0-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="234c0-114">Default state.</span></span>|
|<span data-ttu-id="234c0-115">верно</span><span class="sxs-lookup"><span data-stu-id="234c0-115">valid</span></span>|<span data-ttu-id="234c0-116">1,1</span><span class="sxs-lookup"><span data-stu-id="234c0-116">1</span></span>|<span data-ttu-id="234c0-117">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="234c0-117">Token is valid.</span></span>|
|<span data-ttu-id="234c0-118">истек</span><span class="sxs-lookup"><span data-stu-id="234c0-118">expired</span></span>|<span data-ttu-id="234c0-119">2</span><span class="sxs-lookup"><span data-stu-id="234c0-119">2</span></span>|<span data-ttu-id="234c0-120">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="234c0-120">Token is expired.</span></span>|
|<span data-ttu-id="234c0-121">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="234c0-121">invalid</span></span>|<span data-ttu-id="234c0-122">4</span><span class="sxs-lookup"><span data-stu-id="234c0-122">3</span></span>|<span data-ttu-id="234c0-123">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="234c0-123">Token is invalid.</span></span>|
|<span data-ttu-id="234c0-124">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="234c0-124">assignedToExternalMDM</span></span>|<span data-ttu-id="234c0-125">4 </span><span class="sxs-lookup"><span data-stu-id="234c0-125">4</span></span>|<span data-ttu-id="234c0-126">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="234c0-126">Token is managed by another MDM Service.</span></span>|



