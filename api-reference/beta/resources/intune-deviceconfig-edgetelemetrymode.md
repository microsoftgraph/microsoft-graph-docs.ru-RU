---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d59726f14398068d5b902ba8ca1f05849761216b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385996"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="3c7f4-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="3c7f4-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="3c7f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c7f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c7f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c7f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c7f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c7f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c7f4-107">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="3c7f4-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="3c7f4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3c7f4-108">Members</span></span>
|<span data-ttu-id="3c7f4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3c7f4-109">Member</span></span>|<span data-ttu-id="3c7f4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3c7f4-110">Value</span></span>|<span data-ttu-id="3c7f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c7f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c7f4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3c7f4-112">notConfigured</span></span>|<span data-ttu-id="3c7f4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3c7f4-113">0</span></span>|<span data-ttu-id="3c7f4-114">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="3c7f4-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="3c7f4-115">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="3c7f4-115">intranet</span></span>|<span data-ttu-id="3c7f4-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3c7f4-116">1</span></span>|<span data-ttu-id="3c7f4-117">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="3c7f4-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="3c7f4-118">свойства</span><span class="sxs-lookup"><span data-stu-id="3c7f4-118">internet</span></span>|<span data-ttu-id="3c7f4-119">2</span><span class="sxs-lookup"><span data-stu-id="3c7f4-119">2</span></span>|<span data-ttu-id="3c7f4-120">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="3c7f4-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="3c7f4-121">интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="3c7f4-121">intranetAndInternet</span></span>|<span data-ttu-id="3c7f4-122">4</span><span class="sxs-lookup"><span data-stu-id="3c7f4-122">3</span></span>|<span data-ttu-id="3c7f4-123">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="3c7f4-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



