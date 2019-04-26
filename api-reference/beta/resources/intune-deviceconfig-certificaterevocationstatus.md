---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549387"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="70390-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="70390-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="70390-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70390-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70390-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70390-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70390-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="70390-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="70390-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="70390-107">Members</span></span>
|<span data-ttu-id="70390-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="70390-108">Member</span></span>|<span data-ttu-id="70390-109">Значение</span><span class="sxs-lookup"><span data-stu-id="70390-109">Value</span></span>|<span data-ttu-id="70390-110">Описание</span><span class="sxs-lookup"><span data-stu-id="70390-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70390-111">Нет</span><span class="sxs-lookup"><span data-stu-id="70390-111">none</span></span>|<span data-ttu-id="70390-112">нуль</span><span class="sxs-lookup"><span data-stu-id="70390-112">0</span></span>|<span data-ttu-id="70390-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="70390-113">Not revoked.</span></span>|
|<span data-ttu-id="70390-114">закончен</span><span class="sxs-lookup"><span data-stu-id="70390-114">pending</span></span>|<span data-ttu-id="70390-115">1 </span><span class="sxs-lookup"><span data-stu-id="70390-115">1</span></span>|<span data-ttu-id="70390-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="70390-116">Revocation pending.</span></span>|
|<span data-ttu-id="70390-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="70390-117">issued</span></span>|<span data-ttu-id="70390-118">2 </span><span class="sxs-lookup"><span data-stu-id="70390-118">2</span></span>|<span data-ttu-id="70390-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="70390-119">Revocation command issued.</span></span>|
|<span data-ttu-id="70390-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="70390-120">failed</span></span>|<span data-ttu-id="70390-121">3 </span><span class="sxs-lookup"><span data-stu-id="70390-121">3</span></span>|<span data-ttu-id="70390-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="70390-122">Revocation failed.</span></span>|
|<span data-ttu-id="70390-123">отозван</span><span class="sxs-lookup"><span data-stu-id="70390-123">revoked</span></span>|<span data-ttu-id="70390-124">4 </span><span class="sxs-lookup"><span data-stu-id="70390-124">4</span></span>|<span data-ttu-id="70390-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="70390-125">Revoked.</span></span>|





