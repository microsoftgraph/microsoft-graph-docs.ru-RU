---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 10fc00b5d3135535c557cd179d32029a6aef2f6b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736109"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="1ee54-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="1ee54-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="1ee54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ee54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ee54-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ee54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ee54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ee54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee54-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ee54-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="1ee54-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ee54-108">Members</span></span>
|<span data-ttu-id="1ee54-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ee54-109">Member</span></span>|<span data-ttu-id="1ee54-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1ee54-110">Value</span></span>|<span data-ttu-id="1ee54-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1ee54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee54-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="1ee54-112">onPremises</span></span>|<span data-ttu-id="1ee54-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1ee54-113">0</span></span>|<span data-ttu-id="1ee54-114">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ee54-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="1ee54-115">хост</span><span class="sxs-lookup"><span data-stu-id="1ee54-115">hosted</span></span>|<span data-ttu-id="1ee54-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1ee54-116">1</span></span>|<span data-ttu-id="1ee54-117">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="1ee54-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="1ee54-118">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="1ee54-118">serviceToService</span></span>|<span data-ttu-id="1ee54-119">2</span><span class="sxs-lookup"><span data-stu-id="1ee54-119">2</span></span>|<span data-ttu-id="1ee54-120">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="1ee54-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="1ee54-121">уполномочен</span><span class="sxs-lookup"><span data-stu-id="1ee54-121">dedicated</span></span>|<span data-ttu-id="1ee54-122">4</span><span class="sxs-lookup"><span data-stu-id="1ee54-122">3</span></span>|<span data-ttu-id="1ee54-123">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="1ee54-123">Connects to O365 Dedicated Exchange environment.</span></span>|





