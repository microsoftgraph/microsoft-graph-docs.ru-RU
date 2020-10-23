---
title: тип перечисления Усерпфкспаддингсчеме
description: Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 676bd1b99a2dd18e06dbd451d478c8db4cf2c131
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697219"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="7778d-103">тип перечисления Усерпфкспаддингсчеме</span><span class="sxs-lookup"><span data-stu-id="7778d-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="7778d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7778d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7778d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7778d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7778d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7778d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7778d-107">Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.</span><span class="sxs-lookup"><span data-stu-id="7778d-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="7778d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7778d-108">Members</span></span>
|<span data-ttu-id="7778d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7778d-109">Member</span></span>|<span data-ttu-id="7778d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7778d-110">Value</span></span>|<span data-ttu-id="7778d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7778d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7778d-112">none</span><span class="sxs-lookup"><span data-stu-id="7778d-112">none</span></span>|<span data-ttu-id="7778d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7778d-113">0</span></span>|<span data-ttu-id="7778d-114">Неизвестная схема заполнения.</span><span class="sxs-lookup"><span data-stu-id="7778d-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="7778d-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="7778d-115">pkcs1</span></span>|<span data-ttu-id="7778d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="7778d-116">1</span></span>|<span data-ttu-id="7778d-117">Pkcs1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7778d-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="7778d-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="7778d-118">oaepSha1</span></span>|<span data-ttu-id="7778d-119">2</span><span class="sxs-lookup"><span data-stu-id="7778d-119">2</span></span>|<span data-ttu-id="7778d-120">OaepSha1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7778d-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="7778d-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="7778d-121">oaepSha256</span></span>|<span data-ttu-id="7778d-122">4</span><span class="sxs-lookup"><span data-stu-id="7778d-122">3</span></span>|<span data-ttu-id="7778d-123">Используйте заполнение OAEP SHA – 256.</span><span class="sxs-lookup"><span data-stu-id="7778d-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="7778d-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="7778d-124">oaepSha384</span></span>|<span data-ttu-id="7778d-125">4 </span><span class="sxs-lookup"><span data-stu-id="7778d-125">4</span></span>|<span data-ttu-id="7778d-126">Используйте заполнение OAEP SHA – 384.</span><span class="sxs-lookup"><span data-stu-id="7778d-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="7778d-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="7778d-127">oaepSha512</span></span>|<span data-ttu-id="7778d-128">5 </span><span class="sxs-lookup"><span data-stu-id="7778d-128">5</span></span>|<span data-ttu-id="7778d-129">Используйте заполнение OAEP SHA – 512.</span><span class="sxs-lookup"><span data-stu-id="7778d-129">Use OAEP SHA-512 padding.</span></span>|





