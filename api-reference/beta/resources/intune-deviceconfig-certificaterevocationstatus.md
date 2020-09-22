---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0698e527a75c414b714f9b00f61f2c2f7c036388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081568"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="dcb75-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="dcb75-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="dcb75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcb75-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb75-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcb75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb75-107">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcb75-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="dcb75-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dcb75-108">Members</span></span>
|<span data-ttu-id="dcb75-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dcb75-109">Member</span></span>|<span data-ttu-id="dcb75-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dcb75-110">Value</span></span>|<span data-ttu-id="dcb75-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb75-112">Нет</span><span class="sxs-lookup"><span data-stu-id="dcb75-112">none</span></span>|<span data-ttu-id="dcb75-113">нуль</span><span class="sxs-lookup"><span data-stu-id="dcb75-113">0</span></span>|<span data-ttu-id="dcb75-114">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="dcb75-114">Not revoked.</span></span>|
|<span data-ttu-id="dcb75-115">закончен</span><span class="sxs-lookup"><span data-stu-id="dcb75-115">pending</span></span>|<span data-ttu-id="dcb75-116">1 </span><span class="sxs-lookup"><span data-stu-id="dcb75-116">1</span></span>|<span data-ttu-id="dcb75-117">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="dcb75-117">Revocation pending.</span></span>|
|<span data-ttu-id="dcb75-118">опубликован</span><span class="sxs-lookup"><span data-stu-id="dcb75-118">issued</span></span>|<span data-ttu-id="dcb75-119">2 </span><span class="sxs-lookup"><span data-stu-id="dcb75-119">2</span></span>|<span data-ttu-id="dcb75-120">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="dcb75-120">Revocation command issued.</span></span>|
|<span data-ttu-id="dcb75-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="dcb75-121">failed</span></span>|<span data-ttu-id="dcb75-122">4</span><span class="sxs-lookup"><span data-stu-id="dcb75-122">3</span></span>|<span data-ttu-id="dcb75-123">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="dcb75-123">Revocation failed.</span></span>|
|<span data-ttu-id="dcb75-124">отозван</span><span class="sxs-lookup"><span data-stu-id="dcb75-124">revoked</span></span>|<span data-ttu-id="dcb75-125">4 </span><span class="sxs-lookup"><span data-stu-id="dcb75-125">4</span></span>|<span data-ttu-id="dcb75-126">Отозван.</span><span class="sxs-lookup"><span data-stu-id="dcb75-126">Revoked.</span></span>|






