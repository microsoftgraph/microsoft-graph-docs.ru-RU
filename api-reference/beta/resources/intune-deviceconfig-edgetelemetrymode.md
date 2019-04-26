---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566040"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="1ea2d-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="1ea2d-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="1ea2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ea2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ea2d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ea2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ea2d-106">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="1ea2d-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="1ea2d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ea2d-107">Members</span></span>
|<span data-ttu-id="1ea2d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ea2d-108">Member</span></span>|<span data-ttu-id="1ea2d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1ea2d-109">Value</span></span>|<span data-ttu-id="1ea2d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ea2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea2d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1ea2d-111">notConfigured</span></span>|<span data-ttu-id="1ea2d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1ea2d-112">0</span></span>|<span data-ttu-id="1ea2d-113">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="1ea2d-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="1ea2d-114">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="1ea2d-114">intranet</span></span>|<span data-ttu-id="1ea2d-115">1 </span><span class="sxs-lookup"><span data-stu-id="1ea2d-115">1</span></span>|<span data-ttu-id="1ea2d-116">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="1ea2d-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="1ea2d-117">свойства</span><span class="sxs-lookup"><span data-stu-id="1ea2d-117">internet</span></span>|<span data-ttu-id="1ea2d-118">2 </span><span class="sxs-lookup"><span data-stu-id="1ea2d-118">2</span></span>|<span data-ttu-id="1ea2d-119">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="1ea2d-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="1ea2d-120">Интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="1ea2d-120">intranetAndInternet</span></span>|<span data-ttu-id="1ea2d-121">3 </span><span class="sxs-lookup"><span data-stu-id="1ea2d-121">3</span></span>|<span data-ttu-id="1ea2d-122">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="1ea2d-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





