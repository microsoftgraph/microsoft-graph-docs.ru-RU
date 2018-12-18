---
title: Тип перечисления deviceManagementExchangeAccessState
description: Состояние доступа устройств Exchange.
author: tfitzmac
ms.openlocfilehash: cb72a3e07f0f14fdd509bb0274605cb9592db241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328744"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="16764-103">Тип перечисления deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="16764-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="16764-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16764-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16764-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16764-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16764-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16764-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16764-107">Состояние доступа устройств Exchange.</span><span class="sxs-lookup"><span data-stu-id="16764-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="16764-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="16764-108">Members</span></span>
|<span data-ttu-id="16764-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="16764-109">Member</span></span>|<span data-ttu-id="16764-110">Значение</span><span class="sxs-lookup"><span data-stu-id="16764-110">Value</span></span>|<span data-ttu-id="16764-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16764-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16764-112">none</span><span class="sxs-lookup"><span data-stu-id="16764-112">none</span></span>|<span data-ttu-id="16764-113">0</span><span class="sxs-lookup"><span data-stu-id="16764-113">0</span></span>|<span data-ttu-id="16764-114">Состояние не доступа, обнаруженные в Exchange</span><span class="sxs-lookup"><span data-stu-id="16764-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="16764-115">unknown</span><span class="sxs-lookup"><span data-stu-id="16764-115">unknown</span></span>|<span data-ttu-id="16764-116">1</span><span class="sxs-lookup"><span data-stu-id="16764-116">1</span></span>|<span data-ttu-id="16764-117">Состояние доступа устройства к серверу Exchange не известен</span><span class="sxs-lookup"><span data-stu-id="16764-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="16764-118">разрешено</span><span class="sxs-lookup"><span data-stu-id="16764-118">allowed</span></span>|<span data-ttu-id="16764-119">2</span><span class="sxs-lookup"><span data-stu-id="16764-119">2</span></span>|<span data-ttu-id="16764-120">Устройство имеет доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="16764-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="16764-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="16764-121">blocked</span></span>|<span data-ttu-id="16764-122">3</span><span class="sxs-lookup"><span data-stu-id="16764-122">3</span></span>|<span data-ttu-id="16764-123">Устройство будет заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="16764-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="16764-124">в карантин</span><span class="sxs-lookup"><span data-stu-id="16764-124">quarantined</span></span>|<span data-ttu-id="16764-125">4</span><span class="sxs-lookup"><span data-stu-id="16764-125">4</span></span>|<span data-ttu-id="16764-126">Находится в карантине в Exchange</span><span class="sxs-lookup"><span data-stu-id="16764-126">Device is Quarantined in Exchange</span></span>|





