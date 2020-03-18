---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785093"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="4fe74-103">тип перечисления Конфигуратионманажерактионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="4fe74-103">configurationManagerActionDeliveryStatus enum type</span></span>

> <span data-ttu-id="4fe74-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fe74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fe74-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fe74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe74-106">Состояние доставки действия устройства Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="4fe74-106">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="4fe74-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4fe74-107">Members</span></span>
|<span data-ttu-id="4fe74-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4fe74-108">Member</span></span>|<span data-ttu-id="4fe74-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4fe74-109">Value</span></span>|<span data-ttu-id="4fe74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4fe74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fe74-111">unknown</span><span class="sxs-lookup"><span data-stu-id="4fe74-111">unknown</span></span>|<span data-ttu-id="4fe74-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4fe74-112">0</span></span>|<span data-ttu-id="4fe74-113">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="4fe74-113">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="4fe74-114">пендингделивери</span><span class="sxs-lookup"><span data-stu-id="4fe74-114">pendingDelivery</span></span>|<span data-ttu-id="4fe74-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4fe74-115">1</span></span>|<span data-ttu-id="4fe74-116">Ожидание для доставки действия в Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="4fe74-116">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="4fe74-117">деливередтоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="4fe74-117">deliveredToConnectorService</span></span>|<span data-ttu-id="4fe74-118">2</span><span class="sxs-lookup"><span data-stu-id="4fe74-118">2</span></span>|<span data-ttu-id="4fe74-119">Действие отправляется в службу соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="4fe74-119">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="4fe74-120">фаиледтоделивертоконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="4fe74-120">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="4fe74-121">4</span><span class="sxs-lookup"><span data-stu-id="4fe74-121">3</span></span>|<span data-ttu-id="4fe74-122">Не удалось отправить действие службе соединителя Конфигуратионманажер (Cloud)</span><span class="sxs-lookup"><span data-stu-id="4fe74-122">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="4fe74-123">деливередтунпремисессервер</span><span class="sxs-lookup"><span data-stu-id="4fe74-123">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="4fe74-124">4 </span><span class="sxs-lookup"><span data-stu-id="4fe74-124">4</span></span>|<span data-ttu-id="4fe74-125">Действие доставляется на локальный сервер Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="4fe74-125">Action is delivered to ConfigurationManager on-prem server</span></span>|



