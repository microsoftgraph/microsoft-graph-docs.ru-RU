---
title: Перечисление Филехаштипе
description: Enum для типов хэша файлов.
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c8f2b733363ecbd79a885a0b76c170f076664590
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498226"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="59a6d-103">Перечисление Филехаштипе</span><span class="sxs-lookup"><span data-stu-id="59a6d-103">fileHashType enum</span></span>

<span data-ttu-id="59a6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59a6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59a6d-105">Enum для типов хэша файлов.</span><span class="sxs-lookup"><span data-stu-id="59a6d-105">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="59a6d-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="59a6d-106">Members</span></span>

|<span data-ttu-id="59a6d-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="59a6d-107">Member</span></span>|<span data-ttu-id="59a6d-108">Значение</span><span class="sxs-lookup"><span data-stu-id="59a6d-108">Value</span></span>|<span data-ttu-id="59a6d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59a6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a6d-110">unknown</span><span class="sxs-lookup"><span data-stu-id="59a6d-110">unknown</span></span>|<span data-ttu-id="59a6d-111">нуль</span><span class="sxs-lookup"><span data-stu-id="59a6d-111">0</span></span>|<span data-ttu-id="59a6d-112">Неизвестный тип.</span><span class="sxs-lookup"><span data-stu-id="59a6d-112">Unknown type.</span></span>|
|<span data-ttu-id="59a6d-113">хэшем</span><span class="sxs-lookup"><span data-stu-id="59a6d-113">sha1</span></span>|<span data-ttu-id="59a6d-114">1,1</span><span class="sxs-lookup"><span data-stu-id="59a6d-114">1</span></span>|<span data-ttu-id="59a6d-115">Тип хеша SHA1.</span><span class="sxs-lookup"><span data-stu-id="59a6d-115">SHA1 hash type.</span></span>|
|<span data-ttu-id="59a6d-116">хэш</span><span class="sxs-lookup"><span data-stu-id="59a6d-116">sha256</span></span>|<span data-ttu-id="59a6d-117">2</span><span class="sxs-lookup"><span data-stu-id="59a6d-117">2</span></span>| <span data-ttu-id="59a6d-118">Тип хеша SHA256.</span><span class="sxs-lookup"><span data-stu-id="59a6d-118">SHA256 hash type.</span></span>|
|<span data-ttu-id="59a6d-119">алгоритм</span><span class="sxs-lookup"><span data-stu-id="59a6d-119">md5</span></span>|<span data-ttu-id="59a6d-120">4</span><span class="sxs-lookup"><span data-stu-id="59a6d-120">3</span></span>| <span data-ttu-id="59a6d-121">Тип хеша MD5.</span><span class="sxs-lookup"><span data-stu-id="59a6d-121">MD5 hash type.</span></span>|
|<span data-ttu-id="59a6d-122">Свойства authenticodehash256</span><span class="sxs-lookup"><span data-stu-id="59a6d-122">authenticodeHash256</span></span>|<span data-ttu-id="59a6d-123">4 </span><span class="sxs-lookup"><span data-stu-id="59a6d-123">4</span></span>| <span data-ttu-id="59a6d-124">Тип хеша свойства authenticodehash256.</span><span class="sxs-lookup"><span data-stu-id="59a6d-124">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="59a6d-125">лшаш</span><span class="sxs-lookup"><span data-stu-id="59a6d-125">lsHash</span></span>|<span data-ttu-id="59a6d-126">5 </span><span class="sxs-lookup"><span data-stu-id="59a6d-126">5</span></span>| <span data-ttu-id="59a6d-127">Тип хеша Лшаш.</span><span class="sxs-lookup"><span data-stu-id="59a6d-127">LsHash hash type.</span></span>|
|<span data-ttu-id="59a6d-128">ктф</span><span class="sxs-lookup"><span data-stu-id="59a6d-128">ctph</span></span>|<span data-ttu-id="59a6d-129">6 </span><span class="sxs-lookup"><span data-stu-id="59a6d-129">6</span></span>| <span data-ttu-id="59a6d-130">Тип хеша КТФ.</span><span class="sxs-lookup"><span data-stu-id="59a6d-130">CTPH hash type.</span></span>|
|<span data-ttu-id="59a6d-131">peSha1</span><span class="sxs-lookup"><span data-stu-id="59a6d-131">peSha1</span></span>|<span data-ttu-id="59a6d-132">7 </span><span class="sxs-lookup"><span data-stu-id="59a6d-132">7</span></span>| <span data-ttu-id="59a6d-133">Тип хеша PESHA1.</span><span class="sxs-lookup"><span data-stu-id="59a6d-133">PESHA1 hash type.</span></span>|
|<span data-ttu-id="59a6d-134">peSha256</span><span class="sxs-lookup"><span data-stu-id="59a6d-134">peSha256</span></span>|<span data-ttu-id="59a6d-135">8 </span><span class="sxs-lookup"><span data-stu-id="59a6d-135">8</span></span>| <span data-ttu-id="59a6d-136">Тип хеша PESHA256.</span><span class="sxs-lookup"><span data-stu-id="59a6d-136">PESHA256 hash type.</span></span>|
