---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a1231373597096905d4e0614d4b1b6e2d70b6c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971013"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="794a9-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="794a9-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="794a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="794a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="794a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="794a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="794a9-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="794a9-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="794a9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="794a9-107">Members</span></span>
|<span data-ttu-id="794a9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="794a9-108">Member</span></span>|<span data-ttu-id="794a9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="794a9-109">Value</span></span>|<span data-ttu-id="794a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="794a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="794a9-111">none</span><span class="sxs-lookup"><span data-stu-id="794a9-111">none</span></span>|<span data-ttu-id="794a9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="794a9-112">0</span></span>|<span data-ttu-id="794a9-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="794a9-113">Not revoked.</span></span>|
|<span data-ttu-id="794a9-114">закончен</span><span class="sxs-lookup"><span data-stu-id="794a9-114">pending</span></span>|<span data-ttu-id="794a9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="794a9-115">1</span></span>|<span data-ttu-id="794a9-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="794a9-116">Revocation pending.</span></span>|
|<span data-ttu-id="794a9-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="794a9-117">issued</span></span>|<span data-ttu-id="794a9-118">2</span><span class="sxs-lookup"><span data-stu-id="794a9-118">2</span></span>|<span data-ttu-id="794a9-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="794a9-119">Revocation command issued.</span></span>|
|<span data-ttu-id="794a9-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="794a9-120">failed</span></span>|<span data-ttu-id="794a9-121">4</span><span class="sxs-lookup"><span data-stu-id="794a9-121">3</span></span>|<span data-ttu-id="794a9-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="794a9-122">Revocation failed.</span></span>|
|<span data-ttu-id="794a9-123">отозван</span><span class="sxs-lookup"><span data-stu-id="794a9-123">revoked</span></span>|<span data-ttu-id="794a9-124">SP4</span><span class="sxs-lookup"><span data-stu-id="794a9-124">4</span></span>|<span data-ttu-id="794a9-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="794a9-125">Revoked.</span></span>|





