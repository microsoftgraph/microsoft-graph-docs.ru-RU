---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c182cf2317f185108570116a283973d481f17ab2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159446"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="004c0-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="004c0-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="004c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="004c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="004c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="004c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="004c0-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="004c0-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="004c0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="004c0-107">Members</span></span>
|<span data-ttu-id="004c0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="004c0-108">Member</span></span>|<span data-ttu-id="004c0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="004c0-109">Value</span></span>|<span data-ttu-id="004c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="004c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="004c0-111">Нет</span><span class="sxs-lookup"><span data-stu-id="004c0-111">none</span></span>|<span data-ttu-id="004c0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="004c0-112">0</span></span>|<span data-ttu-id="004c0-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="004c0-113">Not revoked.</span></span>|
|<span data-ttu-id="004c0-114">закончен</span><span class="sxs-lookup"><span data-stu-id="004c0-114">pending</span></span>|<span data-ttu-id="004c0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="004c0-115">1</span></span>|<span data-ttu-id="004c0-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="004c0-116">Revocation pending.</span></span>|
|<span data-ttu-id="004c0-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="004c0-117">issued</span></span>|<span data-ttu-id="004c0-118">2</span><span class="sxs-lookup"><span data-stu-id="004c0-118">2</span></span>|<span data-ttu-id="004c0-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="004c0-119">Revocation command issued.</span></span>|
|<span data-ttu-id="004c0-120">failed</span><span class="sxs-lookup"><span data-stu-id="004c0-120">failed</span></span>|<span data-ttu-id="004c0-121">4</span><span class="sxs-lookup"><span data-stu-id="004c0-121">3</span></span>|<span data-ttu-id="004c0-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="004c0-122">Revocation failed.</span></span>|
|<span data-ttu-id="004c0-123">отозван</span><span class="sxs-lookup"><span data-stu-id="004c0-123">revoked</span></span>|<span data-ttu-id="004c0-124">4</span><span class="sxs-lookup"><span data-stu-id="004c0-124">4</span></span>|<span data-ttu-id="004c0-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="004c0-125">Revoked.</span></span>|




