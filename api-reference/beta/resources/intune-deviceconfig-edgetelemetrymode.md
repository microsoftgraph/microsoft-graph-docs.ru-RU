---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fa6ea5a2bf187a753705b369f3f8a2558860c3eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357273"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="b8e1b-103">тип перечисления Еджетелеметримоде</span><span class="sxs-lookup"><span data-stu-id="b8e1b-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="b8e1b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8e1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e1b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8e1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e1b-106">Тип данных просмотра, отправляемых в Microsoft 365 Analytics</span><span class="sxs-lookup"><span data-stu-id="b8e1b-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="b8e1b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8e1b-107">Members</span></span>
|<span data-ttu-id="b8e1b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8e1b-108">Member</span></span>|<span data-ttu-id="b8e1b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b8e1b-109">Value</span></span>|<span data-ttu-id="b8e1b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8e1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e1b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8e1b-111">notConfigured</span></span>|<span data-ttu-id="b8e1b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b8e1b-112">0</span></span>|<span data-ttu-id="b8e1b-113">По умолчанию — данные телеметрии не собраны и не отправляются</span><span class="sxs-lookup"><span data-stu-id="b8e1b-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="b8e1b-114">Внутренняя</span><span class="sxs-lookup"><span data-stu-id="b8e1b-114">intranet</span></span>|<span data-ttu-id="b8e1b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b8e1b-115">1</span></span>|<span data-ttu-id="b8e1b-116">Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="b8e1b-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="b8e1b-117">свойства</span><span class="sxs-lookup"><span data-stu-id="b8e1b-117">internet</span></span>|<span data-ttu-id="b8e1b-118">2</span><span class="sxs-lookup"><span data-stu-id="b8e1b-118">2</span></span>|<span data-ttu-id="b8e1b-119">Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов</span><span class="sxs-lookup"><span data-stu-id="b8e1b-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="b8e1b-120">интранетандинтернет</span><span class="sxs-lookup"><span data-stu-id="b8e1b-120">intranetAndInternet</span></span>|<span data-ttu-id="b8e1b-121">4</span><span class="sxs-lookup"><span data-stu-id="b8e1b-121">3</span></span>|<span data-ttu-id="b8e1b-122">Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="b8e1b-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



