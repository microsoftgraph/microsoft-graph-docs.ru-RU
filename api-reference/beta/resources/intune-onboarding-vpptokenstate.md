---
title: тип перечисления Впптокенстате
description: Возможные состояния, связанные с токеном Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdb356d5103fc1c1dc07245d8552cb77b9383c8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159866"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="773f4-103">тип перечисления Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="773f4-103">vppTokenState enum type</span></span>

> <span data-ttu-id="773f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="773f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="773f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="773f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="773f4-106">Возможные состояния, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="773f4-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="773f4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="773f4-107">Members</span></span>
|<span data-ttu-id="773f4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="773f4-108">Member</span></span>|<span data-ttu-id="773f4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="773f4-109">Value</span></span>|<span data-ttu-id="773f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="773f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="773f4-111">unknown</span><span class="sxs-lookup"><span data-stu-id="773f4-111">unknown</span></span>|<span data-ttu-id="773f4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="773f4-112">0</span></span>|<span data-ttu-id="773f4-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="773f4-113">Default state.</span></span>|
|<span data-ttu-id="773f4-114">верно</span><span class="sxs-lookup"><span data-stu-id="773f4-114">valid</span></span>|<span data-ttu-id="773f4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="773f4-115">1</span></span>|<span data-ttu-id="773f4-116">Токен является допустимым.</span><span class="sxs-lookup"><span data-stu-id="773f4-116">Token is valid.</span></span>|
|<span data-ttu-id="773f4-117">истек</span><span class="sxs-lookup"><span data-stu-id="773f4-117">expired</span></span>|<span data-ttu-id="773f4-118">2</span><span class="sxs-lookup"><span data-stu-id="773f4-118">2</span></span>|<span data-ttu-id="773f4-119">Срок действия маркера истек.</span><span class="sxs-lookup"><span data-stu-id="773f4-119">Token is expired.</span></span>|
|<span data-ttu-id="773f4-120">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="773f4-120">invalid</span></span>|<span data-ttu-id="773f4-121">4</span><span class="sxs-lookup"><span data-stu-id="773f4-121">3</span></span>|<span data-ttu-id="773f4-122">Недопустимый маркер.</span><span class="sxs-lookup"><span data-stu-id="773f4-122">Token is invalid.</span></span>|
|<span data-ttu-id="773f4-123">Ассигнедтоекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="773f4-123">assignedToExternalMDM</span></span>|<span data-ttu-id="773f4-124">4</span><span class="sxs-lookup"><span data-stu-id="773f4-124">4</span></span>|<span data-ttu-id="773f4-125">Маркер управляется другой службой MDM.</span><span class="sxs-lookup"><span data-stu-id="773f4-125">Token is managed by another MDM Service.</span></span>|




