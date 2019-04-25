---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358832db83e5f5b3e1fb0f5457f480d21ded996
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583524"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="aac22-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="aac22-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="aac22-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aac22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac22-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="aac22-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="aac22-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="aac22-106">Members</span></span>
|<span data-ttu-id="aac22-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="aac22-107">Member</span></span>|<span data-ttu-id="aac22-108">Значение</span><span class="sxs-lookup"><span data-stu-id="aac22-108">Value</span></span>|<span data-ttu-id="aac22-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aac22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac22-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="aac22-110">onPremises</span></span>|<span data-ttu-id="aac22-111">нуль</span><span class="sxs-lookup"><span data-stu-id="aac22-111">0</span></span>|<span data-ttu-id="aac22-112">ПодКлючается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="aac22-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="aac22-113">хост</span><span class="sxs-lookup"><span data-stu-id="aac22-113">hosted</span></span>|<span data-ttu-id="aac22-114">1 </span><span class="sxs-lookup"><span data-stu-id="aac22-114">1</span></span>|<span data-ttu-id="aac22-115">ПодКлючается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="aac22-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="aac22-116">Сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="aac22-116">serviceToService</span></span>|<span data-ttu-id="aac22-117">2 </span><span class="sxs-lookup"><span data-stu-id="aac22-117">2</span></span>|<span data-ttu-id="aac22-118">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="aac22-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="aac22-119">уполномочен</span><span class="sxs-lookup"><span data-stu-id="aac22-119">dedicated</span></span>|<span data-ttu-id="aac22-120">3 </span><span class="sxs-lookup"><span data-stu-id="aac22-120">3</span></span>|<span data-ttu-id="aac22-121">ПодКлючается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="aac22-121">Connects to O365 Dedicated Exchange environment.</span></span>|



