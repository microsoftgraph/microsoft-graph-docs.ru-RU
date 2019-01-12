---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7dacce6dbe91a2bbc76b52795bc20de4cf0e5f71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911884"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="99fea-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="99fea-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="99fea-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99fea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99fea-105">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="99fea-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="99fea-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="99fea-106">Members</span></span>
|<span data-ttu-id="99fea-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="99fea-107">Member</span></span>|<span data-ttu-id="99fea-108">Значение</span><span class="sxs-lookup"><span data-stu-id="99fea-108">Value</span></span>|<span data-ttu-id="99fea-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99fea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99fea-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="99fea-110">notConfigured</span></span>|<span data-ttu-id="99fea-111">0</span><span class="sxs-lookup"><span data-stu-id="99fea-111">0</span></span>|<span data-ttu-id="99fea-112">Не настроен</span><span class="sxs-lookup"><span data-stu-id="99fea-112">Not Configured</span></span>|
|<span data-ttu-id="99fea-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="99fea-113">blockBoth</span></span>|<span data-ttu-id="99fea-114">1</span><span class="sxs-lookup"><span data-stu-id="99fea-114">1</span></span>|<span data-ttu-id="99fea-115">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="99fea-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="99fea-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="99fea-116">blockHostToContainer</span></span>|<span data-ttu-id="99fea-117">2</span><span class="sxs-lookup"><span data-stu-id="99fea-117">2</span></span>|<span data-ttu-id="99fea-118">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="99fea-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="99fea-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="99fea-119">blockContainerToHost</span></span>|<span data-ttu-id="99fea-120">3</span><span class="sxs-lookup"><span data-stu-id="99fea-120">3</span></span>|<span data-ttu-id="99fea-121">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="99fea-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="99fea-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="99fea-122">blockNone</span></span>|<span data-ttu-id="99fea-123">4</span><span class="sxs-lookup"><span data-stu-id="99fea-123">4</span></span>|<span data-ttu-id="99fea-124">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="99fea-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



