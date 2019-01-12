---
title: Тип перечисления deviceManagementExchangeAccessState
description: Состояние доступа устройств Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a407d0971059ed7a0a8bb0ffae2773bc788b31
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928397"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="1d991-103">Тип перечисления deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1d991-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="1d991-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d991-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d991-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d991-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d991-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d991-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d991-107">Состояние доступа устройств Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d991-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="1d991-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d991-108">Members</span></span>
|<span data-ttu-id="1d991-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d991-109">Member</span></span>|<span data-ttu-id="1d991-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1d991-110">Value</span></span>|<span data-ttu-id="1d991-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d991-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d991-112">Нет</span><span class="sxs-lookup"><span data-stu-id="1d991-112">none</span></span>|<span data-ttu-id="1d991-113">0</span><span class="sxs-lookup"><span data-stu-id="1d991-113">0</span></span>|<span data-ttu-id="1d991-114">Состояние не доступа, обнаруженные в Exchange</span><span class="sxs-lookup"><span data-stu-id="1d991-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="1d991-115">unknown</span><span class="sxs-lookup"><span data-stu-id="1d991-115">unknown</span></span>|<span data-ttu-id="1d991-116">1</span><span class="sxs-lookup"><span data-stu-id="1d991-116">1</span></span>|<span data-ttu-id="1d991-117">Состояние доступа устройства к серверу Exchange не известен</span><span class="sxs-lookup"><span data-stu-id="1d991-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="1d991-118">разрешено</span><span class="sxs-lookup"><span data-stu-id="1d991-118">allowed</span></span>|<span data-ttu-id="1d991-119">2</span><span class="sxs-lookup"><span data-stu-id="1d991-119">2</span></span>|<span data-ttu-id="1d991-120">Устройство имеет доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="1d991-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="1d991-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="1d991-121">blocked</span></span>|<span data-ttu-id="1d991-122">3</span><span class="sxs-lookup"><span data-stu-id="1d991-122">3</span></span>|<span data-ttu-id="1d991-123">Устройство будет заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="1d991-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="1d991-124">в карантин</span><span class="sxs-lookup"><span data-stu-id="1d991-124">quarantined</span></span>|<span data-ttu-id="1d991-125">4</span><span class="sxs-lookup"><span data-stu-id="1d991-125">4</span></span>|<span data-ttu-id="1d991-126">Находится в карантине в Exchange</span><span class="sxs-lookup"><span data-stu-id="1d991-126">Device is Quarantined in Exchange</span></span>|





