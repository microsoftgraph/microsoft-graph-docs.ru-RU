---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358832db83e5f5b3e1fb0f5457f480d21ded996
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263562"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="79127-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="79127-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="79127-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79127-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79127-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="79127-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="79127-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="79127-106">Members</span></span>
|<span data-ttu-id="79127-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="79127-107">Member</span></span>|<span data-ttu-id="79127-108">Значение</span><span class="sxs-lookup"><span data-stu-id="79127-108">Value</span></span>|<span data-ttu-id="79127-109">Описание</span><span class="sxs-lookup"><span data-stu-id="79127-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79127-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="79127-110">onPremises</span></span>|<span data-ttu-id="79127-111">нуль</span><span class="sxs-lookup"><span data-stu-id="79127-111">0</span></span>|<span data-ttu-id="79127-112">ПодКлючается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="79127-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="79127-113">хост</span><span class="sxs-lookup"><span data-stu-id="79127-113">hosted</span></span>|<span data-ttu-id="79127-114">1,1</span><span class="sxs-lookup"><span data-stu-id="79127-114">1</span></span>|<span data-ttu-id="79127-115">ПодКлючается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="79127-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="79127-116">Сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="79127-116">serviceToService</span></span>|<span data-ttu-id="79127-117">2</span><span class="sxs-lookup"><span data-stu-id="79127-117">2</span></span>|<span data-ttu-id="79127-118">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="79127-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="79127-119">уполномочен</span><span class="sxs-lookup"><span data-stu-id="79127-119">dedicated</span></span>|<span data-ttu-id="79127-120">4</span><span class="sxs-lookup"><span data-stu-id="79127-120">3</span></span>|<span data-ttu-id="79127-121">ПодКлючается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="79127-121">Connects to O365 Dedicated Exchange environment.</span></span>|



