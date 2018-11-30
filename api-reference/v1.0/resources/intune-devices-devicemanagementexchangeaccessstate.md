---
title: Тип перечисления deviceManagementExchangeAccessState
description: Состояние доступа устройств Exchange.
ms.openlocfilehash: e4891656a85f91c520c783d9e5ce6beac8b08253
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025573"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="17881-103">Тип перечисления deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="17881-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="17881-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17881-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17881-105">Состояние доступа устройств Exchange.</span><span class="sxs-lookup"><span data-stu-id="17881-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="17881-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="17881-106">Members</span></span>
|<span data-ttu-id="17881-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="17881-107">Member</span></span>|<span data-ttu-id="17881-108">Значение</span><span class="sxs-lookup"><span data-stu-id="17881-108">Value</span></span>|<span data-ttu-id="17881-109">Description</span><span class="sxs-lookup"><span data-stu-id="17881-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17881-110">Нет</span><span class="sxs-lookup"><span data-stu-id="17881-110">none</span></span>|<span data-ttu-id="17881-111">0</span><span class="sxs-lookup"><span data-stu-id="17881-111">0</span></span>|<span data-ttu-id="17881-112">Состояние не доступа, обнаруженные в Exchange</span><span class="sxs-lookup"><span data-stu-id="17881-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="17881-113">unknown</span><span class="sxs-lookup"><span data-stu-id="17881-113">unknown</span></span>|<span data-ttu-id="17881-114">1</span><span class="sxs-lookup"><span data-stu-id="17881-114">1</span></span>|<span data-ttu-id="17881-115">Состояние доступа устройства к серверу Exchange не известен</span><span class="sxs-lookup"><span data-stu-id="17881-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="17881-116">разрешено</span><span class="sxs-lookup"><span data-stu-id="17881-116">allowed</span></span>|<span data-ttu-id="17881-117">2</span><span class="sxs-lookup"><span data-stu-id="17881-117">2</span></span>|<span data-ttu-id="17881-118">Устройство имеет доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="17881-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="17881-119">заблокировано</span><span class="sxs-lookup"><span data-stu-id="17881-119">blocked</span></span>|<span data-ttu-id="17881-120">3</span><span class="sxs-lookup"><span data-stu-id="17881-120">3</span></span>|<span data-ttu-id="17881-121">Устройство будет заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="17881-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="17881-122">в карантин</span><span class="sxs-lookup"><span data-stu-id="17881-122">quarantined</span></span>|<span data-ttu-id="17881-123">4</span><span class="sxs-lookup"><span data-stu-id="17881-123">4</span></span>|<span data-ttu-id="17881-124">Находится в карантине в Exchange</span><span class="sxs-lookup"><span data-stu-id="17881-124">Device is Quarantined in Exchange</span></span>|



