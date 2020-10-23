---
title: тип перечисления Девицеманажементексчанжеконнекторсинктипе
description: Тип запрошенной синхронизации соединителя Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6598b2bc7a6ee4c75c201ec86718f933696f7f1c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736102"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="cf19a-103">тип перечисления Девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="cf19a-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="cf19a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf19a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf19a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf19a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf19a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf19a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf19a-107">Тип запрошенной синхронизации соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf19a-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="cf19a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cf19a-108">Members</span></span>
|<span data-ttu-id="cf19a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cf19a-109">Member</span></span>|<span data-ttu-id="cf19a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cf19a-110">Value</span></span>|<span data-ttu-id="cf19a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cf19a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf19a-112">Профиль выполнения FullSync</span><span class="sxs-lookup"><span data-stu-id="cf19a-112">fullSync</span></span>|<span data-ttu-id="cf19a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="cf19a-113">0</span></span>|<span data-ttu-id="cf19a-114">Обнаружение устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf19a-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="cf19a-115">Профиль выполнения deltasync</span><span class="sxs-lookup"><span data-stu-id="cf19a-115">deltaSync</span></span>|<span data-ttu-id="cf19a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="cf19a-116">1</span></span>|<span data-ttu-id="cf19a-117">Обнаружение только устройства в Exchange, которое обновилось в окне "разностная синхронизация".</span><span class="sxs-lookup"><span data-stu-id="cf19a-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





