---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0e0342924faf166e6daf0a66149e841b88d6d0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795696"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="27a79-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="27a79-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="27a79-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27a79-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27a79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27a79-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="27a79-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="27a79-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="27a79-107">Members</span></span>
|<span data-ttu-id="27a79-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="27a79-108">Member</span></span>|<span data-ttu-id="27a79-109">Значение</span><span class="sxs-lookup"><span data-stu-id="27a79-109">Value</span></span>|<span data-ttu-id="27a79-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27a79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a79-111">none</span><span class="sxs-lookup"><span data-stu-id="27a79-111">none</span></span>|<span data-ttu-id="27a79-112">нуль</span><span class="sxs-lookup"><span data-stu-id="27a79-112">0</span></span>|<span data-ttu-id="27a79-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="27a79-113">Not revoked.</span></span>|
|<span data-ttu-id="27a79-114">закончен</span><span class="sxs-lookup"><span data-stu-id="27a79-114">pending</span></span>|<span data-ttu-id="27a79-115">1,1</span><span class="sxs-lookup"><span data-stu-id="27a79-115">1</span></span>|<span data-ttu-id="27a79-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="27a79-116">Revocation pending.</span></span>|
|<span data-ttu-id="27a79-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="27a79-117">issued</span></span>|<span data-ttu-id="27a79-118">2</span><span class="sxs-lookup"><span data-stu-id="27a79-118">2</span></span>|<span data-ttu-id="27a79-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="27a79-119">Revocation command issued.</span></span>|
|<span data-ttu-id="27a79-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="27a79-120">failed</span></span>|<span data-ttu-id="27a79-121">4</span><span class="sxs-lookup"><span data-stu-id="27a79-121">3</span></span>|<span data-ttu-id="27a79-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="27a79-122">Revocation failed.</span></span>|
|<span data-ttu-id="27a79-123">отозван</span><span class="sxs-lookup"><span data-stu-id="27a79-123">revoked</span></span>|<span data-ttu-id="27a79-124">4 </span><span class="sxs-lookup"><span data-stu-id="27a79-124">4</span></span>|<span data-ttu-id="27a79-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="27a79-125">Revoked.</span></span>|



