---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
author: tfitzmac
ms.openlocfilehash: 31459d4053e2ba1ef22a516995796baef2407dbf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301731"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="9049b-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="9049b-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="9049b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9049b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9049b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9049b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9049b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9049b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9049b-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="9049b-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="9049b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9049b-108">Members</span></span>
|<span data-ttu-id="9049b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9049b-109">Member</span></span>|<span data-ttu-id="9049b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9049b-110">Value</span></span>|<span data-ttu-id="9049b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9049b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9049b-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="9049b-112">onPremises</span></span>|<span data-ttu-id="9049b-113">0</span><span class="sxs-lookup"><span data-stu-id="9049b-113">0</span></span>|<span data-ttu-id="9049b-114">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="9049b-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="9049b-115">размещенные</span><span class="sxs-lookup"><span data-stu-id="9049b-115">hosted</span></span>|<span data-ttu-id="9049b-116">1</span><span class="sxs-lookup"><span data-stu-id="9049b-116">1</span></span>|<span data-ttu-id="9049b-117">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="9049b-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9049b-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="9049b-118">serviceToService</span></span>|<span data-ttu-id="9049b-119">2</span><span class="sxs-lookup"><span data-stu-id="9049b-119">2</span></span>|<span data-ttu-id="9049b-120">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="9049b-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9049b-121">выделенные</span><span class="sxs-lookup"><span data-stu-id="9049b-121">dedicated</span></span>|<span data-ttu-id="9049b-122">3</span><span class="sxs-lookup"><span data-stu-id="9049b-122">3</span></span>|<span data-ttu-id="9049b-123">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="9049b-123">Connects to O365 Dedicated Exchange environment.</span></span>|





