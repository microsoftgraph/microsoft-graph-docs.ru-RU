---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07449df53aa65036ae55e63c514c1687fbbab86a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888517"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="c5a09-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="c5a09-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="c5a09-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5a09-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5a09-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5a09-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="c5a09-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5a09-106">Members</span></span>
|<span data-ttu-id="c5a09-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5a09-107">Member</span></span>|<span data-ttu-id="c5a09-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c5a09-108">Value</span></span>|<span data-ttu-id="c5a09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a09-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a09-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="c5a09-110">onPremises</span></span>|<span data-ttu-id="c5a09-111">0</span><span class="sxs-lookup"><span data-stu-id="c5a09-111">0</span></span>|<span data-ttu-id="c5a09-112">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5a09-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="c5a09-113">размещенные</span><span class="sxs-lookup"><span data-stu-id="c5a09-113">hosted</span></span>|<span data-ttu-id="c5a09-114">1</span><span class="sxs-lookup"><span data-stu-id="c5a09-114">1</span></span>|<span data-ttu-id="c5a09-115">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="c5a09-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="c5a09-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="c5a09-116">serviceToService</span></span>|<span data-ttu-id="c5a09-117">2</span><span class="sxs-lookup"><span data-stu-id="c5a09-117">2</span></span>|<span data-ttu-id="c5a09-118">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="c5a09-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="c5a09-119">выделенные</span><span class="sxs-lookup"><span data-stu-id="c5a09-119">dedicated</span></span>|<span data-ttu-id="c5a09-120">3</span><span class="sxs-lookup"><span data-stu-id="c5a09-120">3</span></span>|<span data-ttu-id="c5a09-121">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="c5a09-121">Connects to O365 Dedicated Exchange environment.</span></span>|



