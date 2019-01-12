---
title: Тип перечисления deviceManagementExchangeConnectorType
description: Тип соединителя Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e9e50a4475ca2d57b3f38567703046588d4fb3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986434"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="a3e6c-103">Тип перечисления deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a3e6c-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="a3e6c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3e6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3e6c-105">Тип соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3e6c-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="a3e6c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3e6c-106">Members</span></span>
|<span data-ttu-id="a3e6c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3e6c-107">Member</span></span>|<span data-ttu-id="a3e6c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a3e6c-108">Value</span></span>|<span data-ttu-id="a3e6c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3e6c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e6c-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="a3e6c-110">onPremises</span></span>|<span data-ttu-id="a3e6c-111">0</span><span class="sxs-lookup"><span data-stu-id="a3e6c-111">0</span></span>|<span data-ttu-id="a3e6c-112">Подключается к локальной среды Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3e6c-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="a3e6c-113">размещенные</span><span class="sxs-lookup"><span data-stu-id="a3e6c-113">hosted</span></span>|<span data-ttu-id="a3e6c-114">1</span><span class="sxs-lookup"><span data-stu-id="a3e6c-114">1</span></span>|<span data-ttu-id="a3e6c-115">Подключается к среде Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="a3e6c-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a3e6c-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="a3e6c-116">serviceToService</span></span>|<span data-ttu-id="a3e6c-117">2</span><span class="sxs-lookup"><span data-stu-id="a3e6c-117">2</span></span>|<span data-ttu-id="a3e6c-118">Служба Intune подключается непосредственно в среду Exchange несколькими клиентами O365</span><span class="sxs-lookup"><span data-stu-id="a3e6c-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a3e6c-119">выделенные</span><span class="sxs-lookup"><span data-stu-id="a3e6c-119">dedicated</span></span>|<span data-ttu-id="a3e6c-120">3</span><span class="sxs-lookup"><span data-stu-id="a3e6c-120">3</span></span>|<span data-ttu-id="a3e6c-121">Подключается к среде Exchange выделенных O365.</span><span class="sxs-lookup"><span data-stu-id="a3e6c-121">Connects to O365 Dedicated Exchange environment.</span></span>|



