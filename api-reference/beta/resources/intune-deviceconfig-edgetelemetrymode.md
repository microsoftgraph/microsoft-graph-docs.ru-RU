---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a2ad7e97f9d957e4da278dad6dde3f686445e1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198883"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="00940-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="00940-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="00940-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00940-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00940-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00940-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00940-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00940-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00940-107">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="00940-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="00940-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="00940-108">Members</span></span>
|<span data-ttu-id="00940-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="00940-109">Member</span></span>|<span data-ttu-id="00940-110">Значение</span><span class="sxs-lookup"><span data-stu-id="00940-110">Value</span></span>|<span data-ttu-id="00940-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00940-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00940-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="00940-112">notConfigured</span></span>|<span data-ttu-id="00940-113">нуль</span><span class="sxs-lookup"><span data-stu-id="00940-113">0</span></span>|<span data-ttu-id="00940-114">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="00940-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="00940-115">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="00940-115">intranet</span></span>|<span data-ttu-id="00940-116">1,1</span><span class="sxs-lookup"><span data-stu-id="00940-116">1</span></span>|<span data-ttu-id="00940-117">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="00940-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="00940-118">свойства</span><span class="sxs-lookup"><span data-stu-id="00940-118">internet</span></span>|<span data-ttu-id="00940-119">2</span><span class="sxs-lookup"><span data-stu-id="00940-119">2</span></span>|<span data-ttu-id="00940-120">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="00940-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="00940-121">интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="00940-121">intranetAndInternet</span></span>|<span data-ttu-id="00940-122">4</span><span class="sxs-lookup"><span data-stu-id="00940-122">3</span></span>|<span data-ttu-id="00940-123">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="00940-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




