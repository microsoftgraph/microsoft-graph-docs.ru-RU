---
title: Тип перечисления certificateRevocationStatus
description: Сертификат отозван.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421972"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="37299-103">Тип перечисления certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="37299-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="37299-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37299-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37299-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37299-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37299-107">Сертификат отозван.</span><span class="sxs-lookup"><span data-stu-id="37299-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="37299-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="37299-108">Members</span></span>
|<span data-ttu-id="37299-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="37299-109">Member</span></span>|<span data-ttu-id="37299-110">Значение</span><span class="sxs-lookup"><span data-stu-id="37299-110">Value</span></span>|<span data-ttu-id="37299-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37299-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37299-112">none</span><span class="sxs-lookup"><span data-stu-id="37299-112">none</span></span>|<span data-ttu-id="37299-113">0</span><span class="sxs-lookup"><span data-stu-id="37299-113">0</span></span>|<span data-ttu-id="37299-114">Не был отозван.</span><span class="sxs-lookup"><span data-stu-id="37299-114">Not revoked.</span></span>|
|<span data-ttu-id="37299-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="37299-115">pending</span></span>|<span data-ttu-id="37299-116">1</span><span class="sxs-lookup"><span data-stu-id="37299-116">1</span></span>|<span data-ttu-id="37299-117">Отзыва ожидающие.</span><span class="sxs-lookup"><span data-stu-id="37299-117">Revocation pending.</span></span>|
|<span data-ttu-id="37299-118">выдан</span><span class="sxs-lookup"><span data-stu-id="37299-118">issued</span></span>|<span data-ttu-id="37299-119">2</span><span class="sxs-lookup"><span data-stu-id="37299-119">2</span></span>|<span data-ttu-id="37299-120">Отзыва команды.</span><span class="sxs-lookup"><span data-stu-id="37299-120">Revocation command issued.</span></span>|
|<span data-ttu-id="37299-121">failed</span><span class="sxs-lookup"><span data-stu-id="37299-121">failed</span></span>|<span data-ttu-id="37299-122">3</span><span class="sxs-lookup"><span data-stu-id="37299-122">3</span></span>|<span data-ttu-id="37299-123">Не удалось отзыва.</span><span class="sxs-lookup"><span data-stu-id="37299-123">Revocation failed.</span></span>|
|<span data-ttu-id="37299-124">отменено</span><span class="sxs-lookup"><span data-stu-id="37299-124">revoked</span></span>|<span data-ttu-id="37299-125">4</span><span class="sxs-lookup"><span data-stu-id="37299-125">4</span></span>|<span data-ttu-id="37299-126">Был отозван.</span><span class="sxs-lookup"><span data-stu-id="37299-126">Revoked.</span></span>|




