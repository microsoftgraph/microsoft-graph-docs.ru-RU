---
title: Тип перечисления deviceManagementExchangeAccessState
description: Состояние доступа устройств Exchange.
author: tfitzmac
ms.openlocfilehash: 37db054314375411dc237746ca6ca3bdb99e9016
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328723"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="ce489-103">Тип перечисления deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ce489-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="ce489-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce489-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce489-105">Состояние доступа устройств Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce489-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="ce489-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce489-106">Members</span></span>
|<span data-ttu-id="ce489-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ce489-107">Member</span></span>|<span data-ttu-id="ce489-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ce489-108">Value</span></span>|<span data-ttu-id="ce489-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce489-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce489-110">none</span><span class="sxs-lookup"><span data-stu-id="ce489-110">none</span></span>|<span data-ttu-id="ce489-111">0</span><span class="sxs-lookup"><span data-stu-id="ce489-111">0</span></span>|<span data-ttu-id="ce489-112">Состояние не доступа, обнаруженные в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce489-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="ce489-113">unknown</span><span class="sxs-lookup"><span data-stu-id="ce489-113">unknown</span></span>|<span data-ttu-id="ce489-114">1</span><span class="sxs-lookup"><span data-stu-id="ce489-114">1</span></span>|<span data-ttu-id="ce489-115">Состояние доступа устройства к серверу Exchange не известен</span><span class="sxs-lookup"><span data-stu-id="ce489-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="ce489-116">разрешено</span><span class="sxs-lookup"><span data-stu-id="ce489-116">allowed</span></span>|<span data-ttu-id="ce489-117">2</span><span class="sxs-lookup"><span data-stu-id="ce489-117">2</span></span>|<span data-ttu-id="ce489-118">Устройство имеет доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="ce489-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="ce489-119">заблокировано</span><span class="sxs-lookup"><span data-stu-id="ce489-119">blocked</span></span>|<span data-ttu-id="ce489-120">3</span><span class="sxs-lookup"><span data-stu-id="ce489-120">3</span></span>|<span data-ttu-id="ce489-121">Устройство будет заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce489-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="ce489-122">в карантин</span><span class="sxs-lookup"><span data-stu-id="ce489-122">quarantined</span></span>|<span data-ttu-id="ce489-123">4</span><span class="sxs-lookup"><span data-stu-id="ce489-123">4</span></span>|<span data-ttu-id="ce489-124">Находится в карантине в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce489-124">Device is Quarantined in Exchange</span></span>|



