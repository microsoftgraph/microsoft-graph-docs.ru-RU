---
title: Тип перечисления applicationGuardBlockClipboardSharingType
description: Возможные значения для applicationGuardBlockClipboardSharingType
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f9621db53e16231f710cccb12d79f65d22d4017
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415063"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="53ddf-103">Тип перечисления applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="53ddf-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="53ddf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53ddf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53ddf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53ddf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53ddf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53ddf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53ddf-107">Возможные значения для applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="53ddf-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="53ddf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="53ddf-108">Members</span></span>
|<span data-ttu-id="53ddf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="53ddf-109">Member</span></span>|<span data-ttu-id="53ddf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="53ddf-110">Value</span></span>|<span data-ttu-id="53ddf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53ddf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53ddf-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="53ddf-112">notConfigured</span></span>|<span data-ttu-id="53ddf-113">0</span><span class="sxs-lookup"><span data-stu-id="53ddf-113">0</span></span>|<span data-ttu-id="53ddf-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="53ddf-114">Not Configured</span></span>|
|<span data-ttu-id="53ddf-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="53ddf-115">blockBoth</span></span>|<span data-ttu-id="53ddf-116">1</span><span class="sxs-lookup"><span data-stu-id="53ddf-116">1</span></span>|<span data-ttu-id="53ddf-117">Буфер обмена блока совместный доступ к данным из узла в контейнер и из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="53ddf-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="53ddf-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="53ddf-118">blockHostToContainer</span></span>|<span data-ttu-id="53ddf-119">2</span><span class="sxs-lookup"><span data-stu-id="53ddf-119">2</span></span>|<span data-ttu-id="53ddf-120">Буфер обмена блокировки для совместного использования данных из узла, который контейнера</span><span class="sxs-lookup"><span data-stu-id="53ddf-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="53ddf-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="53ddf-121">blockContainerToHost</span></span>|<span data-ttu-id="53ddf-122">3</span><span class="sxs-lookup"><span data-stu-id="53ddf-122">3</span></span>|<span data-ttu-id="53ddf-123">Буфер обмена блока совместный доступ к данным из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="53ddf-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="53ddf-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="53ddf-124">blockNone</span></span>|<span data-ttu-id="53ddf-125">4</span><span class="sxs-lookup"><span data-stu-id="53ddf-125">4</span></span>|<span data-ttu-id="53ddf-126">Буфер обмена блока совместный доступ к данным из узла в контейнер, ни из контейнера для размещения</span><span class="sxs-lookup"><span data-stu-id="53ddf-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




