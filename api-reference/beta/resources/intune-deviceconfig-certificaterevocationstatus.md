---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef7181707e6e80c9ad816f345f2a299dbce147e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990115"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="31eb4-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="31eb4-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="31eb4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31eb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31eb4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31eb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31eb4-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="31eb4-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="31eb4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="31eb4-107">Members</span></span>
|<span data-ttu-id="31eb4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="31eb4-108">Member</span></span>|<span data-ttu-id="31eb4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="31eb4-109">Value</span></span>|<span data-ttu-id="31eb4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="31eb4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31eb4-111">none</span><span class="sxs-lookup"><span data-stu-id="31eb4-111">none</span></span>|<span data-ttu-id="31eb4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="31eb4-112">0</span></span>|<span data-ttu-id="31eb4-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="31eb4-113">Not revoked.</span></span>|
|<span data-ttu-id="31eb4-114">закончен</span><span class="sxs-lookup"><span data-stu-id="31eb4-114">pending</span></span>|<span data-ttu-id="31eb4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="31eb4-115">1</span></span>|<span data-ttu-id="31eb4-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="31eb4-116">Revocation pending.</span></span>|
|<span data-ttu-id="31eb4-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="31eb4-117">issued</span></span>|<span data-ttu-id="31eb4-118">2</span><span class="sxs-lookup"><span data-stu-id="31eb4-118">2</span></span>|<span data-ttu-id="31eb4-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="31eb4-119">Revocation command issued.</span></span>|
|<span data-ttu-id="31eb4-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="31eb4-120">failed</span></span>|<span data-ttu-id="31eb4-121">4</span><span class="sxs-lookup"><span data-stu-id="31eb4-121">3</span></span>|<span data-ttu-id="31eb4-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="31eb4-122">Revocation failed.</span></span>|
|<span data-ttu-id="31eb4-123">отозван</span><span class="sxs-lookup"><span data-stu-id="31eb4-123">revoked</span></span>|<span data-ttu-id="31eb4-124">SP4</span><span class="sxs-lookup"><span data-stu-id="31eb4-124">4</span></span>|<span data-ttu-id="31eb4-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="31eb4-125">Revoked.</span></span>|





