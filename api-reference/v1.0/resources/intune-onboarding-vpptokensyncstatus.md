---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
ms.openlocfilehash: e038f15a3c58928ebb066c0fbf5aac320bf574a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027023"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="c1d74-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="c1d74-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="c1d74-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1d74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1d74-105">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="c1d74-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="c1d74-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c1d74-106">Members</span></span>
|<span data-ttu-id="c1d74-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c1d74-107">Member</span></span>|<span data-ttu-id="c1d74-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c1d74-108">Value</span></span>|<span data-ttu-id="c1d74-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c1d74-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d74-110">Нет</span><span class="sxs-lookup"><span data-stu-id="c1d74-110">none</span></span>|<span data-ttu-id="c1d74-111">0</span><span class="sxs-lookup"><span data-stu-id="c1d74-111">0</span></span>|<span data-ttu-id="c1d74-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c1d74-112">Default status.</span></span>|
|<span data-ttu-id="c1d74-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="c1d74-113">inProgress</span></span>|<span data-ttu-id="c1d74-114">1</span><span class="sxs-lookup"><span data-stu-id="c1d74-114">1</span></span>|<span data-ttu-id="c1d74-115">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="c1d74-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="c1d74-116">завершена</span><span class="sxs-lookup"><span data-stu-id="c1d74-116">completed</span></span>|<span data-ttu-id="c1d74-117">2</span><span class="sxs-lookup"><span data-stu-id="c1d74-117">2</span></span>|<span data-ttu-id="c1d74-118">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="c1d74-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="c1d74-119">failed</span><span class="sxs-lookup"><span data-stu-id="c1d74-119">failed</span></span>|<span data-ttu-id="c1d74-120">3</span><span class="sxs-lookup"><span data-stu-id="c1d74-120">3</span></span>|<span data-ttu-id="c1d74-121">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c1d74-121">Last Sync failed.</span></span>|



