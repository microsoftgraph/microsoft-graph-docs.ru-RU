---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db458423a00fd7b38bddea1b1954cda1ec6ec83b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888685"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="a6156-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a6156-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="a6156-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6156-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6156-105">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="a6156-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="a6156-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a6156-106">Members</span></span>
|<span data-ttu-id="a6156-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a6156-107">Member</span></span>|<span data-ttu-id="a6156-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a6156-108">Value</span></span>|<span data-ttu-id="a6156-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6156-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6156-110">Нет</span><span class="sxs-lookup"><span data-stu-id="a6156-110">none</span></span>|<span data-ttu-id="a6156-111">0</span><span class="sxs-lookup"><span data-stu-id="a6156-111">0</span></span>|<span data-ttu-id="a6156-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6156-112">Default status.</span></span>|
|<span data-ttu-id="a6156-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="a6156-113">inProgress</span></span>|<span data-ttu-id="a6156-114">1</span><span class="sxs-lookup"><span data-stu-id="a6156-114">1</span></span>|<span data-ttu-id="a6156-115">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="a6156-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="a6156-116">завершена</span><span class="sxs-lookup"><span data-stu-id="a6156-116">completed</span></span>|<span data-ttu-id="a6156-117">2</span><span class="sxs-lookup"><span data-stu-id="a6156-117">2</span></span>|<span data-ttu-id="a6156-118">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="a6156-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="a6156-119">failed</span><span class="sxs-lookup"><span data-stu-id="a6156-119">failed</span></span>|<span data-ttu-id="a6156-120">3</span><span class="sxs-lookup"><span data-stu-id="a6156-120">3</span></span>|<span data-ttu-id="a6156-121">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a6156-121">Last Sync failed.</span></span>|



