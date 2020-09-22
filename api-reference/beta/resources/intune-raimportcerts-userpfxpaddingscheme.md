---
title: тип перечисления Усерпфкспаддингсчеме
description: Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6e0e01c59302593ee329c097c17cd905dfdaaebd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993268"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="a3f11-103">тип перечисления Усерпфкспаддингсчеме</span><span class="sxs-lookup"><span data-stu-id="a3f11-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="a3f11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3f11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3f11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3f11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3f11-107">Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.</span><span class="sxs-lookup"><span data-stu-id="a3f11-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="a3f11-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3f11-108">Members</span></span>
|<span data-ttu-id="a3f11-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3f11-109">Member</span></span>|<span data-ttu-id="a3f11-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a3f11-110">Value</span></span>|<span data-ttu-id="a3f11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f11-112">Нет</span><span class="sxs-lookup"><span data-stu-id="a3f11-112">none</span></span>|<span data-ttu-id="a3f11-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a3f11-113">0</span></span>|<span data-ttu-id="a3f11-114">Неизвестная схема заполнения.</span><span class="sxs-lookup"><span data-stu-id="a3f11-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="a3f11-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="a3f11-115">pkcs1</span></span>|<span data-ttu-id="a3f11-116">1 </span><span class="sxs-lookup"><span data-stu-id="a3f11-116">1</span></span>|<span data-ttu-id="a3f11-117">Pkcs1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3f11-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="a3f11-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="a3f11-118">oaepSha1</span></span>|<span data-ttu-id="a3f11-119">2 </span><span class="sxs-lookup"><span data-stu-id="a3f11-119">2</span></span>|<span data-ttu-id="a3f11-120">OaepSha1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3f11-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="a3f11-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="a3f11-121">oaepSha256</span></span>|<span data-ttu-id="a3f11-122">4</span><span class="sxs-lookup"><span data-stu-id="a3f11-122">3</span></span>|<span data-ttu-id="a3f11-123">Используйте заполнение OAEP SHA – 256.</span><span class="sxs-lookup"><span data-stu-id="a3f11-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="a3f11-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="a3f11-124">oaepSha384</span></span>|<span data-ttu-id="a3f11-125">4 </span><span class="sxs-lookup"><span data-stu-id="a3f11-125">4</span></span>|<span data-ttu-id="a3f11-126">Используйте заполнение OAEP SHA – 384.</span><span class="sxs-lookup"><span data-stu-id="a3f11-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="a3f11-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="a3f11-127">oaepSha512</span></span>|<span data-ttu-id="a3f11-128">5 </span><span class="sxs-lookup"><span data-stu-id="a3f11-128">5</span></span>|<span data-ttu-id="a3f11-129">Используйте заполнение OAEP SHA – 512.</span><span class="sxs-lookup"><span data-stu-id="a3f11-129">Use OAEP SHA-512 padding.</span></span>|






