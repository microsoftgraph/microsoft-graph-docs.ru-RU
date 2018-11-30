---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
ms.openlocfilehash: 59d325612430a184feaf7df655a4da660b65ea78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025723"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="047f8-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="047f8-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="047f8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="047f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="047f8-105">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="047f8-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="047f8-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="047f8-106">Members</span></span>
|<span data-ttu-id="047f8-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="047f8-107">Member</span></span>|<span data-ttu-id="047f8-108">Значение</span><span class="sxs-lookup"><span data-stu-id="047f8-108">Value</span></span>|<span data-ttu-id="047f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="047f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047f8-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="047f8-110">notConfigured</span></span>|<span data-ttu-id="047f8-111">0</span><span class="sxs-lookup"><span data-stu-id="047f8-111">0</span></span>|<span data-ttu-id="047f8-112">Не настроен</span><span class="sxs-lookup"><span data-stu-id="047f8-112">Not Configured</span></span>|
|<span data-ttu-id="047f8-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="047f8-113">blockBoth</span></span>|<span data-ttu-id="047f8-114">1</span><span class="sxs-lookup"><span data-stu-id="047f8-114">1</span></span>|<span data-ttu-id="047f8-115">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="047f8-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="047f8-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="047f8-116">blockHostToContainer</span></span>|<span data-ttu-id="047f8-117">2</span><span class="sxs-lookup"><span data-stu-id="047f8-117">2</span></span>|<span data-ttu-id="047f8-118">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="047f8-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="047f8-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="047f8-119">blockContainerToHost</span></span>|<span data-ttu-id="047f8-120">3</span><span class="sxs-lookup"><span data-stu-id="047f8-120">3</span></span>|<span data-ttu-id="047f8-121">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="047f8-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="047f8-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="047f8-122">blockNone</span></span>|<span data-ttu-id="047f8-123">4</span><span class="sxs-lookup"><span data-stu-id="047f8-123">4</span></span>|<span data-ttu-id="047f8-124">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="047f8-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



