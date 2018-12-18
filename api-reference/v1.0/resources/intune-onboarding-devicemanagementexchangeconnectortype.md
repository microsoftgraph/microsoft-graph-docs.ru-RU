---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
author: tfitzmac
ms.openlocfilehash: 333a5a7c6f73fead263edbdf3edafeefc3514ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306736"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="12684-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="12684-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="12684-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12684-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12684-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="12684-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="12684-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="12684-106">Members</span></span>
|<span data-ttu-id="12684-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="12684-107">Member</span></span>|<span data-ttu-id="12684-108">Значение</span><span class="sxs-lookup"><span data-stu-id="12684-108">Value</span></span>|<span data-ttu-id="12684-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12684-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12684-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="12684-110">onPremises</span></span>|<span data-ttu-id="12684-111">0</span><span class="sxs-lookup"><span data-stu-id="12684-111">0</span></span>|<span data-ttu-id="12684-112">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="12684-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="12684-113">размещенные</span><span class="sxs-lookup"><span data-stu-id="12684-113">hosted</span></span>|<span data-ttu-id="12684-114">1</span><span class="sxs-lookup"><span data-stu-id="12684-114">1</span></span>|<span data-ttu-id="12684-115">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="12684-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="12684-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="12684-116">serviceToService</span></span>|<span data-ttu-id="12684-117">2</span><span class="sxs-lookup"><span data-stu-id="12684-117">2</span></span>|<span data-ttu-id="12684-118">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="12684-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="12684-119">выделенные</span><span class="sxs-lookup"><span data-stu-id="12684-119">dedicated</span></span>|<span data-ttu-id="12684-120">3</span><span class="sxs-lookup"><span data-stu-id="12684-120">3</span></span>|<span data-ttu-id="12684-121">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="12684-121">Connects to O365 Dedicated Exchange environment.</span></span>|



