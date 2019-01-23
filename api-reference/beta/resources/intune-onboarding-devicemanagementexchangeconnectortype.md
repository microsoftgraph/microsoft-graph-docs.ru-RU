---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20eb1053d3dbf6cb657313f0c68f6c6c84804848
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398984"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="e6147-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="e6147-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="e6147-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6147-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6147-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6147-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6147-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6147-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6147-107">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6147-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="e6147-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e6147-108">Members</span></span>
|<span data-ttu-id="e6147-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e6147-109">Member</span></span>|<span data-ttu-id="e6147-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e6147-110">Value</span></span>|<span data-ttu-id="e6147-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6147-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6147-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="e6147-112">onPremises</span></span>|<span data-ttu-id="e6147-113">0</span><span class="sxs-lookup"><span data-stu-id="e6147-113">0</span></span>|<span data-ttu-id="e6147-114">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6147-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="e6147-115">размещенные</span><span class="sxs-lookup"><span data-stu-id="e6147-115">hosted</span></span>|<span data-ttu-id="e6147-116">1</span><span class="sxs-lookup"><span data-stu-id="e6147-116">1</span></span>|<span data-ttu-id="e6147-117">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="e6147-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="e6147-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="e6147-118">serviceToService</span></span>|<span data-ttu-id="e6147-119">2</span><span class="sxs-lookup"><span data-stu-id="e6147-119">2</span></span>|<span data-ttu-id="e6147-120">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="e6147-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="e6147-121">выделенные</span><span class="sxs-lookup"><span data-stu-id="e6147-121">dedicated</span></span>|<span data-ttu-id="e6147-122">3</span><span class="sxs-lookup"><span data-stu-id="e6147-122">3</span></span>|<span data-ttu-id="e6147-123">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="e6147-123">Connects to O365 Dedicated Exchange environment.</span></span>|




