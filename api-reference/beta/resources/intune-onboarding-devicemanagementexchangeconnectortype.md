---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75129a49352bb2cfe738c0dd58e382b26530ef53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566593"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="2b064-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="2b064-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="2b064-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b064-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b064-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b064-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b064-106">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b064-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="2b064-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2b064-107">Members</span></span>
|<span data-ttu-id="2b064-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2b064-108">Member</span></span>|<span data-ttu-id="2b064-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2b064-109">Value</span></span>|<span data-ttu-id="2b064-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b064-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b064-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="2b064-111">onPremises</span></span>|<span data-ttu-id="2b064-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2b064-112">0</span></span>|<span data-ttu-id="2b064-113">ПодКлючается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b064-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="2b064-114">хост</span><span class="sxs-lookup"><span data-stu-id="2b064-114">hosted</span></span>|<span data-ttu-id="2b064-115">1 </span><span class="sxs-lookup"><span data-stu-id="2b064-115">1</span></span>|<span data-ttu-id="2b064-116">ПодКлючается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="2b064-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="2b064-117">Сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="2b064-117">serviceToService</span></span>|<span data-ttu-id="2b064-118">2 </span><span class="sxs-lookup"><span data-stu-id="2b064-118">2</span></span>|<span data-ttu-id="2b064-119">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="2b064-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="2b064-120">уполномочен</span><span class="sxs-lookup"><span data-stu-id="2b064-120">dedicated</span></span>|<span data-ttu-id="2b064-121">3 </span><span class="sxs-lookup"><span data-stu-id="2b064-121">3</span></span>|<span data-ttu-id="2b064-122">ПодКлючается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="2b064-122">Connects to O365 Dedicated Exchange environment.</span></span>|





