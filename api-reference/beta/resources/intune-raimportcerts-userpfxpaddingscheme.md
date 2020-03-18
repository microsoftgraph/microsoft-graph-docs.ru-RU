---
title: тип перечисления Усерпфкспаддингсчеме
description: Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 73cd96dcc01a99df657ca7f538046c7e5e7ed4a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42774227"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="3d378-103">тип перечисления Усерпфкспаддингсчеме</span><span class="sxs-lookup"><span data-stu-id="3d378-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="3d378-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d378-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d378-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d378-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d378-106">Поддерживаемые значения для схемы заполнения, используемой поставщиком шифрования.</span><span class="sxs-lookup"><span data-stu-id="3d378-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="3d378-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3d378-107">Members</span></span>
|<span data-ttu-id="3d378-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3d378-108">Member</span></span>|<span data-ttu-id="3d378-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3d378-109">Value</span></span>|<span data-ttu-id="3d378-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3d378-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d378-111">none</span><span class="sxs-lookup"><span data-stu-id="3d378-111">none</span></span>|<span data-ttu-id="3d378-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3d378-112">0</span></span>|<span data-ttu-id="3d378-113">Неизвестная схема заполнения.</span><span class="sxs-lookup"><span data-stu-id="3d378-113">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="3d378-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="3d378-114">pkcs1</span></span>|<span data-ttu-id="3d378-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3d378-115">1</span></span>|<span data-ttu-id="3d378-116">Pkcs1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3d378-116">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="3d378-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="3d378-117">oaepSha1</span></span>|<span data-ttu-id="3d378-118">2</span><span class="sxs-lookup"><span data-stu-id="3d378-118">2</span></span>|<span data-ttu-id="3d378-119">OaepSha1 больше не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3d378-119">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="3d378-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="3d378-120">oaepSha256</span></span>|<span data-ttu-id="3d378-121">4</span><span class="sxs-lookup"><span data-stu-id="3d378-121">3</span></span>|<span data-ttu-id="3d378-122">Используйте заполнение OAEP SHA – 256.</span><span class="sxs-lookup"><span data-stu-id="3d378-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="3d378-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="3d378-123">oaepSha384</span></span>|<span data-ttu-id="3d378-124">4 </span><span class="sxs-lookup"><span data-stu-id="3d378-124">4</span></span>|<span data-ttu-id="3d378-125">Используйте заполнение OAEP SHA – 384.</span><span class="sxs-lookup"><span data-stu-id="3d378-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="3d378-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="3d378-126">oaepSha512</span></span>|<span data-ttu-id="3d378-127">5 </span><span class="sxs-lookup"><span data-stu-id="3d378-127">5</span></span>|<span data-ttu-id="3d378-128">Используйте заполнение OAEP SHA – 512.</span><span class="sxs-lookup"><span data-stu-id="3d378-128">Use OAEP SHA-512 padding.</span></span>|



