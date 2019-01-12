---
title: Тип перечисления deviceManagementExchangeConnectorSyncType
description: Тип соединителя Exchange запрошенную синхронизацию.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5af14006bd6f3cc8733faecc8e0219cc02e7fcd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983284"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="b2c80-103">Тип перечисления deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="b2c80-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="b2c80-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2c80-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2c80-105">Тип соединителя Exchange запрошенную синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="b2c80-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="b2c80-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b2c80-106">Members</span></span>
|<span data-ttu-id="b2c80-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b2c80-107">Member</span></span>|<span data-ttu-id="b2c80-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b2c80-108">Value</span></span>|<span data-ttu-id="b2c80-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2c80-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c80-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="b2c80-110">fullSync</span></span>|<span data-ttu-id="b2c80-111">0</span><span class="sxs-lookup"><span data-stu-id="b2c80-111">0</span></span>|<span data-ttu-id="b2c80-112">Обнаружение всех устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2c80-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="b2c80-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="b2c80-113">deltaSync</span></span>|<span data-ttu-id="b2c80-114">1</span><span class="sxs-lookup"><span data-stu-id="b2c80-114">1</span></span>|<span data-ttu-id="b2c80-115">Обнаружение только устройств в Exchange, которая обновления во время синхронизации дельты.</span><span class="sxs-lookup"><span data-stu-id="b2c80-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



