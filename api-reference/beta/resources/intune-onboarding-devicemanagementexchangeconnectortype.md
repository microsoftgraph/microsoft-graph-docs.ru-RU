---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36cdb3ff0490ea1b2d446beb587ef3a828e638ed
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993055"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="86f46-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="86f46-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="86f46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86f46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86f46-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86f46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86f46-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="86f46-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="86f46-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="86f46-107">Members</span></span>
|<span data-ttu-id="86f46-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="86f46-108">Member</span></span>|<span data-ttu-id="86f46-109">Значение</span><span class="sxs-lookup"><span data-stu-id="86f46-109">Value</span></span>|<span data-ttu-id="86f46-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86f46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f46-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="86f46-111">onPremises</span></span>|<span data-ttu-id="86f46-112">нуль</span><span class="sxs-lookup"><span data-stu-id="86f46-112">0</span></span>|<span data-ttu-id="86f46-113">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="86f46-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="86f46-114">хост</span><span class="sxs-lookup"><span data-stu-id="86f46-114">hosted</span></span>|<span data-ttu-id="86f46-115">1,1</span><span class="sxs-lookup"><span data-stu-id="86f46-115">1</span></span>|<span data-ttu-id="86f46-116">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="86f46-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="86f46-117">Сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="86f46-117">serviceToService</span></span>|<span data-ttu-id="86f46-118">2</span><span class="sxs-lookup"><span data-stu-id="86f46-118">2</span></span>|<span data-ttu-id="86f46-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="86f46-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="86f46-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="86f46-120">dedicated</span></span>|<span data-ttu-id="86f46-121">4</span><span class="sxs-lookup"><span data-stu-id="86f46-121">3</span></span>|<span data-ttu-id="86f46-122">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="86f46-122">Connects to O365 Dedicated Exchange environment.</span></span>|





