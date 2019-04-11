---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782809"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="bd08e-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="bd08e-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="bd08e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd08e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd08e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd08e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd08e-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd08e-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="bd08e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd08e-107">Members</span></span>
|<span data-ttu-id="bd08e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd08e-108">Member</span></span>|<span data-ttu-id="bd08e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bd08e-109">Value</span></span>|<span data-ttu-id="bd08e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd08e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd08e-111">нет</span><span class="sxs-lookup"><span data-stu-id="bd08e-111">none</span></span>|<span data-ttu-id="bd08e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bd08e-112">0</span></span>|<span data-ttu-id="bd08e-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="bd08e-113">Not revoked.</span></span>|
|<span data-ttu-id="bd08e-114">закончен</span><span class="sxs-lookup"><span data-stu-id="bd08e-114">pending</span></span>|<span data-ttu-id="bd08e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bd08e-115">1</span></span>|<span data-ttu-id="bd08e-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="bd08e-116">Revocation pending.</span></span>|
|<span data-ttu-id="bd08e-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="bd08e-117">issued</span></span>|<span data-ttu-id="bd08e-118">2</span><span class="sxs-lookup"><span data-stu-id="bd08e-118">2</span></span>|<span data-ttu-id="bd08e-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="bd08e-119">Revocation command issued.</span></span>|
|<span data-ttu-id="bd08e-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="bd08e-120">failed</span></span>|<span data-ttu-id="bd08e-121">4</span><span class="sxs-lookup"><span data-stu-id="bd08e-121">3</span></span>|<span data-ttu-id="bd08e-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="bd08e-122">Revocation failed.</span></span>|
|<span data-ttu-id="bd08e-123">отозван</span><span class="sxs-lookup"><span data-stu-id="bd08e-123">revoked</span></span>|<span data-ttu-id="bd08e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="bd08e-124">4</span></span>|<span data-ttu-id="bd08e-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="bd08e-125">Revoked.</span></span>|





