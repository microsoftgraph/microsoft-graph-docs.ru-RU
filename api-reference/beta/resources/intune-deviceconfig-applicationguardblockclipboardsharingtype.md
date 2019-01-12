---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cba0a3fcd25c9f4672d7590718c25e977edf635b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949145"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="c5e80-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="c5e80-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="c5e80-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5e80-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5e80-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5e80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5e80-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5e80-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5e80-107">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="c5e80-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="c5e80-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5e80-108">Members</span></span>
|<span data-ttu-id="c5e80-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5e80-109">Member</span></span>|<span data-ttu-id="c5e80-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c5e80-110">Value</span></span>|<span data-ttu-id="c5e80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e80-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c5e80-112">notConfigured</span></span>|<span data-ttu-id="c5e80-113">0</span><span class="sxs-lookup"><span data-stu-id="c5e80-113">0</span></span>|<span data-ttu-id="c5e80-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="c5e80-114">Not Configured</span></span>|
|<span data-ttu-id="c5e80-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="c5e80-115">blockBoth</span></span>|<span data-ttu-id="c5e80-116">1</span><span class="sxs-lookup"><span data-stu-id="c5e80-116">1</span></span>|<span data-ttu-id="c5e80-117">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="c5e80-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="c5e80-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="c5e80-118">blockHostToContainer</span></span>|<span data-ttu-id="c5e80-119">2</span><span class="sxs-lookup"><span data-stu-id="c5e80-119">2</span></span>|<span data-ttu-id="c5e80-120">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="c5e80-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="c5e80-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="c5e80-121">blockContainerToHost</span></span>|<span data-ttu-id="c5e80-122">3</span><span class="sxs-lookup"><span data-stu-id="c5e80-122">3</span></span>|<span data-ttu-id="c5e80-123">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="c5e80-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="c5e80-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="c5e80-124">blockNone</span></span>|<span data-ttu-id="c5e80-125">4</span><span class="sxs-lookup"><span data-stu-id="c5e80-125">4</span></span>|<span data-ttu-id="c5e80-126">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="c5e80-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





