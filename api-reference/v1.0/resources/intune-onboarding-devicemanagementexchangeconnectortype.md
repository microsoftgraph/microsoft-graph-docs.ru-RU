---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aec7d3ee34f4d9cdd9a31a93db8934673bbafa7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459478"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="daedb-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="daedb-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="daedb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daedb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daedb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daedb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daedb-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="daedb-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="daedb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="daedb-107">Members</span></span>
|<span data-ttu-id="daedb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="daedb-108">Member</span></span>|<span data-ttu-id="daedb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="daedb-109">Value</span></span>|<span data-ttu-id="daedb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="daedb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daedb-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="daedb-111">onPremises</span></span>|<span data-ttu-id="daedb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="daedb-112">0</span></span>|<span data-ttu-id="daedb-113">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="daedb-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="daedb-114">хост</span><span class="sxs-lookup"><span data-stu-id="daedb-114">hosted</span></span>|<span data-ttu-id="daedb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="daedb-115">1</span></span>|<span data-ttu-id="daedb-116">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="daedb-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="daedb-117">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="daedb-117">serviceToService</span></span>|<span data-ttu-id="daedb-118">2</span><span class="sxs-lookup"><span data-stu-id="daedb-118">2</span></span>|<span data-ttu-id="daedb-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="daedb-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="daedb-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="daedb-120">dedicated</span></span>|<span data-ttu-id="daedb-121">4</span><span class="sxs-lookup"><span data-stu-id="daedb-121">3</span></span>|<span data-ttu-id="daedb-122">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="daedb-122">Connects to O365 Dedicated Exchange environment.</span></span>|







