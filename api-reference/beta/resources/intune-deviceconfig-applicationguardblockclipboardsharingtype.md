---
title: тип перечисления Аппликатионгуардблоккклипбоардшарингтипе
description: Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58c2a30a1dd1bf7e848cd6db702a002731bcaf7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527112"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="c766f-103">тип перечисления Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="c766f-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="c766f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c766f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c766f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c766f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c766f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c766f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c766f-107">Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="c766f-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="c766f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c766f-108">Members</span></span>
|<span data-ttu-id="c766f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c766f-109">Member</span></span>|<span data-ttu-id="c766f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c766f-110">Value</span></span>|<span data-ttu-id="c766f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c766f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c766f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c766f-112">notConfigured</span></span>|<span data-ttu-id="c766f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c766f-113">0</span></span>|<span data-ttu-id="c766f-114">Not Configured</span><span class="sxs-lookup"><span data-stu-id="c766f-114">Not Configured</span></span>|
|<span data-ttu-id="c766f-115">блоккбос</span><span class="sxs-lookup"><span data-stu-id="c766f-115">blockBoth</span></span>|<span data-ttu-id="c766f-116">1 </span><span class="sxs-lookup"><span data-stu-id="c766f-116">1</span></span>|<span data-ttu-id="c766f-117">Блокировка буфера обмена для совместного использования данных из узла в контейнер и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="c766f-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="c766f-118">блоккхосттоконтаинер</span><span class="sxs-lookup"><span data-stu-id="c766f-118">blockHostToContainer</span></span>|<span data-ttu-id="c766f-119">2 </span><span class="sxs-lookup"><span data-stu-id="c766f-119">2</span></span>|<span data-ttu-id="c766f-120">Блокировка буфера обмена для предоставления общего доступа к данным из узла в контейнер</span><span class="sxs-lookup"><span data-stu-id="c766f-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="c766f-121">блоккконтаинертохост</span><span class="sxs-lookup"><span data-stu-id="c766f-121">blockContainerToHost</span></span>|<span data-ttu-id="c766f-122">3 </span><span class="sxs-lookup"><span data-stu-id="c766f-122">3</span></span>|<span data-ttu-id="c766f-123">Блокировка буфера обмена для предоставления общего доступа к данным из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="c766f-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="c766f-124">блоккноне</span><span class="sxs-lookup"><span data-stu-id="c766f-124">blockNone</span></span>|<span data-ttu-id="c766f-125">4 </span><span class="sxs-lookup"><span data-stu-id="c766f-125">4</span></span>|<span data-ttu-id="c766f-126">Блокировка буфера обмена для совместного использования данных без размещения в контейнере и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="c766f-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



