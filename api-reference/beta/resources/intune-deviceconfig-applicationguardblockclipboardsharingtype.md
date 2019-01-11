---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f11df623a3b7dcf79df351fac7d6eeee80c254ce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851494"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="b7d42-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="b7d42-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="b7d42-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7d42-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7d42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7d42-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b7d42-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7d42-107">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="b7d42-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="b7d42-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b7d42-108">Members</span></span>
|<span data-ttu-id="b7d42-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b7d42-109">Member</span></span>|<span data-ttu-id="b7d42-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b7d42-110">Value</span></span>|<span data-ttu-id="b7d42-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7d42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d42-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b7d42-112">notConfigured</span></span>|<span data-ttu-id="b7d42-113">0</span><span class="sxs-lookup"><span data-stu-id="b7d42-113">0</span></span>|<span data-ttu-id="b7d42-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="b7d42-114">Not Configured</span></span>|
|<span data-ttu-id="b7d42-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="b7d42-115">blockBoth</span></span>|<span data-ttu-id="b7d42-116">1</span><span class="sxs-lookup"><span data-stu-id="b7d42-116">1</span></span>|<span data-ttu-id="b7d42-117">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="b7d42-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="b7d42-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="b7d42-118">blockHostToContainer</span></span>|<span data-ttu-id="b7d42-119">2</span><span class="sxs-lookup"><span data-stu-id="b7d42-119">2</span></span>|<span data-ttu-id="b7d42-120">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="b7d42-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="b7d42-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="b7d42-121">blockContainerToHost</span></span>|<span data-ttu-id="b7d42-122">3</span><span class="sxs-lookup"><span data-stu-id="b7d42-122">3</span></span>|<span data-ttu-id="b7d42-123">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="b7d42-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="b7d42-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="b7d42-124">blockNone</span></span>|<span data-ttu-id="b7d42-125">4</span><span class="sxs-lookup"><span data-stu-id="b7d42-125">4</span></span>|<span data-ttu-id="b7d42-126">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="b7d42-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





