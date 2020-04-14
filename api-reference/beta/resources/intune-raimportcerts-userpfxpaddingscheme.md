---
title: тип перечисления Усерпфкспаддингсчеме
description: Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3e96dc40ca742c802a1b2bc88e05a708202648bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467720"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="5c9f4-103">тип перечисления Усерпфкспаддингсчеме</span><span class="sxs-lookup"><span data-stu-id="5c9f4-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="5c9f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c9f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c9f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c9f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c9f4-107">Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="5c9f4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c9f4-108">Members</span></span>
|<span data-ttu-id="5c9f4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c9f4-109">Member</span></span>|<span data-ttu-id="5c9f4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5c9f4-110">Value</span></span>|<span data-ttu-id="5c9f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c9f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c9f4-112">нет</span><span class="sxs-lookup"><span data-stu-id="5c9f4-112">none</span></span>|<span data-ttu-id="5c9f4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5c9f4-113">0</span></span>|<span data-ttu-id="5c9f4-114">Неизвестная схема заполнения.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="5c9f4-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="5c9f4-115">pkcs1</span></span>|<span data-ttu-id="5c9f4-116">1,1</span><span class="sxs-lookup"><span data-stu-id="5c9f4-116">1</span></span>|<span data-ttu-id="5c9f4-117">Pkcs1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5c9f4-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="5c9f4-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="5c9f4-118">oaepSha1</span></span>|<span data-ttu-id="5c9f4-119">2</span><span class="sxs-lookup"><span data-stu-id="5c9f4-119">2</span></span>|<span data-ttu-id="5c9f4-120">OaepSha1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5c9f4-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="5c9f4-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="5c9f4-121">oaepSha256</span></span>|<span data-ttu-id="5c9f4-122">4</span><span class="sxs-lookup"><span data-stu-id="5c9f4-122">3</span></span>|<span data-ttu-id="5c9f4-123">Используйте заполнение OAEP SHA – 256.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="5c9f4-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="5c9f4-124">oaepSha384</span></span>|<span data-ttu-id="5c9f4-125">4 </span><span class="sxs-lookup"><span data-stu-id="5c9f4-125">4</span></span>|<span data-ttu-id="5c9f4-126">Используйте заполнение OAEP SHA – 384.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="5c9f4-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="5c9f4-127">oaepSha512</span></span>|<span data-ttu-id="5c9f4-128">5 </span><span class="sxs-lookup"><span data-stu-id="5c9f4-128">5</span></span>|<span data-ttu-id="5c9f4-129">Используйте заполнение OAEP SHA – 512.</span><span class="sxs-lookup"><span data-stu-id="5c9f4-129">Use OAEP SHA-512 padding.</span></span>|



