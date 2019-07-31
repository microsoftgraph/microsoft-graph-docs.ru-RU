---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: feeecf706a262d38bf956a49bc27d5d32e1e8ddb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001406"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="99c16-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="99c16-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="99c16-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c16-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99c16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c16-106">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="99c16-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="99c16-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="99c16-107">Members</span></span>
|<span data-ttu-id="99c16-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="99c16-108">Member</span></span>|<span data-ttu-id="99c16-109">Значение</span><span class="sxs-lookup"><span data-stu-id="99c16-109">Value</span></span>|<span data-ttu-id="99c16-110">Описание</span><span class="sxs-lookup"><span data-stu-id="99c16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c16-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="99c16-111">notConfigured</span></span>|<span data-ttu-id="99c16-112">нуль</span><span class="sxs-lookup"><span data-stu-id="99c16-112">0</span></span>|<span data-ttu-id="99c16-113">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="99c16-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="99c16-114">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="99c16-114">intranet</span></span>|<span data-ttu-id="99c16-115">1,1</span><span class="sxs-lookup"><span data-stu-id="99c16-115">1</span></span>|<span data-ttu-id="99c16-116">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="99c16-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="99c16-117">свойства</span><span class="sxs-lookup"><span data-stu-id="99c16-117">internet</span></span>|<span data-ttu-id="99c16-118">2</span><span class="sxs-lookup"><span data-stu-id="99c16-118">2</span></span>|<span data-ttu-id="99c16-119">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="99c16-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="99c16-120">Интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="99c16-120">intranetAndInternet</span></span>|<span data-ttu-id="99c16-121">4</span><span class="sxs-lookup"><span data-stu-id="99c16-121">3</span></span>|<span data-ttu-id="99c16-122">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="99c16-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





