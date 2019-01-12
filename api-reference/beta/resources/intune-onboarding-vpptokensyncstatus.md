---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4101f1338513787b27ce530579ffd42c7756366a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931288"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="8de43-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8de43-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="8de43-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8de43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8de43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8de43-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8de43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8de43-107">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="8de43-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="8de43-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8de43-108">Members</span></span>
|<span data-ttu-id="8de43-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8de43-109">Member</span></span>|<span data-ttu-id="8de43-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8de43-110">Value</span></span>|<span data-ttu-id="8de43-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8de43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de43-112">Нет</span><span class="sxs-lookup"><span data-stu-id="8de43-112">none</span></span>|<span data-ttu-id="8de43-113">0</span><span class="sxs-lookup"><span data-stu-id="8de43-113">0</span></span>|<span data-ttu-id="8de43-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8de43-114">Default status.</span></span>|
|<span data-ttu-id="8de43-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="8de43-115">inProgress</span></span>|<span data-ttu-id="8de43-116">1</span><span class="sxs-lookup"><span data-stu-id="8de43-116">1</span></span>|<span data-ttu-id="8de43-117">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="8de43-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="8de43-118">завершена</span><span class="sxs-lookup"><span data-stu-id="8de43-118">completed</span></span>|<span data-ttu-id="8de43-119">2</span><span class="sxs-lookup"><span data-stu-id="8de43-119">2</span></span>|<span data-ttu-id="8de43-120">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="8de43-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="8de43-121">failed</span><span class="sxs-lookup"><span data-stu-id="8de43-121">failed</span></span>|<span data-ttu-id="8de43-122">3</span><span class="sxs-lookup"><span data-stu-id="8de43-122">3</span></span>|<span data-ttu-id="8de43-123">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8de43-123">Last Sync failed.</span></span>|





