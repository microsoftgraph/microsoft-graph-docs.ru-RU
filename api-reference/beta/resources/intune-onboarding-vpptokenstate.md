---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d9ae2b3bfb45ff33c5f0a39d746350212db3027c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010639"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="9dc1f-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="9dc1f-103">vppTokenState enum type</span></span>

> <span data-ttu-id="9dc1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dc1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dc1f-106">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="9dc1f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9dc1f-107">Members</span></span>
|<span data-ttu-id="9dc1f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9dc1f-108">Member</span></span>|<span data-ttu-id="9dc1f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9dc1f-109">Value</span></span>|<span data-ttu-id="9dc1f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc1f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dc1f-111">unknown</span><span class="sxs-lookup"><span data-stu-id="9dc1f-111">unknown</span></span>|<span data-ttu-id="9dc1f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9dc1f-112">0</span></span>|<span data-ttu-id="9dc1f-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-113">Default state.</span></span>|
|<span data-ttu-id="9dc1f-114">верно</span><span class="sxs-lookup"><span data-stu-id="9dc1f-114">valid</span></span>|<span data-ttu-id="9dc1f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9dc1f-115">1</span></span>|<span data-ttu-id="9dc1f-116">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-116">Token is valid.</span></span>|
|<span data-ttu-id="9dc1f-117">истек</span><span class="sxs-lookup"><span data-stu-id="9dc1f-117">expired</span></span>|<span data-ttu-id="9dc1f-118">2</span><span class="sxs-lookup"><span data-stu-id="9dc1f-118">2</span></span>|<span data-ttu-id="9dc1f-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-119">Token is expired.</span></span>|
|<span data-ttu-id="9dc1f-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="9dc1f-120">invalid</span></span>|<span data-ttu-id="9dc1f-121">4</span><span class="sxs-lookup"><span data-stu-id="9dc1f-121">3</span></span>|<span data-ttu-id="9dc1f-122">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-122">Token is invalid.</span></span>|
|<span data-ttu-id="9dc1f-123">Ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="9dc1f-123">assignedToExternalMDM</span></span>|<span data-ttu-id="9dc1f-124">SP4</span><span class="sxs-lookup"><span data-stu-id="9dc1f-124">4</span></span>|<span data-ttu-id="9dc1f-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="9dc1f-125">Token is managed by another MDM Service.</span></span>|





