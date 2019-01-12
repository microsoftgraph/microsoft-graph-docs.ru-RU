---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: d1ba4d2cd9be740b23502ec4c0154caa2be07f3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948532"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="227d8-103">Тип перечисления diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="227d8-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="227d8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="227d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="227d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="227d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="227d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="227d8-107">Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.</span><span class="sxs-lookup"><span data-stu-id="227d8-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="227d8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="227d8-108">Members</span></span>
|<span data-ttu-id="227d8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="227d8-109">Member</span></span>|<span data-ttu-id="227d8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="227d8-110">Value</span></span>|<span data-ttu-id="227d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="227d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227d8-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="227d8-112">userDefined</span></span>|<span data-ttu-id="227d8-113">0</span><span class="sxs-lookup"><span data-stu-id="227d8-113">0</span></span>|<span data-ttu-id="227d8-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="227d8-114">Allow the user to set.</span></span>|
|<span data-ttu-id="227d8-115">Нет</span><span class="sxs-lookup"><span data-stu-id="227d8-115">none</span></span>|<span data-ttu-id="227d8-116">1</span><span class="sxs-lookup"><span data-stu-id="227d8-116">1</span></span>|<span data-ttu-id="227d8-117">Данные телеметрии отправляется компоненты операционной системы.</span><span class="sxs-lookup"><span data-stu-id="227d8-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="227d8-118">Примечание: Это значение применимо только к устройствам, enterprise и сервера.</span><span class="sxs-lookup"><span data-stu-id="227d8-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="227d8-119">С помощью этого параметра на других устройствах эквивалентно параметру значение 1.</span><span class="sxs-lookup"><span data-stu-id="227d8-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="227d8-120">Базовая</span><span class="sxs-lookup"><span data-stu-id="227d8-120">basic</span></span>|<span data-ttu-id="227d8-121">2</span><span class="sxs-lookup"><span data-stu-id="227d8-121">2</span></span>|<span data-ttu-id="227d8-122">Отправляет данные телеметрии для базовой.</span><span class="sxs-lookup"><span data-stu-id="227d8-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="227d8-123">Enhanced</span><span class="sxs-lookup"><span data-stu-id="227d8-123">enhanced</span></span>|<span data-ttu-id="227d8-124">3</span><span class="sxs-lookup"><span data-stu-id="227d8-124">3</span></span>|<span data-ttu-id="227d8-125">Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.</span><span class="sxs-lookup"><span data-stu-id="227d8-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="227d8-126">Полный</span><span class="sxs-lookup"><span data-stu-id="227d8-126">full</span></span>|<span data-ttu-id="227d8-127">4</span><span class="sxs-lookup"><span data-stu-id="227d8-127">4</span></span>|<span data-ttu-id="227d8-128">Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.</span><span class="sxs-lookup"><span data-stu-id="227d8-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





