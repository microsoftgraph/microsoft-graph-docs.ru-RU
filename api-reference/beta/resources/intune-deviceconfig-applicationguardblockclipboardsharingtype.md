---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
ms.openlocfilehash: e0e05001e4f3cedc2893fc6b2006f5b5b5d74db6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079228"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="66e24-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="66e24-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="66e24-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66e24-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e24-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66e24-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66e24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66e24-107">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="66e24-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="66e24-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="66e24-108">Members</span></span>
|<span data-ttu-id="66e24-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="66e24-109">Member</span></span>|<span data-ttu-id="66e24-110">Значение</span><span class="sxs-lookup"><span data-stu-id="66e24-110">Value</span></span>|<span data-ttu-id="66e24-111">Description</span><span class="sxs-lookup"><span data-stu-id="66e24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e24-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="66e24-112">notConfigured</span></span>|<span data-ttu-id="66e24-113">0</span><span class="sxs-lookup"><span data-stu-id="66e24-113">0</span></span>|<span data-ttu-id="66e24-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="66e24-114">Not Configured</span></span>|
|<span data-ttu-id="66e24-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="66e24-115">blockBoth</span></span>|<span data-ttu-id="66e24-116">1</span><span class="sxs-lookup"><span data-stu-id="66e24-116">1</span></span>|<span data-ttu-id="66e24-117">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="66e24-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="66e24-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="66e24-118">blockHostToContainer</span></span>|<span data-ttu-id="66e24-119">2</span><span class="sxs-lookup"><span data-stu-id="66e24-119">2</span></span>|<span data-ttu-id="66e24-120">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="66e24-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="66e24-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="66e24-121">blockContainerToHost</span></span>|<span data-ttu-id="66e24-122">3</span><span class="sxs-lookup"><span data-stu-id="66e24-122">3</span></span>|<span data-ttu-id="66e24-123">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="66e24-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="66e24-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="66e24-124">blockNone</span></span>|<span data-ttu-id="66e24-125">4</span><span class="sxs-lookup"><span data-stu-id="66e24-125">4</span></span>|<span data-ttu-id="66e24-126">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="66e24-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





