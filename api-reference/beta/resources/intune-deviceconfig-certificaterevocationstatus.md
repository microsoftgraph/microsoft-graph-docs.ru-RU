---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4544968e473c41d787df606112801c9b60e2cb98
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947430"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="da2a8-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="da2a8-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="da2a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da2a8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da2a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da2a8-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="da2a8-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="da2a8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="da2a8-107">Members</span></span>
|<span data-ttu-id="da2a8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="da2a8-108">Member</span></span>|<span data-ttu-id="da2a8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="da2a8-109">Value</span></span>|<span data-ttu-id="da2a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="da2a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2a8-111">none</span><span class="sxs-lookup"><span data-stu-id="da2a8-111">none</span></span>|<span data-ttu-id="da2a8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="da2a8-112">0</span></span>|<span data-ttu-id="da2a8-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="da2a8-113">Not revoked.</span></span>|
|<span data-ttu-id="da2a8-114">закончен</span><span class="sxs-lookup"><span data-stu-id="da2a8-114">pending</span></span>|<span data-ttu-id="da2a8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="da2a8-115">1</span></span>|<span data-ttu-id="da2a8-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="da2a8-116">Revocation pending.</span></span>|
|<span data-ttu-id="da2a8-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="da2a8-117">issued</span></span>|<span data-ttu-id="da2a8-118">2</span><span class="sxs-lookup"><span data-stu-id="da2a8-118">2</span></span>|<span data-ttu-id="da2a8-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="da2a8-119">Revocation command issued.</span></span>|
|<span data-ttu-id="da2a8-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="da2a8-120">failed</span></span>|<span data-ttu-id="da2a8-121">4</span><span class="sxs-lookup"><span data-stu-id="da2a8-121">3</span></span>|<span data-ttu-id="da2a8-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="da2a8-122">Revocation failed.</span></span>|
|<span data-ttu-id="da2a8-123">отозван</span><span class="sxs-lookup"><span data-stu-id="da2a8-123">revoked</span></span>|<span data-ttu-id="da2a8-124">SP4</span><span class="sxs-lookup"><span data-stu-id="da2a8-124">4</span></span>|<span data-ttu-id="da2a8-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="da2a8-125">Revoked.</span></span>|




