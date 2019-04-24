---
title: Перечисление Филехаштипе
description: Enum для типов хэша файлов.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506372"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="fc761-103">Перечисление Филехаштипе</span><span class="sxs-lookup"><span data-stu-id="fc761-103">fileHashType enum</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc761-104">Enum для типов хэша файлов.</span><span class="sxs-lookup"><span data-stu-id="fc761-104">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="fc761-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="fc761-105">Members</span></span>

|<span data-ttu-id="fc761-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="fc761-106">Member</span></span>|<span data-ttu-id="fc761-107">Значение</span><span class="sxs-lookup"><span data-stu-id="fc761-107">Value</span></span>|<span data-ttu-id="fc761-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc761-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc761-109">unknown</span><span class="sxs-lookup"><span data-stu-id="fc761-109">unknown</span></span>|<span data-ttu-id="fc761-110">нуль</span><span class="sxs-lookup"><span data-stu-id="fc761-110">0</span></span>|<span data-ttu-id="fc761-111">НеИзвестный тип.</span><span class="sxs-lookup"><span data-stu-id="fc761-111">Unknown type.</span></span>|
|<span data-ttu-id="fc761-112">хэшем</span><span class="sxs-lookup"><span data-stu-id="fc761-112">sha1</span></span>|<span data-ttu-id="fc761-113">1 </span><span class="sxs-lookup"><span data-stu-id="fc761-113">1</span></span>|<span data-ttu-id="fc761-114">Тип хеша SHA1.</span><span class="sxs-lookup"><span data-stu-id="fc761-114">SHA1 hash type.</span></span>|
|<span data-ttu-id="fc761-115">хэш</span><span class="sxs-lookup"><span data-stu-id="fc761-115">sha256</span></span>|<span data-ttu-id="fc761-116">2 </span><span class="sxs-lookup"><span data-stu-id="fc761-116">2</span></span>| <span data-ttu-id="fc761-117">Тип хеша SHA256.</span><span class="sxs-lookup"><span data-stu-id="fc761-117">SHA256 hash type.</span></span>|
|<span data-ttu-id="fc761-118">алгоритм</span><span class="sxs-lookup"><span data-stu-id="fc761-118">md5</span></span>|<span data-ttu-id="fc761-119">3 </span><span class="sxs-lookup"><span data-stu-id="fc761-119">3</span></span>| <span data-ttu-id="fc761-120">Тип хеша MD5.</span><span class="sxs-lookup"><span data-stu-id="fc761-120">MD5 hash type.</span></span>|
|<span data-ttu-id="fc761-121">Свойства authenticodehash256</span><span class="sxs-lookup"><span data-stu-id="fc761-121">authenticodeHash256</span></span>|<span data-ttu-id="fc761-122">4 </span><span class="sxs-lookup"><span data-stu-id="fc761-122">4</span></span>| <span data-ttu-id="fc761-123">Тип хеша свойства authenticodehash256.</span><span class="sxs-lookup"><span data-stu-id="fc761-123">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="fc761-124">Лшаш</span><span class="sxs-lookup"><span data-stu-id="fc761-124">lsHash</span></span>|<span data-ttu-id="fc761-125">5 </span><span class="sxs-lookup"><span data-stu-id="fc761-125">5</span></span>| <span data-ttu-id="fc761-126">Тип хеша Лшаш.</span><span class="sxs-lookup"><span data-stu-id="fc761-126">LsHash hash type.</span></span>|
|<span data-ttu-id="fc761-127">КТФ</span><span class="sxs-lookup"><span data-stu-id="fc761-127">ctph</span></span>|<span data-ttu-id="fc761-128">6 </span><span class="sxs-lookup"><span data-stu-id="fc761-128">6</span></span>| <span data-ttu-id="fc761-129">Тип хеша КТФ.</span><span class="sxs-lookup"><span data-stu-id="fc761-129">CTPH hash type.</span></span>|
|<span data-ttu-id="fc761-130">peSha1</span><span class="sxs-lookup"><span data-stu-id="fc761-130">peSha1</span></span>|<span data-ttu-id="fc761-131">7 </span><span class="sxs-lookup"><span data-stu-id="fc761-131">7</span></span>| <span data-ttu-id="fc761-132">Тип хеша PESHA1.</span><span class="sxs-lookup"><span data-stu-id="fc761-132">PESHA1 hash type.</span></span>|
|<span data-ttu-id="fc761-133">peSha256</span><span class="sxs-lookup"><span data-stu-id="fc761-133">peSha256</span></span>|<span data-ttu-id="fc761-134">8 </span><span class="sxs-lookup"><span data-stu-id="fc761-134">8</span></span>| <span data-ttu-id="fc761-135">Тип хеша PESHA256.</span><span class="sxs-lookup"><span data-stu-id="fc761-135">PESHA256 hash type.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
