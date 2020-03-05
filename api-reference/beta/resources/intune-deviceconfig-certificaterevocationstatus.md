---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 870cf8a59dc2f7a8ae26f3e7a76dd49249b0e008
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526981"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="2923a-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="2923a-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="2923a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2923a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2923a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2923a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2923a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2923a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2923a-107">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="2923a-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="2923a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2923a-108">Members</span></span>
|<span data-ttu-id="2923a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2923a-109">Member</span></span>|<span data-ttu-id="2923a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2923a-110">Value</span></span>|<span data-ttu-id="2923a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2923a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2923a-112">нет</span><span class="sxs-lookup"><span data-stu-id="2923a-112">none</span></span>|<span data-ttu-id="2923a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2923a-113">0</span></span>|<span data-ttu-id="2923a-114">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="2923a-114">Not revoked.</span></span>|
|<span data-ttu-id="2923a-115">закончен</span><span class="sxs-lookup"><span data-stu-id="2923a-115">pending</span></span>|<span data-ttu-id="2923a-116">1 </span><span class="sxs-lookup"><span data-stu-id="2923a-116">1</span></span>|<span data-ttu-id="2923a-117">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="2923a-117">Revocation pending.</span></span>|
|<span data-ttu-id="2923a-118">опубликован</span><span class="sxs-lookup"><span data-stu-id="2923a-118">issued</span></span>|<span data-ttu-id="2923a-119">2 </span><span class="sxs-lookup"><span data-stu-id="2923a-119">2</span></span>|<span data-ttu-id="2923a-120">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="2923a-120">Revocation command issued.</span></span>|
|<span data-ttu-id="2923a-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="2923a-121">failed</span></span>|<span data-ttu-id="2923a-122">3 </span><span class="sxs-lookup"><span data-stu-id="2923a-122">3</span></span>|<span data-ttu-id="2923a-123">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="2923a-123">Revocation failed.</span></span>|
|<span data-ttu-id="2923a-124">отозван</span><span class="sxs-lookup"><span data-stu-id="2923a-124">revoked</span></span>|<span data-ttu-id="2923a-125">4 </span><span class="sxs-lookup"><span data-stu-id="2923a-125">4</span></span>|<span data-ttu-id="2923a-126">Отозван.</span><span class="sxs-lookup"><span data-stu-id="2923a-126">Revoked.</span></span>|



