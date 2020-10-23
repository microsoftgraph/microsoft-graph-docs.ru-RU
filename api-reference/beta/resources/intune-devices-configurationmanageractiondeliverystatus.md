---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09c7b1be3a5fdfc33a064d2a9208daa68ba4263e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733988"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="a263b-103">тип перечисления Конфигуратионманажерактионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="a263b-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="a263b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a263b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a263b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a263b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a263b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a263b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a263b-107">Состояние доставки действия устройства Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="a263b-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="a263b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a263b-108">Members</span></span>
|<span data-ttu-id="a263b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a263b-109">Member</span></span>|<span data-ttu-id="a263b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a263b-110">Value</span></span>|<span data-ttu-id="a263b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a263b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a263b-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a263b-112">unknown</span></span>|<span data-ttu-id="a263b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a263b-113">0</span></span>|<span data-ttu-id="a263b-114">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="a263b-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="a263b-115">пендингделивери</span><span class="sxs-lookup"><span data-stu-id="a263b-115">pendingDelivery</span></span>|<span data-ttu-id="a263b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a263b-116">1</span></span>|<span data-ttu-id="a263b-117">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="a263b-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="a263b-118">деливередтоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="a263b-118">deliveredToConnectorService</span></span>|<span data-ttu-id="a263b-119">2</span><span class="sxs-lookup"><span data-stu-id="a263b-119">2</span></span>|<span data-ttu-id="a263b-120">Действие отправляется в службу соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="a263b-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="a263b-121">фаиледтоделивертоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="a263b-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="a263b-122">4</span><span class="sxs-lookup"><span data-stu-id="a263b-122">3</span></span>|<span data-ttu-id="a263b-123">Не удалось отправить действие службе соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="a263b-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="a263b-124">деливередтунпремисессервер</span><span class="sxs-lookup"><span data-stu-id="a263b-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="a263b-125">4 </span><span class="sxs-lookup"><span data-stu-id="a263b-125">4</span></span>|<span data-ttu-id="a263b-126">Действие доставляется на локальный сервер Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="a263b-126">Action is delivered to ConfigurationManager on-prem server</span></span>|





