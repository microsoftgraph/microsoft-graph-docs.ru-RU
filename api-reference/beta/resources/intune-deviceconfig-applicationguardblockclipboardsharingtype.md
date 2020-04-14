---
title: тип перечисления Аппликатионгуардблоккклипбоардшарингтипе
description: Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ebf56c4dc7e31a4c6a70e808c6f7f35aaaf9181d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470022"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="71098-103">тип перечисления Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="71098-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="71098-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71098-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71098-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71098-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71098-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71098-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71098-107">Возможные значения для Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="71098-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="71098-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="71098-108">Members</span></span>
|<span data-ttu-id="71098-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="71098-109">Member</span></span>|<span data-ttu-id="71098-110">Значение</span><span class="sxs-lookup"><span data-stu-id="71098-110">Value</span></span>|<span data-ttu-id="71098-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71098-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71098-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="71098-112">notConfigured</span></span>|<span data-ttu-id="71098-113">нуль</span><span class="sxs-lookup"><span data-stu-id="71098-113">0</span></span>|<span data-ttu-id="71098-114">Not Configured</span><span class="sxs-lookup"><span data-stu-id="71098-114">Not Configured</span></span>|
|<span data-ttu-id="71098-115">блоккбос</span><span class="sxs-lookup"><span data-stu-id="71098-115">blockBoth</span></span>|<span data-ttu-id="71098-116">1,1</span><span class="sxs-lookup"><span data-stu-id="71098-116">1</span></span>|<span data-ttu-id="71098-117">Блокировка буфера обмена для совместного использования данных из узла в контейнер и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="71098-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="71098-118">блоккхосттоконтаинер</span><span class="sxs-lookup"><span data-stu-id="71098-118">blockHostToContainer</span></span>|<span data-ttu-id="71098-119">2</span><span class="sxs-lookup"><span data-stu-id="71098-119">2</span></span>|<span data-ttu-id="71098-120">Блокировка буфера обмена для предоставления общего доступа к данным из узла в контейнер</span><span class="sxs-lookup"><span data-stu-id="71098-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="71098-121">блоккконтаинертохост</span><span class="sxs-lookup"><span data-stu-id="71098-121">blockContainerToHost</span></span>|<span data-ttu-id="71098-122">4</span><span class="sxs-lookup"><span data-stu-id="71098-122">3</span></span>|<span data-ttu-id="71098-123">Блокировка буфера обмена для предоставления общего доступа к данным из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="71098-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="71098-124">блоккноне</span><span class="sxs-lookup"><span data-stu-id="71098-124">blockNone</span></span>|<span data-ttu-id="71098-125">4 </span><span class="sxs-lookup"><span data-stu-id="71098-125">4</span></span>|<span data-ttu-id="71098-126">Блокировка буфера обмена для совместного использования данных без размещения в контейнере и из контейнера в узел</span><span class="sxs-lookup"><span data-stu-id="71098-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



