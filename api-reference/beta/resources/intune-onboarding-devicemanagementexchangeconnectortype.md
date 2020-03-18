---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba3550a494350a31a4b7dc3a2977c7b9660a51cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779067"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="3849f-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="3849f-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="3849f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3849f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3849f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3849f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3849f-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="3849f-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="3849f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3849f-107">Members</span></span>
|<span data-ttu-id="3849f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3849f-108">Member</span></span>|<span data-ttu-id="3849f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3849f-109">Value</span></span>|<span data-ttu-id="3849f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3849f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3849f-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="3849f-111">onPremises</span></span>|<span data-ttu-id="3849f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3849f-112">0</span></span>|<span data-ttu-id="3849f-113">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="3849f-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="3849f-114">хост</span><span class="sxs-lookup"><span data-stu-id="3849f-114">hosted</span></span>|<span data-ttu-id="3849f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3849f-115">1</span></span>|<span data-ttu-id="3849f-116">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="3849f-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3849f-117">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="3849f-117">serviceToService</span></span>|<span data-ttu-id="3849f-118">2</span><span class="sxs-lookup"><span data-stu-id="3849f-118">2</span></span>|<span data-ttu-id="3849f-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="3849f-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3849f-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="3849f-120">dedicated</span></span>|<span data-ttu-id="3849f-121">4</span><span class="sxs-lookup"><span data-stu-id="3849f-121">3</span></span>|<span data-ttu-id="3849f-122">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="3849f-122">Connects to O365 Dedicated Exchange environment.</span></span>|



