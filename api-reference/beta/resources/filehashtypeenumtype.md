---
title: Перечисление fileHashType
description: Перечисление для типов файлов хэш-функции.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518382"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="d929f-103">Перечисление fileHashType</span><span class="sxs-lookup"><span data-stu-id="d929f-103">fileHashType enum</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d929f-104">Перечисление для типов файлов хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-104">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="d929f-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="d929f-105">Members</span></span>

|<span data-ttu-id="d929f-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="d929f-106">Member</span></span>|<span data-ttu-id="d929f-107">Значение</span><span class="sxs-lookup"><span data-stu-id="d929f-107">Value</span></span>|<span data-ttu-id="d929f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d929f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d929f-109">unknown</span><span class="sxs-lookup"><span data-stu-id="d929f-109">unknown</span></span>|<span data-ttu-id="d929f-110">(0)</span><span class="sxs-lookup"><span data-stu-id="d929f-110">0</span></span>|<span data-ttu-id="d929f-111">Неизвестный тип.</span><span class="sxs-lookup"><span data-stu-id="d929f-111">Unknown type.</span></span>|
|<span data-ttu-id="d929f-112">SHA1</span><span class="sxs-lookup"><span data-stu-id="d929f-112">sha1</span></span>|<span data-ttu-id="d929f-113">$1</span><span class="sxs-lookup"><span data-stu-id="d929f-113">1</span></span>|<span data-ttu-id="d929f-114">Тип хэш SHA1.</span><span class="sxs-lookup"><span data-stu-id="d929f-114">SHA1 hash type.</span></span>|
|<span data-ttu-id="d929f-115">SHA256</span><span class="sxs-lookup"><span data-stu-id="d929f-115">sha256</span></span>|<span data-ttu-id="d929f-116">–2</span><span class="sxs-lookup"><span data-stu-id="d929f-116">2</span></span>| <span data-ttu-id="d929f-117">Тип SHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-117">SHA256 hash type.</span></span>|
|<span data-ttu-id="d929f-118">MD5</span><span class="sxs-lookup"><span data-stu-id="d929f-118">md5</span></span>|<span data-ttu-id="d929f-119">–3</span><span class="sxs-lookup"><span data-stu-id="d929f-119">3</span></span>| <span data-ttu-id="d929f-120">Тип хэш MD5.</span><span class="sxs-lookup"><span data-stu-id="d929f-120">MD5 hash type.</span></span>|
|<span data-ttu-id="d929f-121">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="d929f-121">authenticodeHash256</span></span>|<span data-ttu-id="d929f-122">4</span><span class="sxs-lookup"><span data-stu-id="d929f-122">4</span></span>| <span data-ttu-id="d929f-123">Тип AuthenticodeHash256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-123">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="d929f-124">lsHash</span><span class="sxs-lookup"><span data-stu-id="d929f-124">lsHash</span></span>|<span data-ttu-id="d929f-125">$-5</span><span class="sxs-lookup"><span data-stu-id="d929f-125">5</span></span>| <span data-ttu-id="d929f-126">Тип LsHash хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-126">LsHash hash type.</span></span>|
|<span data-ttu-id="d929f-127">ctph</span><span class="sxs-lookup"><span data-stu-id="d929f-127">ctph</span></span>|<span data-ttu-id="d929f-128">6</span><span class="sxs-lookup"><span data-stu-id="d929f-128">6</span></span>| <span data-ttu-id="d929f-129">Тип CTPH хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-129">CTPH hash type.</span></span>|
|<span data-ttu-id="d929f-130">peSha1</span><span class="sxs-lookup"><span data-stu-id="d929f-130">peSha1</span></span>|<span data-ttu-id="d929f-131">7</span><span class="sxs-lookup"><span data-stu-id="d929f-131">7</span></span>| <span data-ttu-id="d929f-132">Тип PESHA1 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-132">PESHA1 hash type.</span></span>|
|<span data-ttu-id="d929f-133">peSha256</span><span class="sxs-lookup"><span data-stu-id="d929f-133">peSha256</span></span>|<span data-ttu-id="d929f-134">: = 8</span><span class="sxs-lookup"><span data-stu-id="d929f-134">8</span></span>| <span data-ttu-id="d929f-135">Тип PESHA256 хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="d929f-135">PESHA256 hash type.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
