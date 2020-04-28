---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d449fc723fd4c3a03c9a72bdbc74768b7db698c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402233"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="8e678-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="8e678-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="8e678-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e678-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e678-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e678-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e678-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e678-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e678-107">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="8e678-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="8e678-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8e678-108">Members</span></span>
|<span data-ttu-id="8e678-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8e678-109">Member</span></span>|<span data-ttu-id="8e678-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8e678-110">Value</span></span>|<span data-ttu-id="8e678-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e678-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e678-112">Нет</span><span class="sxs-lookup"><span data-stu-id="8e678-112">none</span></span>|<span data-ttu-id="8e678-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8e678-113">0</span></span>|<span data-ttu-id="8e678-114">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="8e678-114">Not revoked.</span></span>|
|<span data-ttu-id="8e678-115">закончен</span><span class="sxs-lookup"><span data-stu-id="8e678-115">pending</span></span>|<span data-ttu-id="8e678-116">1,1</span><span class="sxs-lookup"><span data-stu-id="8e678-116">1</span></span>|<span data-ttu-id="8e678-117">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="8e678-117">Revocation pending.</span></span>|
|<span data-ttu-id="8e678-118">опубликован</span><span class="sxs-lookup"><span data-stu-id="8e678-118">issued</span></span>|<span data-ttu-id="8e678-119">2</span><span class="sxs-lookup"><span data-stu-id="8e678-119">2</span></span>|<span data-ttu-id="8e678-120">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="8e678-120">Revocation command issued.</span></span>|
|<span data-ttu-id="8e678-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="8e678-121">failed</span></span>|<span data-ttu-id="8e678-122">4</span><span class="sxs-lookup"><span data-stu-id="8e678-122">3</span></span>|<span data-ttu-id="8e678-123">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="8e678-123">Revocation failed.</span></span>|
|<span data-ttu-id="8e678-124">отозван</span><span class="sxs-lookup"><span data-stu-id="8e678-124">revoked</span></span>|<span data-ttu-id="8e678-125">4 </span><span class="sxs-lookup"><span data-stu-id="8e678-125">4</span></span>|<span data-ttu-id="8e678-126">Отозван.</span><span class="sxs-lookup"><span data-stu-id="8e678-126">Revoked.</span></span>|



