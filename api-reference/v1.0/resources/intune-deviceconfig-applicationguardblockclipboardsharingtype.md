---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fe418aa1f91c0e65770b797781dda9e29803d86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865977"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="1ef69-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="1ef69-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="1ef69-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ef69-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ef69-105">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="1ef69-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="1ef69-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ef69-106">Members</span></span>
|<span data-ttu-id="1ef69-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ef69-107">Member</span></span>|<span data-ttu-id="1ef69-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1ef69-108">Value</span></span>|<span data-ttu-id="1ef69-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef69-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef69-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1ef69-110">notConfigured</span></span>|<span data-ttu-id="1ef69-111">0</span><span class="sxs-lookup"><span data-stu-id="1ef69-111">0</span></span>|<span data-ttu-id="1ef69-112">Не настроен</span><span class="sxs-lookup"><span data-stu-id="1ef69-112">Not Configured</span></span>|
|<span data-ttu-id="1ef69-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="1ef69-113">blockBoth</span></span>|<span data-ttu-id="1ef69-114">1</span><span class="sxs-lookup"><span data-stu-id="1ef69-114">1</span></span>|<span data-ttu-id="1ef69-115">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="1ef69-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="1ef69-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="1ef69-116">blockHostToContainer</span></span>|<span data-ttu-id="1ef69-117">2</span><span class="sxs-lookup"><span data-stu-id="1ef69-117">2</span></span>|<span data-ttu-id="1ef69-118">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="1ef69-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="1ef69-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="1ef69-119">blockContainerToHost</span></span>|<span data-ttu-id="1ef69-120">3</span><span class="sxs-lookup"><span data-stu-id="1ef69-120">3</span></span>|<span data-ttu-id="1ef69-121">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="1ef69-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="1ef69-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="1ef69-122">blockNone</span></span>|<span data-ttu-id="1ef69-123">4</span><span class="sxs-lookup"><span data-stu-id="1ef69-123">4</span></span>|<span data-ttu-id="1ef69-124">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="1ef69-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



