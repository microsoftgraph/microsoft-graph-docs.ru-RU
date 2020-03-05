---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 644b1d58a38d23d71a2fa56e7bfd5d678ffee76e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447999"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="a5771-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="a5771-103">vppTokenState enum type</span></span>

<span data-ttu-id="a5771-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a5771-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5771-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5771-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5771-106">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a5771-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="a5771-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a5771-107">Members</span></span>
|<span data-ttu-id="a5771-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5771-108">Member</span></span>|<span data-ttu-id="a5771-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a5771-109">Value</span></span>|<span data-ttu-id="a5771-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5771-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5771-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a5771-111">unknown</span></span>|<span data-ttu-id="a5771-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a5771-112">0</span></span>|<span data-ttu-id="a5771-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5771-113">Default state.</span></span>|
|<span data-ttu-id="a5771-114">верно</span><span class="sxs-lookup"><span data-stu-id="a5771-114">valid</span></span>|<span data-ttu-id="a5771-115">1 </span><span class="sxs-lookup"><span data-stu-id="a5771-115">1</span></span>|<span data-ttu-id="a5771-116">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="a5771-116">Token is valid.</span></span>|
|<span data-ttu-id="a5771-117">истек</span><span class="sxs-lookup"><span data-stu-id="a5771-117">expired</span></span>|<span data-ttu-id="a5771-118">2 </span><span class="sxs-lookup"><span data-stu-id="a5771-118">2</span></span>|<span data-ttu-id="a5771-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="a5771-119">Token is expired.</span></span>|
|<span data-ttu-id="a5771-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="a5771-120">invalid</span></span>|<span data-ttu-id="a5771-121">3 </span><span class="sxs-lookup"><span data-stu-id="a5771-121">3</span></span>|<span data-ttu-id="a5771-122">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="a5771-122">Token is invalid.</span></span>|
|<span data-ttu-id="a5771-123">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="a5771-123">assignedToExternalMDM</span></span>|<span data-ttu-id="a5771-124">4 </span><span class="sxs-lookup"><span data-stu-id="a5771-124">4</span></span>|<span data-ttu-id="a5771-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="a5771-125">Token is managed by another MDM Service.</span></span>|




