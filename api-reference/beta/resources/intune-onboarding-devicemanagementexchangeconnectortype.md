---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: af90d5f3fd461fbc7888cabec66959f385a4dc3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029626"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="26802-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="26802-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="26802-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26802-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26802-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26802-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26802-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26802-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26802-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="26802-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="26802-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="26802-108">Members</span></span>
|<span data-ttu-id="26802-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="26802-109">Member</span></span>|<span data-ttu-id="26802-110">Значение</span><span class="sxs-lookup"><span data-stu-id="26802-110">Value</span></span>|<span data-ttu-id="26802-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26802-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26802-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="26802-112">onPremises</span></span>|<span data-ttu-id="26802-113">нуль</span><span class="sxs-lookup"><span data-stu-id="26802-113">0</span></span>|<span data-ttu-id="26802-114">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="26802-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="26802-115">хост</span><span class="sxs-lookup"><span data-stu-id="26802-115">hosted</span></span>|<span data-ttu-id="26802-116">1 </span><span class="sxs-lookup"><span data-stu-id="26802-116">1</span></span>|<span data-ttu-id="26802-117">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="26802-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="26802-118">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="26802-118">serviceToService</span></span>|<span data-ttu-id="26802-119">2 </span><span class="sxs-lookup"><span data-stu-id="26802-119">2</span></span>|<span data-ttu-id="26802-120">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="26802-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="26802-121">уполномочен</span><span class="sxs-lookup"><span data-stu-id="26802-121">dedicated</span></span>|<span data-ttu-id="26802-122">4</span><span class="sxs-lookup"><span data-stu-id="26802-122">3</span></span>|<span data-ttu-id="26802-123">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="26802-123">Connects to O365 Dedicated Exchange environment.</span></span>|






