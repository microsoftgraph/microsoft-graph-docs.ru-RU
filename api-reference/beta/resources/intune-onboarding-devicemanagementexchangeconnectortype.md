---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: eaab7f66d35b7251aa9dd4f87a8b24f071d26140
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374150"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="b16f3-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="b16f3-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="b16f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b16f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b16f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b16f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b16f3-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="b16f3-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="b16f3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b16f3-107">Members</span></span>
|<span data-ttu-id="b16f3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b16f3-108">Member</span></span>|<span data-ttu-id="b16f3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b16f3-109">Value</span></span>|<span data-ttu-id="b16f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b16f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b16f3-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="b16f3-111">onPremises</span></span>|<span data-ttu-id="b16f3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b16f3-112">0</span></span>|<span data-ttu-id="b16f3-113">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="b16f3-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="b16f3-114">хост</span><span class="sxs-lookup"><span data-stu-id="b16f3-114">hosted</span></span>|<span data-ttu-id="b16f3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b16f3-115">1</span></span>|<span data-ttu-id="b16f3-116">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="b16f3-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b16f3-117">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="b16f3-117">serviceToService</span></span>|<span data-ttu-id="b16f3-118">2</span><span class="sxs-lookup"><span data-stu-id="b16f3-118">2</span></span>|<span data-ttu-id="b16f3-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="b16f3-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b16f3-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="b16f3-120">dedicated</span></span>|<span data-ttu-id="b16f3-121">4</span><span class="sxs-lookup"><span data-stu-id="b16f3-121">3</span></span>|<span data-ttu-id="b16f3-122">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="b16f3-122">Connects to O365 Dedicated Exchange environment.</span></span>|



