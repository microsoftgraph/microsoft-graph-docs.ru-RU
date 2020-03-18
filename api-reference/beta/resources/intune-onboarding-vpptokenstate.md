---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 415c3b0df84c6b15a0185876280b82c7e8ed3d20
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777385"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="32760-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="32760-103">vppTokenState enum type</span></span>

> <span data-ttu-id="32760-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32760-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32760-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32760-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32760-106">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="32760-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="32760-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="32760-107">Members</span></span>
|<span data-ttu-id="32760-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="32760-108">Member</span></span>|<span data-ttu-id="32760-109">Значение</span><span class="sxs-lookup"><span data-stu-id="32760-109">Value</span></span>|<span data-ttu-id="32760-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32760-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32760-111">unknown</span><span class="sxs-lookup"><span data-stu-id="32760-111">unknown</span></span>|<span data-ttu-id="32760-112">нуль</span><span class="sxs-lookup"><span data-stu-id="32760-112">0</span></span>|<span data-ttu-id="32760-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="32760-113">Default state.</span></span>|
|<span data-ttu-id="32760-114">верно</span><span class="sxs-lookup"><span data-stu-id="32760-114">valid</span></span>|<span data-ttu-id="32760-115">1,1</span><span class="sxs-lookup"><span data-stu-id="32760-115">1</span></span>|<span data-ttu-id="32760-116">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="32760-116">Token is valid.</span></span>|
|<span data-ttu-id="32760-117">истек</span><span class="sxs-lookup"><span data-stu-id="32760-117">expired</span></span>|<span data-ttu-id="32760-118">2</span><span class="sxs-lookup"><span data-stu-id="32760-118">2</span></span>|<span data-ttu-id="32760-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="32760-119">Token is expired.</span></span>|
|<span data-ttu-id="32760-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="32760-120">invalid</span></span>|<span data-ttu-id="32760-121">4</span><span class="sxs-lookup"><span data-stu-id="32760-121">3</span></span>|<span data-ttu-id="32760-122">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="32760-122">Token is invalid.</span></span>|
|<span data-ttu-id="32760-123">ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="32760-123">assignedToExternalMDM</span></span>|<span data-ttu-id="32760-124">4 </span><span class="sxs-lookup"><span data-stu-id="32760-124">4</span></span>|<span data-ttu-id="32760-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="32760-125">Token is managed by another MDM Service.</span></span>|



