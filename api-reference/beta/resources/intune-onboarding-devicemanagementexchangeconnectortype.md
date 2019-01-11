---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49e61dc3a2a6ba7eee80891846cd2f58c2a22485
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876106"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="47a77-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="47a77-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="47a77-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47a77-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a77-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47a77-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47a77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a77-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="47a77-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="47a77-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="47a77-108">Members</span></span>
|<span data-ttu-id="47a77-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="47a77-109">Member</span></span>|<span data-ttu-id="47a77-110">Значение</span><span class="sxs-lookup"><span data-stu-id="47a77-110">Value</span></span>|<span data-ttu-id="47a77-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47a77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a77-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="47a77-112">onPremises</span></span>|<span data-ttu-id="47a77-113">0</span><span class="sxs-lookup"><span data-stu-id="47a77-113">0</span></span>|<span data-ttu-id="47a77-114">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="47a77-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="47a77-115">размещенные</span><span class="sxs-lookup"><span data-stu-id="47a77-115">hosted</span></span>|<span data-ttu-id="47a77-116">1</span><span class="sxs-lookup"><span data-stu-id="47a77-116">1</span></span>|<span data-ttu-id="47a77-117">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="47a77-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="47a77-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="47a77-118">serviceToService</span></span>|<span data-ttu-id="47a77-119">2</span><span class="sxs-lookup"><span data-stu-id="47a77-119">2</span></span>|<span data-ttu-id="47a77-120">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="47a77-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="47a77-121">выделенные</span><span class="sxs-lookup"><span data-stu-id="47a77-121">dedicated</span></span>|<span data-ttu-id="47a77-122">3</span><span class="sxs-lookup"><span data-stu-id="47a77-122">3</span></span>|<span data-ttu-id="47a77-123">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="47a77-123">Connects to O365 Dedicated Exchange environment.</span></span>|





