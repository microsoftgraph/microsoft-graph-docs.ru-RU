---
title: Перечисление fileHashType
description: Перечисление для типов файлов хэш-функции.
localization_priority: Normal
ms.openlocfilehash: e1c31aaea6c8cea40817efea61dc8654d3d17fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816333"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="9e551-103">Перечисление fileHashType</span><span class="sxs-lookup"><span data-stu-id="9e551-103">fileHashType enum</span></span>

> <span data-ttu-id="9e551-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e551-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e551-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e551-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e551-106">Перечисление для типов файлов хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="9e551-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9e551-107">Members</span></span>

|<span data-ttu-id="9e551-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9e551-108">Member</span></span>|<span data-ttu-id="9e551-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9e551-109">Value</span></span>|<span data-ttu-id="9e551-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e551-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e551-111">unknown</span><span class="sxs-lookup"><span data-stu-id="9e551-111">unknown</span></span>|<span data-ttu-id="9e551-112">0</span><span class="sxs-lookup"><span data-stu-id="9e551-112">0</span></span>|<span data-ttu-id="9e551-113">Неизвестный тип.</span><span class="sxs-lookup"><span data-stu-id="9e551-113">Unknown type.</span></span>|
|<span data-ttu-id="9e551-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="9e551-114">sha1</span></span>|<span data-ttu-id="9e551-115">1</span><span class="sxs-lookup"><span data-stu-id="9e551-115">1</span></span>|<span data-ttu-id="9e551-116">Тип хэш SHA1.</span><span class="sxs-lookup"><span data-stu-id="9e551-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="9e551-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="9e551-117">sha256</span></span>|<span data-ttu-id="9e551-118">2</span><span class="sxs-lookup"><span data-stu-id="9e551-118">2</span></span>| <span data-ttu-id="9e551-119">Тип SHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="9e551-120">MD5</span><span class="sxs-lookup"><span data-stu-id="9e551-120">md5</span></span>|<span data-ttu-id="9e551-121">3</span><span class="sxs-lookup"><span data-stu-id="9e551-121">3</span></span>| <span data-ttu-id="9e551-122">Тип хэш MD5.</span><span class="sxs-lookup"><span data-stu-id="9e551-122">MD5 hash type.</span></span>|
|<span data-ttu-id="9e551-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="9e551-123">authenticodeHash256</span></span>|<span data-ttu-id="9e551-124">4</span><span class="sxs-lookup"><span data-stu-id="9e551-124">4</span></span>| <span data-ttu-id="9e551-125">Тип AuthenticodeHash256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="9e551-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="9e551-126">lsHash</span></span>|<span data-ttu-id="9e551-127">5</span><span class="sxs-lookup"><span data-stu-id="9e551-127">5</span></span>| <span data-ttu-id="9e551-128">Тип LsHash хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-128">LsHash hash type.</span></span>|
|<span data-ttu-id="9e551-129">ctph</span><span class="sxs-lookup"><span data-stu-id="9e551-129">ctph</span></span>|<span data-ttu-id="9e551-130">6</span><span class="sxs-lookup"><span data-stu-id="9e551-130">6</span></span>| <span data-ttu-id="9e551-131">Тип CTPH хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-131">CTPH hash type.</span></span>|
|<span data-ttu-id="9e551-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="9e551-132">peSha1</span></span>|<span data-ttu-id="9e551-133">7</span><span class="sxs-lookup"><span data-stu-id="9e551-133">7</span></span>| <span data-ttu-id="9e551-134">Тип PESHA1 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="9e551-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="9e551-135">peSha256</span></span>|<span data-ttu-id="9e551-136">8</span><span class="sxs-lookup"><span data-stu-id="9e551-136">8</span></span>| <span data-ttu-id="9e551-137">Тип PESHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="9e551-137">PESHA256 hash type.</span></span>|
