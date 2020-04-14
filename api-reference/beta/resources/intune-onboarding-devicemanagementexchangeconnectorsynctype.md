---
title: тип перечисления Девицеманажементексчанжеконнекторсинктипе
description: Тип запрошенной синхронизации соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f4cde0b7d1d0ae6c728140c8e6b045b5a497a841
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448070"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="fc564-103">тип перечисления Девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="fc564-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="fc564-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc564-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc564-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc564-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc564-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc564-107">Тип запрошенной синхронизации соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc564-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="fc564-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fc564-108">Members</span></span>
|<span data-ttu-id="fc564-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fc564-109">Member</span></span>|<span data-ttu-id="fc564-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fc564-110">Value</span></span>|<span data-ttu-id="fc564-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc564-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc564-112">Профиль выполнения FullSync</span><span class="sxs-lookup"><span data-stu-id="fc564-112">fullSync</span></span>|<span data-ttu-id="fc564-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fc564-113">0</span></span>|<span data-ttu-id="fc564-114">Обнаружение устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc564-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="fc564-115">Профиль выполнения deltasync</span><span class="sxs-lookup"><span data-stu-id="fc564-115">deltaSync</span></span>|<span data-ttu-id="fc564-116">1,1</span><span class="sxs-lookup"><span data-stu-id="fc564-116">1</span></span>|<span data-ttu-id="fc564-117">Обнаружение только устройства в Exchange, которое обновилось в окне "разностная синхронизация".</span><span class="sxs-lookup"><span data-stu-id="fc564-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



