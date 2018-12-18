---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
ms.openlocfilehash: c6612c86911fd3d43128a8a7a441db8093ad3656
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316655"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="e903b-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="e903b-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="e903b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e903b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e903b-105">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="e903b-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="e903b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e903b-106">Members</span></span>
|<span data-ttu-id="e903b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e903b-107">Member</span></span>|<span data-ttu-id="e903b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e903b-108">Value</span></span>|<span data-ttu-id="e903b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e903b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e903b-110">none</span><span class="sxs-lookup"><span data-stu-id="e903b-110">none</span></span>|<span data-ttu-id="e903b-111">0</span><span class="sxs-lookup"><span data-stu-id="e903b-111">0</span></span>|<span data-ttu-id="e903b-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e903b-112">Default status.</span></span>|
|<span data-ttu-id="e903b-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="e903b-113">inProgress</span></span>|<span data-ttu-id="e903b-114">1</span><span class="sxs-lookup"><span data-stu-id="e903b-114">1</span></span>|<span data-ttu-id="e903b-115">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="e903b-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="e903b-116">завершена</span><span class="sxs-lookup"><span data-stu-id="e903b-116">completed</span></span>|<span data-ttu-id="e903b-117">2</span><span class="sxs-lookup"><span data-stu-id="e903b-117">2</span></span>|<span data-ttu-id="e903b-118">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="e903b-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="e903b-119">failed</span><span class="sxs-lookup"><span data-stu-id="e903b-119">failed</span></span>|<span data-ttu-id="e903b-120">3</span><span class="sxs-lookup"><span data-stu-id="e903b-120">3</span></span>|<span data-ttu-id="e903b-121">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e903b-121">Last Sync failed.</span></span>|



