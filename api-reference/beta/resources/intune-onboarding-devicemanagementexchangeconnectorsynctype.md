---
title: Тип перечисления deviceManagementExchangeConnectorSyncType
description: Тип соединителя Exchange запрошенную синхронизацию.
ms.openlocfilehash: 96117a7d11ca49cd39b60cb932bbb985ccf50d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077765"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="f198d-103">Тип перечисления deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="f198d-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="f198d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f198d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f198d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f198d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f198d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f198d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f198d-107">Тип соединителя Exchange запрошенную синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="f198d-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="f198d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f198d-108">Members</span></span>
|<span data-ttu-id="f198d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f198d-109">Member</span></span>|<span data-ttu-id="f198d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f198d-110">Value</span></span>|<span data-ttu-id="f198d-111">Description</span><span class="sxs-lookup"><span data-stu-id="f198d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f198d-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="f198d-112">fullSync</span></span>|<span data-ttu-id="f198d-113">0</span><span class="sxs-lookup"><span data-stu-id="f198d-113">0</span></span>|<span data-ttu-id="f198d-114">Обнаружение всех устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f198d-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="f198d-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="f198d-115">deltaSync</span></span>|<span data-ttu-id="f198d-116">1</span><span class="sxs-lookup"><span data-stu-id="f198d-116">1</span></span>|<span data-ttu-id="f198d-117">Обнаружение только устройств в Exchange, которая обновления во время синхронизации дельты.</span><span class="sxs-lookup"><span data-stu-id="f198d-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





