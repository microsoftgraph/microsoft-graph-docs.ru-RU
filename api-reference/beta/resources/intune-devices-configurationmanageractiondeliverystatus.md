---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bbe36a6f7e346467d35bf997817241d7f30ef6df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214632"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="3754f-103">тип перечисления Конфигуратионманажерактионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="3754f-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="3754f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3754f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3754f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3754f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3754f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3754f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3754f-107">Состояние доставки действия устройства Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="3754f-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="3754f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3754f-108">Members</span></span>
|<span data-ttu-id="3754f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3754f-109">Member</span></span>|<span data-ttu-id="3754f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3754f-110">Value</span></span>|<span data-ttu-id="3754f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3754f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3754f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3754f-112">unknown</span></span>|<span data-ttu-id="3754f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3754f-113">0</span></span>|<span data-ttu-id="3754f-114">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="3754f-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="3754f-115">пендингделивери</span><span class="sxs-lookup"><span data-stu-id="3754f-115">pendingDelivery</span></span>|<span data-ttu-id="3754f-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3754f-116">1</span></span>|<span data-ttu-id="3754f-117">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="3754f-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="3754f-118">деливередтоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="3754f-118">deliveredToConnectorService</span></span>|<span data-ttu-id="3754f-119">2</span><span class="sxs-lookup"><span data-stu-id="3754f-119">2</span></span>|<span data-ttu-id="3754f-120">Действие отправляется в службу соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="3754f-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="3754f-121">фаиледтоделивертоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="3754f-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="3754f-122">4</span><span class="sxs-lookup"><span data-stu-id="3754f-122">3</span></span>|<span data-ttu-id="3754f-123">Не удалось отправить действие службе соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="3754f-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="3754f-124">деливередтунпремисессервер</span><span class="sxs-lookup"><span data-stu-id="3754f-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="3754f-125">4 </span><span class="sxs-lookup"><span data-stu-id="3754f-125">4</span></span>|<span data-ttu-id="3754f-126">Действие доставляется на локальный сервер Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="3754f-126">Action is delivered to ConfigurationManager on-prem server</span></span>|




