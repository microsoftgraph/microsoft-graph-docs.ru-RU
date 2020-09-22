---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9b34a3e51161ffd11321893f2f612385874188c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056522"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="bff1a-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="bff1a-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="bff1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bff1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bff1a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bff1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bff1a-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="bff1a-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="bff1a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bff1a-107">Members</span></span>
|<span data-ttu-id="bff1a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bff1a-108">Member</span></span>|<span data-ttu-id="bff1a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bff1a-109">Value</span></span>|<span data-ttu-id="bff1a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bff1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff1a-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="bff1a-111">onPremises</span></span>|<span data-ttu-id="bff1a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bff1a-112">0</span></span>|<span data-ttu-id="bff1a-113">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="bff1a-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="bff1a-114">хост</span><span class="sxs-lookup"><span data-stu-id="bff1a-114">hosted</span></span>|<span data-ttu-id="bff1a-115">1 </span><span class="sxs-lookup"><span data-stu-id="bff1a-115">1</span></span>|<span data-ttu-id="bff1a-116">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="bff1a-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="bff1a-117">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="bff1a-117">serviceToService</span></span>|<span data-ttu-id="bff1a-118">2 </span><span class="sxs-lookup"><span data-stu-id="bff1a-118">2</span></span>|<span data-ttu-id="bff1a-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="bff1a-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="bff1a-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="bff1a-120">dedicated</span></span>|<span data-ttu-id="bff1a-121">4</span><span class="sxs-lookup"><span data-stu-id="bff1a-121">3</span></span>|<span data-ttu-id="bff1a-122">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="bff1a-122">Connects to O365 Dedicated Exchange environment.</span></span>|









