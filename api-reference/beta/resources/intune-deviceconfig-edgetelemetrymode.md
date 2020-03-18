---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d94fb93dcb7e95e0ba1ae7581ce5f26f44496002
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791837"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="1eafc-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="1eafc-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="1eafc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1eafc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eafc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1eafc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eafc-106">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="1eafc-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="1eafc-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1eafc-107">Members</span></span>
|<span data-ttu-id="1eafc-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1eafc-108">Member</span></span>|<span data-ttu-id="1eafc-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1eafc-109">Value</span></span>|<span data-ttu-id="1eafc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1eafc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eafc-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1eafc-111">notConfigured</span></span>|<span data-ttu-id="1eafc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1eafc-112">0</span></span>|<span data-ttu-id="1eafc-113">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="1eafc-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="1eafc-114">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="1eafc-114">intranet</span></span>|<span data-ttu-id="1eafc-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1eafc-115">1</span></span>|<span data-ttu-id="1eafc-116">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="1eafc-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="1eafc-117">свойства</span><span class="sxs-lookup"><span data-stu-id="1eafc-117">internet</span></span>|<span data-ttu-id="1eafc-118">2</span><span class="sxs-lookup"><span data-stu-id="1eafc-118">2</span></span>|<span data-ttu-id="1eafc-119">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="1eafc-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="1eafc-120">интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="1eafc-120">intranetAndInternet</span></span>|<span data-ttu-id="1eafc-121">4</span><span class="sxs-lookup"><span data-stu-id="1eafc-121">3</span></span>|<span data-ttu-id="1eafc-122">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="1eafc-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



