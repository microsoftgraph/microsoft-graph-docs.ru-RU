---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
localization_priority: Normal
ms.openlocfilehash: 3be69b4be25ece2ced611c028a855347e4dba66e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871535"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="e2e07-103">Тип перечисления diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="e2e07-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="e2e07-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2e07-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2e07-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2e07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2e07-107">Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.</span><span class="sxs-lookup"><span data-stu-id="e2e07-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="e2e07-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e2e07-108">Members</span></span>
|<span data-ttu-id="e2e07-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e2e07-109">Member</span></span>|<span data-ttu-id="e2e07-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e2e07-110">Value</span></span>|<span data-ttu-id="e2e07-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e07-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="e2e07-112">userDefined</span></span>|<span data-ttu-id="e2e07-113">0</span><span class="sxs-lookup"><span data-stu-id="e2e07-113">0</span></span>|<span data-ttu-id="e2e07-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="e2e07-114">Allow the user to set.</span></span>|
|<span data-ttu-id="e2e07-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e2e07-115">none</span></span>|<span data-ttu-id="e2e07-116">1</span><span class="sxs-lookup"><span data-stu-id="e2e07-116">1</span></span>|<span data-ttu-id="e2e07-117">Данные телеметрии отправляется компоненты операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e2e07-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="e2e07-118">Примечание: Это значение применимо только к устройствам, enterprise и сервера.</span><span class="sxs-lookup"><span data-stu-id="e2e07-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="e2e07-119">С помощью этого параметра на других устройствах эквивалентно параметру значение 1.</span><span class="sxs-lookup"><span data-stu-id="e2e07-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="e2e07-120">Базовая</span><span class="sxs-lookup"><span data-stu-id="e2e07-120">basic</span></span>|<span data-ttu-id="e2e07-121">2</span><span class="sxs-lookup"><span data-stu-id="e2e07-121">2</span></span>|<span data-ttu-id="e2e07-122">Отправляет данные телеметрии для базовой.</span><span class="sxs-lookup"><span data-stu-id="e2e07-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="e2e07-123">Enhanced</span><span class="sxs-lookup"><span data-stu-id="e2e07-123">enhanced</span></span>|<span data-ttu-id="e2e07-124">3</span><span class="sxs-lookup"><span data-stu-id="e2e07-124">3</span></span>|<span data-ttu-id="e2e07-125">Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.</span><span class="sxs-lookup"><span data-stu-id="e2e07-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="e2e07-126">Полный</span><span class="sxs-lookup"><span data-stu-id="e2e07-126">full</span></span>|<span data-ttu-id="e2e07-127">4</span><span class="sxs-lookup"><span data-stu-id="e2e07-127">4</span></span>|<span data-ttu-id="e2e07-128">Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.</span><span class="sxs-lookup"><span data-stu-id="e2e07-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





