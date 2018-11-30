---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
ms.openlocfilehash: 694b211afeaaaabb997f03dfc64618fc0301f0ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027612"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="50b3f-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="50b3f-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="50b3f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50b3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50b3f-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="50b3f-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="50b3f-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="50b3f-106">Members</span></span>
|<span data-ttu-id="50b3f-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="50b3f-107">Member</span></span>|<span data-ttu-id="50b3f-108">Значение</span><span class="sxs-lookup"><span data-stu-id="50b3f-108">Value</span></span>|<span data-ttu-id="50b3f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="50b3f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b3f-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="50b3f-110">onPremises</span></span>|<span data-ttu-id="50b3f-111">0</span><span class="sxs-lookup"><span data-stu-id="50b3f-111">0</span></span>|<span data-ttu-id="50b3f-112">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="50b3f-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="50b3f-113">размещенные</span><span class="sxs-lookup"><span data-stu-id="50b3f-113">hosted</span></span>|<span data-ttu-id="50b3f-114">1</span><span class="sxs-lookup"><span data-stu-id="50b3f-114">1</span></span>|<span data-ttu-id="50b3f-115">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="50b3f-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="50b3f-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="50b3f-116">serviceToService</span></span>|<span data-ttu-id="50b3f-117">2</span><span class="sxs-lookup"><span data-stu-id="50b3f-117">2</span></span>|<span data-ttu-id="50b3f-118">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="50b3f-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="50b3f-119">выделенные</span><span class="sxs-lookup"><span data-stu-id="50b3f-119">dedicated</span></span>|<span data-ttu-id="50b3f-120">3</span><span class="sxs-lookup"><span data-stu-id="50b3f-120">3</span></span>|<span data-ttu-id="50b3f-121">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="50b3f-121">Connects to O365 Dedicated Exchange environment.</span></span>|



