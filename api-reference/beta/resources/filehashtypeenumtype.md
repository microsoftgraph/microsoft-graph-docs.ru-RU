---
title: Перечисление fileHashType
description: Перечисление для типов файлов хэш-функции.
ms.openlocfilehash: fbaa390ee8c543d2ed7c77cc05a11b519df0da9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075507"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="0ae6d-103">Перечисление fileHashType</span><span class="sxs-lookup"><span data-stu-id="0ae6d-103">fileHashType enum</span></span>

> <span data-ttu-id="0ae6d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ae6d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ae6d-106">Перечисление для типов файлов хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="0ae6d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0ae6d-107">Members</span></span>

|<span data-ttu-id="0ae6d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0ae6d-108">Member</span></span>|<span data-ttu-id="0ae6d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0ae6d-109">Value</span></span>|<span data-ttu-id="0ae6d-110">Description</span><span class="sxs-lookup"><span data-stu-id="0ae6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae6d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="0ae6d-111">unknown</span></span>|<span data-ttu-id="0ae6d-112">0</span><span class="sxs-lookup"><span data-stu-id="0ae6d-112">0</span></span>|<span data-ttu-id="0ae6d-113">Неизвестный тип.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-113">Unknown type.</span></span>|
|<span data-ttu-id="0ae6d-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="0ae6d-114">sha1</span></span>|<span data-ttu-id="0ae6d-115">1</span><span class="sxs-lookup"><span data-stu-id="0ae6d-115">1</span></span>|<span data-ttu-id="0ae6d-116">Тип хэш SHA1.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="0ae6d-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="0ae6d-117">sha256</span></span>|<span data-ttu-id="0ae6d-118">2</span><span class="sxs-lookup"><span data-stu-id="0ae6d-118">2</span></span>| <span data-ttu-id="0ae6d-119">Тип SHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="0ae6d-120">MD5</span><span class="sxs-lookup"><span data-stu-id="0ae6d-120">md5</span></span>|<span data-ttu-id="0ae6d-121">3</span><span class="sxs-lookup"><span data-stu-id="0ae6d-121">3</span></span>| <span data-ttu-id="0ae6d-122">Тип хэш MD5.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-122">MD5 hash type.</span></span>|
|<span data-ttu-id="0ae6d-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="0ae6d-123">authenticodeHash256</span></span>|<span data-ttu-id="0ae6d-124">4</span><span class="sxs-lookup"><span data-stu-id="0ae6d-124">4</span></span>| <span data-ttu-id="0ae6d-125">Тип AuthenticodeHash256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="0ae6d-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="0ae6d-126">lsHash</span></span>|<span data-ttu-id="0ae6d-127">5</span><span class="sxs-lookup"><span data-stu-id="0ae6d-127">5</span></span>| <span data-ttu-id="0ae6d-128">Тип LsHash хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-128">LsHash hash type.</span></span>|
|<span data-ttu-id="0ae6d-129">ctph</span><span class="sxs-lookup"><span data-stu-id="0ae6d-129">ctph</span></span>|<span data-ttu-id="0ae6d-130">6</span><span class="sxs-lookup"><span data-stu-id="0ae6d-130">6</span></span>| <span data-ttu-id="0ae6d-131">Тип CTPH хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-131">CTPH hash type.</span></span>|
|<span data-ttu-id="0ae6d-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="0ae6d-132">peSha1</span></span>|<span data-ttu-id="0ae6d-133">7</span><span class="sxs-lookup"><span data-stu-id="0ae6d-133">7</span></span>| <span data-ttu-id="0ae6d-134">Тип PESHA1 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="0ae6d-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="0ae6d-135">peSha256</span></span>|<span data-ttu-id="0ae6d-136">8</span><span class="sxs-lookup"><span data-stu-id="0ae6d-136">8</span></span>| <span data-ttu-id="0ae6d-137">Тип PESHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="0ae6d-137">PESHA256 hash type.</span></span>|
