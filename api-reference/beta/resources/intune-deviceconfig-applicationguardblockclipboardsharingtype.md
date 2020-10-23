---
title: тип перечисления Аппликатионгуардблоккклипбоардшарингтипе
description: Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d8aa4e34a9be5a3d2c3c9d8b0fa59635b7c16c6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708888"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="92469-103">тип перечисления Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="92469-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="92469-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92469-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92469-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92469-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92469-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92469-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92469-107">Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="92469-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="92469-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="92469-108">Members</span></span>
|<span data-ttu-id="92469-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="92469-109">Member</span></span>|<span data-ttu-id="92469-110">Значение</span><span class="sxs-lookup"><span data-stu-id="92469-110">Value</span></span>|<span data-ttu-id="92469-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92469-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92469-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="92469-112">notConfigured</span></span>|<span data-ttu-id="92469-113">нуль</span><span class="sxs-lookup"><span data-stu-id="92469-113">0</span></span>|<span data-ttu-id="92469-114">Not Configured</span><span class="sxs-lookup"><span data-stu-id="92469-114">Not Configured</span></span>|
|<span data-ttu-id="92469-115">блоккбос</span><span class="sxs-lookup"><span data-stu-id="92469-115">blockBoth</span></span>|<span data-ttu-id="92469-116">1,1</span><span class="sxs-lookup"><span data-stu-id="92469-116">1</span></span>|<span data-ttu-id="92469-117">Блокировка буфера обмена для совместного использования данных из узла в контейнер и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="92469-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="92469-118">блоккхосттоконтаинер</span><span class="sxs-lookup"><span data-stu-id="92469-118">blockHostToContainer</span></span>|<span data-ttu-id="92469-119">2</span><span class="sxs-lookup"><span data-stu-id="92469-119">2</span></span>|<span data-ttu-id="92469-120">Блокировка буфера обмена для предоставления общего доступа к данным из узла в контейнер</span><span class="sxs-lookup"><span data-stu-id="92469-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="92469-121">блоккконтаинертохост</span><span class="sxs-lookup"><span data-stu-id="92469-121">blockContainerToHost</span></span>|<span data-ttu-id="92469-122">4</span><span class="sxs-lookup"><span data-stu-id="92469-122">3</span></span>|<span data-ttu-id="92469-123">Блокировка буфера обмена для предоставления общего доступа к данным из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="92469-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="92469-124">блоккноне</span><span class="sxs-lookup"><span data-stu-id="92469-124">blockNone</span></span>|<span data-ttu-id="92469-125">4 </span><span class="sxs-lookup"><span data-stu-id="92469-125">4</span></span>|<span data-ttu-id="92469-126">Блокировка буфера обмена для совместного использования данных без размещения в контейнере и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="92469-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





