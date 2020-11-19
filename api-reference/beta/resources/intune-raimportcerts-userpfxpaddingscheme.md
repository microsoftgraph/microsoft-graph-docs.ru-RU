---
title: тип перечисления Усерпфкспаддингсчеме
description: Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0cbdc056c1dc0ea1aa73ae0cd96af428ce9f2bf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307172"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="fe90b-103">тип перечисления Усерпфкспаддингсчеме</span><span class="sxs-lookup"><span data-stu-id="fe90b-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="fe90b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe90b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe90b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe90b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe90b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe90b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe90b-107">Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.</span><span class="sxs-lookup"><span data-stu-id="fe90b-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="fe90b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fe90b-108">Members</span></span>
|<span data-ttu-id="fe90b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fe90b-109">Member</span></span>|<span data-ttu-id="fe90b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fe90b-110">Value</span></span>|<span data-ttu-id="fe90b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe90b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe90b-112">Нет</span><span class="sxs-lookup"><span data-stu-id="fe90b-112">none</span></span>|<span data-ttu-id="fe90b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fe90b-113">0</span></span>|<span data-ttu-id="fe90b-114">Неизвестная схема заполнения.</span><span class="sxs-lookup"><span data-stu-id="fe90b-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="fe90b-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="fe90b-115">pkcs1</span></span>|<span data-ttu-id="fe90b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="fe90b-116">1</span></span>|<span data-ttu-id="fe90b-117">Pkcs1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fe90b-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="fe90b-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="fe90b-118">oaepSha1</span></span>|<span data-ttu-id="fe90b-119">2</span><span class="sxs-lookup"><span data-stu-id="fe90b-119">2</span></span>|<span data-ttu-id="fe90b-120">OaepSha1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fe90b-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="fe90b-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="fe90b-121">oaepSha256</span></span>|<span data-ttu-id="fe90b-122">4</span><span class="sxs-lookup"><span data-stu-id="fe90b-122">3</span></span>|<span data-ttu-id="fe90b-123">Используйте заполнение OAEP SHA – 256.</span><span class="sxs-lookup"><span data-stu-id="fe90b-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="fe90b-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="fe90b-124">oaepSha384</span></span>|<span data-ttu-id="fe90b-125">4 </span><span class="sxs-lookup"><span data-stu-id="fe90b-125">4</span></span>|<span data-ttu-id="fe90b-126">Используйте заполнение OAEP SHA – 384.</span><span class="sxs-lookup"><span data-stu-id="fe90b-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="fe90b-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="fe90b-127">oaepSha512</span></span>|<span data-ttu-id="fe90b-128">5 </span><span class="sxs-lookup"><span data-stu-id="fe90b-128">5</span></span>|<span data-ttu-id="fe90b-129">Используйте заполнение OAEP SHA – 512.</span><span class="sxs-lookup"><span data-stu-id="fe90b-129">Use OAEP SHA-512 padding.</span></span>|




