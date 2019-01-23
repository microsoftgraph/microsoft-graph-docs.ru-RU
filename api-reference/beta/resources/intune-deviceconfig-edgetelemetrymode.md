---
title: Тип перечисления edgeTelemetryMode
description: Тип просмотра данных, отправляемых Microsoft 365 аналитики
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430740"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="45cb5-103">Тип перечисления edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="45cb5-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="45cb5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45cb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45cb5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45cb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45cb5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45cb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45cb5-107">Тип просмотра данных, отправляемых Microsoft 365 аналитики</span><span class="sxs-lookup"><span data-stu-id="45cb5-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="45cb5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="45cb5-108">Members</span></span>
|<span data-ttu-id="45cb5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="45cb5-109">Member</span></span>|<span data-ttu-id="45cb5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="45cb5-110">Value</span></span>|<span data-ttu-id="45cb5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="45cb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45cb5-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="45cb5-112">notConfigured</span></span>|<span data-ttu-id="45cb5-113">0</span><span class="sxs-lookup"><span data-stu-id="45cb5-113">0</span></span>|<span data-ttu-id="45cb5-114">По умолчанию — без данных телеметрии собраны или отправки</span><span class="sxs-lookup"><span data-stu-id="45cb5-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="45cb5-115">интрасеть</span><span class="sxs-lookup"><span data-stu-id="45cb5-115">intranet</span></span>|<span data-ttu-id="45cb5-116">1</span><span class="sxs-lookup"><span data-stu-id="45cb5-116">1</span></span>|<span data-ttu-id="45cb5-117">Разрешить отправку только журнал интрасети: только отправка, просмотр данных журнала для сайтов интрасети</span><span class="sxs-lookup"><span data-stu-id="45cb5-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="45cb5-118">internet</span><span class="sxs-lookup"><span data-stu-id="45cb5-118">internet</span></span>|<span data-ttu-id="45cb5-119">2</span><span class="sxs-lookup"><span data-stu-id="45cb5-119">2</span></span>|<span data-ttu-id="45cb5-120">Разрешить отправку только журнал Интернета: только отправка, просмотр данных журнала для веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="45cb5-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="45cb5-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="45cb5-121">intranetAndInternet</span></span>|<span data-ttu-id="45cb5-122">3</span><span class="sxs-lookup"><span data-stu-id="45cb5-122">3</span></span>|<span data-ttu-id="45cb5-123">Разрешить отправку интрасеть и Интернет журнала: отправка, просмотр данных журнала для сайтов Интернета и интрасети</span><span class="sxs-lookup"><span data-stu-id="45cb5-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




