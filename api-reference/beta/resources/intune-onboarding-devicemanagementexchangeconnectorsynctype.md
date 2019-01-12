---
title: Тип перечисления deviceManagementExchangeConnectorSyncType
description: Тип соединителя Exchange запрошенную синхронизацию.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac6f54c2a09752df2382ae6b27f9dc9387262acf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912731"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="8f1ca-103">Тип перечисления deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="8f1ca-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="8f1ca-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f1ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f1ca-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f1ca-107">Тип соединителя Exchange запрошенную синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="8f1ca-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f1ca-108">Members</span></span>
|<span data-ttu-id="8f1ca-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f1ca-109">Member</span></span>|<span data-ttu-id="8f1ca-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8f1ca-110">Value</span></span>|<span data-ttu-id="8f1ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f1ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1ca-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="8f1ca-112">fullSync</span></span>|<span data-ttu-id="8f1ca-113">0</span><span class="sxs-lookup"><span data-stu-id="8f1ca-113">0</span></span>|<span data-ttu-id="8f1ca-114">Обнаружение всех устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="8f1ca-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="8f1ca-115">deltaSync</span></span>|<span data-ttu-id="8f1ca-116">1</span><span class="sxs-lookup"><span data-stu-id="8f1ca-116">1</span></span>|<span data-ttu-id="8f1ca-117">Обнаружение только устройств в Exchange, которая обновления во время синхронизации дельты.</span><span class="sxs-lookup"><span data-stu-id="8f1ca-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





