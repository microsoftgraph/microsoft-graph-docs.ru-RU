---
title: Тип перечисления deviceManagementExchangeConnectorStatus
description: Текущее состояние соединителя Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16181c49b05c74ef680f456b4bffd11b435299fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397773"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="34beb-103">Тип перечисления deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="34beb-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="34beb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34beb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34beb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34beb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34beb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34beb-107">Текущее состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="34beb-107">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="34beb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="34beb-108">Members</span></span>
|<span data-ttu-id="34beb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="34beb-109">Member</span></span>|<span data-ttu-id="34beb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="34beb-110">Value</span></span>|<span data-ttu-id="34beb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34beb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34beb-112">none</span><span class="sxs-lookup"><span data-stu-id="34beb-112">none</span></span>|<span data-ttu-id="34beb-113">0</span><span class="sxs-lookup"><span data-stu-id="34beb-113">0</span></span>|<span data-ttu-id="34beb-114">Не соединитель отсутствует.</span><span class="sxs-lookup"><span data-stu-id="34beb-114">No Connector exists.</span></span>|
|<span data-ttu-id="34beb-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="34beb-115">connectionPending</span></span>|<span data-ttu-id="34beb-116">1</span><span class="sxs-lookup"><span data-stu-id="34beb-116">1</span></span>|<span data-ttu-id="34beb-117">Ожидание подключения в среду Exchange.</span><span class="sxs-lookup"><span data-stu-id="34beb-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="34beb-118">подключение</span><span class="sxs-lookup"><span data-stu-id="34beb-118">connected</span></span>|<span data-ttu-id="34beb-119">2</span><span class="sxs-lookup"><span data-stu-id="34beb-119">2</span></span>|<span data-ttu-id="34beb-120">Подключения к среде Exchange</span><span class="sxs-lookup"><span data-stu-id="34beb-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="34beb-121">отключен</span><span class="sxs-lookup"><span data-stu-id="34beb-121">disconnected</span></span>|<span data-ttu-id="34beb-122">3</span><span class="sxs-lookup"><span data-stu-id="34beb-122">3</span></span>|<span data-ttu-id="34beb-123">Отключение от среды Exchange</span><span class="sxs-lookup"><span data-stu-id="34beb-123">Disconnected from the Exchange Environment</span></span>|




