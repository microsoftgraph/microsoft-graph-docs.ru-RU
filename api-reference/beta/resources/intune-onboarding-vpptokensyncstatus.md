---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
ms.openlocfilehash: 443eb87299fbb052edf8788d07b029c68d58c2fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080948"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="ebe96-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ebe96-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="ebe96-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebe96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebe96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebe96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebe96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebe96-107">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="ebe96-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="ebe96-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ebe96-108">Members</span></span>
|<span data-ttu-id="ebe96-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ebe96-109">Member</span></span>|<span data-ttu-id="ebe96-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ebe96-110">Value</span></span>|<span data-ttu-id="ebe96-111">Description</span><span class="sxs-lookup"><span data-stu-id="ebe96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe96-112">Нет</span><span class="sxs-lookup"><span data-stu-id="ebe96-112">none</span></span>|<span data-ttu-id="ebe96-113">0</span><span class="sxs-lookup"><span data-stu-id="ebe96-113">0</span></span>|<span data-ttu-id="ebe96-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ebe96-114">Default status.</span></span>|
|<span data-ttu-id="ebe96-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="ebe96-115">inProgress</span></span>|<span data-ttu-id="ebe96-116">1</span><span class="sxs-lookup"><span data-stu-id="ebe96-116">1</span></span>|<span data-ttu-id="ebe96-117">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="ebe96-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="ebe96-118">завершена</span><span class="sxs-lookup"><span data-stu-id="ebe96-118">completed</span></span>|<span data-ttu-id="ebe96-119">2</span><span class="sxs-lookup"><span data-stu-id="ebe96-119">2</span></span>|<span data-ttu-id="ebe96-120">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="ebe96-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="ebe96-121">failed</span><span class="sxs-lookup"><span data-stu-id="ebe96-121">failed</span></span>|<span data-ttu-id="ebe96-122">3</span><span class="sxs-lookup"><span data-stu-id="ebe96-122">3</span></span>|<span data-ttu-id="ebe96-123">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ebe96-123">Last Sync failed.</span></span>|





