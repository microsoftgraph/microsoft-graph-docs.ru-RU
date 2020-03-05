---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6c8e7463df2b8f2f172b87e137522906e14b8105
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524148"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="921b0-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="921b0-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="921b0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="921b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="921b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="921b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="921b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="921b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921b0-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="921b0-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="921b0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="921b0-108">Members</span></span>
|<span data-ttu-id="921b0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="921b0-109">Member</span></span>|<span data-ttu-id="921b0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="921b0-110">Value</span></span>|<span data-ttu-id="921b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="921b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921b0-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="921b0-112">onPremises</span></span>|<span data-ttu-id="921b0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="921b0-113">0</span></span>|<span data-ttu-id="921b0-114">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="921b0-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="921b0-115">хост</span><span class="sxs-lookup"><span data-stu-id="921b0-115">hosted</span></span>|<span data-ttu-id="921b0-116">1 </span><span class="sxs-lookup"><span data-stu-id="921b0-116">1</span></span>|<span data-ttu-id="921b0-117">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="921b0-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="921b0-118">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="921b0-118">serviceToService</span></span>|<span data-ttu-id="921b0-119">2 </span><span class="sxs-lookup"><span data-stu-id="921b0-119">2</span></span>|<span data-ttu-id="921b0-120">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="921b0-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="921b0-121">уполномочен</span><span class="sxs-lookup"><span data-stu-id="921b0-121">dedicated</span></span>|<span data-ttu-id="921b0-122">3 </span><span class="sxs-lookup"><span data-stu-id="921b0-122">3</span></span>|<span data-ttu-id="921b0-123">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="921b0-123">Connects to O365 Dedicated Exchange environment.</span></span>|



