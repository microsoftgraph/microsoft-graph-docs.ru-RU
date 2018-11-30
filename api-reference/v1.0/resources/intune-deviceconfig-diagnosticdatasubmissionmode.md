---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
ms.openlocfilehash: b09a4bf334af5981c3ce6dabbab0ac64e2b24887
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027464"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="6ff39-103">Тип перечисления diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="6ff39-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="6ff39-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ff39-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ff39-105">Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.</span><span class="sxs-lookup"><span data-stu-id="6ff39-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="6ff39-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6ff39-106">Members</span></span>
|<span data-ttu-id="6ff39-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6ff39-107">Member</span></span>|<span data-ttu-id="6ff39-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6ff39-108">Value</span></span>|<span data-ttu-id="6ff39-109">Description</span><span class="sxs-lookup"><span data-stu-id="6ff39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff39-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="6ff39-110">userDefined</span></span>|<span data-ttu-id="6ff39-111">0</span><span class="sxs-lookup"><span data-stu-id="6ff39-111">0</span></span>|<span data-ttu-id="6ff39-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="6ff39-112">Allow the user to set.</span></span>|
|<span data-ttu-id="6ff39-113">Нет</span><span class="sxs-lookup"><span data-stu-id="6ff39-113">none</span></span>|<span data-ttu-id="6ff39-114">1</span><span class="sxs-lookup"><span data-stu-id="6ff39-114">1</span></span>|<span data-ttu-id="6ff39-115">Данные телеметрии отправляется компоненты операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6ff39-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="6ff39-116">Примечание: Это значение применимо только к устройствам, enterprise и сервера.</span><span class="sxs-lookup"><span data-stu-id="6ff39-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="6ff39-117">С помощью этого параметра на других устройствах эквивалентно параметру значение 1.</span><span class="sxs-lookup"><span data-stu-id="6ff39-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="6ff39-118">Базовая</span><span class="sxs-lookup"><span data-stu-id="6ff39-118">basic</span></span>|<span data-ttu-id="6ff39-119">2</span><span class="sxs-lookup"><span data-stu-id="6ff39-119">2</span></span>|<span data-ttu-id="6ff39-120">Отправляет данные телеметрии для базовой.</span><span class="sxs-lookup"><span data-stu-id="6ff39-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="6ff39-121">Enhanced</span><span class="sxs-lookup"><span data-stu-id="6ff39-121">enhanced</span></span>|<span data-ttu-id="6ff39-122">3</span><span class="sxs-lookup"><span data-stu-id="6ff39-122">3</span></span>|<span data-ttu-id="6ff39-123">Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.</span><span class="sxs-lookup"><span data-stu-id="6ff39-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="6ff39-124">Полный</span><span class="sxs-lookup"><span data-stu-id="6ff39-124">full</span></span>|<span data-ttu-id="6ff39-125">4</span><span class="sxs-lookup"><span data-stu-id="6ff39-125">4</span></span>|<span data-ttu-id="6ff39-126">Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.</span><span class="sxs-lookup"><span data-stu-id="6ff39-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



