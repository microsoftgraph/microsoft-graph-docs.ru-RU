---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfdb80ae40abcc505927b94a33330bc09454e790
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965084"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="00556-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="00556-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="00556-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00556-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00556-105">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="00556-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="00556-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="00556-106">Members</span></span>
|<span data-ttu-id="00556-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="00556-107">Member</span></span>|<span data-ttu-id="00556-108">Значение</span><span class="sxs-lookup"><span data-stu-id="00556-108">Value</span></span>|<span data-ttu-id="00556-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00556-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00556-110">Нет</span><span class="sxs-lookup"><span data-stu-id="00556-110">none</span></span>|<span data-ttu-id="00556-111">0</span><span class="sxs-lookup"><span data-stu-id="00556-111">0</span></span>|<span data-ttu-id="00556-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="00556-112">Default status.</span></span>|
|<span data-ttu-id="00556-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="00556-113">inProgress</span></span>|<span data-ttu-id="00556-114">1</span><span class="sxs-lookup"><span data-stu-id="00556-114">1</span></span>|<span data-ttu-id="00556-115">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="00556-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="00556-116">завершена</span><span class="sxs-lookup"><span data-stu-id="00556-116">completed</span></span>|<span data-ttu-id="00556-117">2</span><span class="sxs-lookup"><span data-stu-id="00556-117">2</span></span>|<span data-ttu-id="00556-118">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="00556-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="00556-119">failed</span><span class="sxs-lookup"><span data-stu-id="00556-119">failed</span></span>|<span data-ttu-id="00556-120">3</span><span class="sxs-lookup"><span data-stu-id="00556-120">3</span></span>|<span data-ttu-id="00556-121">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="00556-121">Last Sync failed.</span></span>|



