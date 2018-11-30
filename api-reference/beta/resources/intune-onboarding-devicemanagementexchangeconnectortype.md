---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
ms.openlocfilehash: 59bc1aa080f84fdd25a2da26ec9e7ff9aba20641
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076458"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="84b93-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="84b93-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="84b93-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84b93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84b93-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84b93-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84b93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84b93-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="84b93-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="84b93-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="84b93-108">Members</span></span>
|<span data-ttu-id="84b93-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="84b93-109">Member</span></span>|<span data-ttu-id="84b93-110">Значение</span><span class="sxs-lookup"><span data-stu-id="84b93-110">Value</span></span>|<span data-ttu-id="84b93-111">Description</span><span class="sxs-lookup"><span data-stu-id="84b93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84b93-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="84b93-112">onPremises</span></span>|<span data-ttu-id="84b93-113">0</span><span class="sxs-lookup"><span data-stu-id="84b93-113">0</span></span>|<span data-ttu-id="84b93-114">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="84b93-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="84b93-115">размещенные</span><span class="sxs-lookup"><span data-stu-id="84b93-115">hosted</span></span>|<span data-ttu-id="84b93-116">1</span><span class="sxs-lookup"><span data-stu-id="84b93-116">1</span></span>|<span data-ttu-id="84b93-117">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="84b93-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="84b93-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="84b93-118">serviceToService</span></span>|<span data-ttu-id="84b93-119">2</span><span class="sxs-lookup"><span data-stu-id="84b93-119">2</span></span>|<span data-ttu-id="84b93-120">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="84b93-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="84b93-121">выделенные</span><span class="sxs-lookup"><span data-stu-id="84b93-121">dedicated</span></span>|<span data-ttu-id="84b93-122">3</span><span class="sxs-lookup"><span data-stu-id="84b93-122">3</span></span>|<span data-ttu-id="84b93-123">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="84b93-123">Connects to O365 Dedicated Exchange environment.</span></span>|





