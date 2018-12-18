---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
ms.openlocfilehash: af1843a8d7515e5ca14997256968942f485eab64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304083"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="adfb9-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="adfb9-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="adfb9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="adfb9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adfb9-105">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="adfb9-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="adfb9-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="adfb9-106">Members</span></span>
|<span data-ttu-id="adfb9-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="adfb9-107">Member</span></span>|<span data-ttu-id="adfb9-108">Значение</span><span class="sxs-lookup"><span data-stu-id="adfb9-108">Value</span></span>|<span data-ttu-id="adfb9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="adfb9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adfb9-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="adfb9-110">notConfigured</span></span>|<span data-ttu-id="adfb9-111">0</span><span class="sxs-lookup"><span data-stu-id="adfb9-111">0</span></span>|<span data-ttu-id="adfb9-112">Не настроен</span><span class="sxs-lookup"><span data-stu-id="adfb9-112">Not Configured</span></span>|
|<span data-ttu-id="adfb9-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="adfb9-113">blockBoth</span></span>|<span data-ttu-id="adfb9-114">1</span><span class="sxs-lookup"><span data-stu-id="adfb9-114">1</span></span>|<span data-ttu-id="adfb9-115">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="adfb9-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="adfb9-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="adfb9-116">blockHostToContainer</span></span>|<span data-ttu-id="adfb9-117">2</span><span class="sxs-lookup"><span data-stu-id="adfb9-117">2</span></span>|<span data-ttu-id="adfb9-118">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="adfb9-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="adfb9-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="adfb9-119">blockContainerToHost</span></span>|<span data-ttu-id="adfb9-120">3</span><span class="sxs-lookup"><span data-stu-id="adfb9-120">3</span></span>|<span data-ttu-id="adfb9-121">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="adfb9-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="adfb9-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="adfb9-122">blockNone</span></span>|<span data-ttu-id="adfb9-123">4</span><span class="sxs-lookup"><span data-stu-id="adfb9-123">4</span></span>|<span data-ttu-id="adfb9-124">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="adfb9-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



