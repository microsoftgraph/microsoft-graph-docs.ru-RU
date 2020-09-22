---
title: Перечисление Филехаштипе
description: Enum для типов хэша файлов.
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: ab94fec4d4a8f6940b7c2bfccc61d38d9fe66887
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076388"
---
# <a name="filehashtype-enum-type"></a><span data-ttu-id="0de57-103">тип перечисления Филехаштипе</span><span class="sxs-lookup"><span data-stu-id="0de57-103">fileHashType enum type</span></span>

<span data-ttu-id="0de57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0de57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0de57-105">Enum для типов хэша файлов.</span><span class="sxs-lookup"><span data-stu-id="0de57-105">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="0de57-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="0de57-106">Members</span></span>

|<span data-ttu-id="0de57-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="0de57-107">Member</span></span>|<span data-ttu-id="0de57-108">Значение</span><span class="sxs-lookup"><span data-stu-id="0de57-108">Value</span></span>|<span data-ttu-id="0de57-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0de57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de57-110">unknown</span><span class="sxs-lookup"><span data-stu-id="0de57-110">unknown</span></span>|<span data-ttu-id="0de57-111">нуль</span><span class="sxs-lookup"><span data-stu-id="0de57-111">0</span></span>|<span data-ttu-id="0de57-112">Неизвестный тип.</span><span class="sxs-lookup"><span data-stu-id="0de57-112">Unknown type.</span></span>|
|<span data-ttu-id="0de57-113">хэшем</span><span class="sxs-lookup"><span data-stu-id="0de57-113">sha1</span></span>|<span data-ttu-id="0de57-114">1 </span><span class="sxs-lookup"><span data-stu-id="0de57-114">1</span></span>|<span data-ttu-id="0de57-115">Тип хеша SHA1.</span><span class="sxs-lookup"><span data-stu-id="0de57-115">SHA1 hash type.</span></span>|
|<span data-ttu-id="0de57-116">хэш</span><span class="sxs-lookup"><span data-stu-id="0de57-116">sha256</span></span>|<span data-ttu-id="0de57-117">2 </span><span class="sxs-lookup"><span data-stu-id="0de57-117">2</span></span>| <span data-ttu-id="0de57-118">Тип хеша SHA256.</span><span class="sxs-lookup"><span data-stu-id="0de57-118">SHA256 hash type.</span></span>|
|<span data-ttu-id="0de57-119">алгоритм</span><span class="sxs-lookup"><span data-stu-id="0de57-119">md5</span></span>|<span data-ttu-id="0de57-120">4</span><span class="sxs-lookup"><span data-stu-id="0de57-120">3</span></span>| <span data-ttu-id="0de57-121">Тип хеша MD5.</span><span class="sxs-lookup"><span data-stu-id="0de57-121">MD5 hash type.</span></span>|
|<span data-ttu-id="0de57-122">Свойства authenticodehash256</span><span class="sxs-lookup"><span data-stu-id="0de57-122">authenticodeHash256</span></span>|<span data-ttu-id="0de57-123">4 </span><span class="sxs-lookup"><span data-stu-id="0de57-123">4</span></span>| <span data-ttu-id="0de57-124">Тип хеша свойства authenticodehash256.</span><span class="sxs-lookup"><span data-stu-id="0de57-124">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="0de57-125">лшаш</span><span class="sxs-lookup"><span data-stu-id="0de57-125">lsHash</span></span>|<span data-ttu-id="0de57-126">5 </span><span class="sxs-lookup"><span data-stu-id="0de57-126">5</span></span>| <span data-ttu-id="0de57-127">Тип хеша Лшаш.</span><span class="sxs-lookup"><span data-stu-id="0de57-127">LsHash hash type.</span></span>|
|<span data-ttu-id="0de57-128">ктф</span><span class="sxs-lookup"><span data-stu-id="0de57-128">ctph</span></span>|<span data-ttu-id="0de57-129">6 </span><span class="sxs-lookup"><span data-stu-id="0de57-129">6</span></span>| <span data-ttu-id="0de57-130">Тип хеша КТФ.</span><span class="sxs-lookup"><span data-stu-id="0de57-130">CTPH hash type.</span></span>|
|<span data-ttu-id="0de57-131">peSha1</span><span class="sxs-lookup"><span data-stu-id="0de57-131">peSha1</span></span>|<span data-ttu-id="0de57-132">7 </span><span class="sxs-lookup"><span data-stu-id="0de57-132">7</span></span>| <span data-ttu-id="0de57-133">Тип хеша PESHA1.</span><span class="sxs-lookup"><span data-stu-id="0de57-133">PESHA1 hash type.</span></span>|
|<span data-ttu-id="0de57-134">peSha256</span><span class="sxs-lookup"><span data-stu-id="0de57-134">peSha256</span></span>|<span data-ttu-id="0de57-135">8 </span><span class="sxs-lookup"><span data-stu-id="0de57-135">8</span></span>| <span data-ttu-id="0de57-136">Тип хеша PESHA256.</span><span class="sxs-lookup"><span data-stu-id="0de57-136">PESHA256 hash type.</span></span>|


