---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
ms.openlocfilehash: 18a0fcf9f4d22d7904cb76d1fc45d80b14dfc7d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344242"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="a76e5-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a76e5-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="a76e5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a76e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a76e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a76e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a76e5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a76e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a76e5-107">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="a76e5-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="a76e5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a76e5-108">Members</span></span>
|<span data-ttu-id="a76e5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a76e5-109">Member</span></span>|<span data-ttu-id="a76e5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a76e5-110">Value</span></span>|<span data-ttu-id="a76e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a76e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a76e5-112">none</span><span class="sxs-lookup"><span data-stu-id="a76e5-112">none</span></span>|<span data-ttu-id="a76e5-113">0</span><span class="sxs-lookup"><span data-stu-id="a76e5-113">0</span></span>|<span data-ttu-id="a76e5-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a76e5-114">Default status.</span></span>|
|<span data-ttu-id="a76e5-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="a76e5-115">inProgress</span></span>|<span data-ttu-id="a76e5-116">1</span><span class="sxs-lookup"><span data-stu-id="a76e5-116">1</span></span>|<span data-ttu-id="a76e5-117">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="a76e5-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="a76e5-118">завершена</span><span class="sxs-lookup"><span data-stu-id="a76e5-118">completed</span></span>|<span data-ttu-id="a76e5-119">2</span><span class="sxs-lookup"><span data-stu-id="a76e5-119">2</span></span>|<span data-ttu-id="a76e5-120">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="a76e5-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="a76e5-121">failed</span><span class="sxs-lookup"><span data-stu-id="a76e5-121">failed</span></span>|<span data-ttu-id="a76e5-122">3</span><span class="sxs-lookup"><span data-stu-id="a76e5-122">3</span></span>|<span data-ttu-id="a76e5-123">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a76e5-123">Last Sync failed.</span></span>|





