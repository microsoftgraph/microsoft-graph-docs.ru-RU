---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
ms.openlocfilehash: d55945c0e229801bab9a338a475e6ef6fd5e8b02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311510"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="fa626-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="fa626-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="fa626-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa626-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa626-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa626-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa626-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa626-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa626-107">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="fa626-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="fa626-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fa626-108">Members</span></span>
|<span data-ttu-id="fa626-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fa626-109">Member</span></span>|<span data-ttu-id="fa626-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fa626-110">Value</span></span>|<span data-ttu-id="fa626-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa626-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa626-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fa626-112">notConfigured</span></span>|<span data-ttu-id="fa626-113">0</span><span class="sxs-lookup"><span data-stu-id="fa626-113">0</span></span>|<span data-ttu-id="fa626-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="fa626-114">Not Configured</span></span>|
|<span data-ttu-id="fa626-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="fa626-115">blockBoth</span></span>|<span data-ttu-id="fa626-116">1</span><span class="sxs-lookup"><span data-stu-id="fa626-116">1</span></span>|<span data-ttu-id="fa626-117">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="fa626-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="fa626-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="fa626-118">blockHostToContainer</span></span>|<span data-ttu-id="fa626-119">2</span><span class="sxs-lookup"><span data-stu-id="fa626-119">2</span></span>|<span data-ttu-id="fa626-120">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="fa626-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="fa626-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="fa626-121">blockContainerToHost</span></span>|<span data-ttu-id="fa626-122">3</span><span class="sxs-lookup"><span data-stu-id="fa626-122">3</span></span>|<span data-ttu-id="fa626-123">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="fa626-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="fa626-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="fa626-124">blockNone</span></span>|<span data-ttu-id="fa626-125">4</span><span class="sxs-lookup"><span data-stu-id="fa626-125">4</span></span>|<span data-ttu-id="fa626-126">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="fa626-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





