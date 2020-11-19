---
title: тип перечисления Девицеманажементексчанжеконнектортипе
description: Тип соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ee6b98f668035f16f65ce366159d7d455ea6ae3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288189"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="5aad1-103">тип перечисления Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="5aad1-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="5aad1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aad1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5aad1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5aad1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5aad1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5aad1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5aad1-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aad1-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="5aad1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5aad1-108">Members</span></span>
|<span data-ttu-id="5aad1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5aad1-109">Member</span></span>|<span data-ttu-id="5aad1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5aad1-110">Value</span></span>|<span data-ttu-id="5aad1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5aad1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aad1-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="5aad1-112">onPremises</span></span>|<span data-ttu-id="5aad1-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5aad1-113">0</span></span>|<span data-ttu-id="5aad1-114">Подключается к локальной среде Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aad1-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="5aad1-115">хост</span><span class="sxs-lookup"><span data-stu-id="5aad1-115">hosted</span></span>|<span data-ttu-id="5aad1-116">1,1</span><span class="sxs-lookup"><span data-stu-id="5aad1-116">1</span></span>|<span data-ttu-id="5aad1-117">Подключается к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="5aad1-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5aad1-118">сервицетосервице</span><span class="sxs-lookup"><span data-stu-id="5aad1-118">serviceToService</span></span>|<span data-ttu-id="5aad1-119">2</span><span class="sxs-lookup"><span data-stu-id="5aad1-119">2</span></span>|<span data-ttu-id="5aad1-120">Служба Intune подключается напрямую к среде Exchange с несколькими клиентами Office 365</span><span class="sxs-lookup"><span data-stu-id="5aad1-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5aad1-121">уполномочен</span><span class="sxs-lookup"><span data-stu-id="5aad1-121">dedicated</span></span>|<span data-ttu-id="5aad1-122">4</span><span class="sxs-lookup"><span data-stu-id="5aad1-122">3</span></span>|<span data-ttu-id="5aad1-123">Подключается к выделенной среде Exchange O365.</span><span class="sxs-lookup"><span data-stu-id="5aad1-123">Connects to O365 Dedicated Exchange environment.</span></span>|




