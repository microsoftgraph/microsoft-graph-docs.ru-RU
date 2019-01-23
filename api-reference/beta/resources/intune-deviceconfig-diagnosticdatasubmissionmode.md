---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422259"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="8afc5-103">Тип перечисления diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="8afc5-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="8afc5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8afc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8afc5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8afc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8afc5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8afc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8afc5-107">Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.</span><span class="sxs-lookup"><span data-stu-id="8afc5-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="8afc5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8afc5-108">Members</span></span>
|<span data-ttu-id="8afc5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8afc5-109">Member</span></span>|<span data-ttu-id="8afc5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8afc5-110">Value</span></span>|<span data-ttu-id="8afc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8afc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8afc5-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="8afc5-112">userDefined</span></span>|<span data-ttu-id="8afc5-113">0</span><span class="sxs-lookup"><span data-stu-id="8afc5-113">0</span></span>|<span data-ttu-id="8afc5-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="8afc5-114">Allow the user to set.</span></span>|
|<span data-ttu-id="8afc5-115">none</span><span class="sxs-lookup"><span data-stu-id="8afc5-115">none</span></span>|<span data-ttu-id="8afc5-116">1</span><span class="sxs-lookup"><span data-stu-id="8afc5-116">1</span></span>|<span data-ttu-id="8afc5-117">Данные телеметрии отправляется компоненты операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8afc5-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="8afc5-118">Примечание: Это значение применимо только к устройствам, enterprise и сервера.</span><span class="sxs-lookup"><span data-stu-id="8afc5-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="8afc5-119">С помощью этого параметра на других устройствах эквивалентно параметру значение 1.</span><span class="sxs-lookup"><span data-stu-id="8afc5-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="8afc5-120">Базовая</span><span class="sxs-lookup"><span data-stu-id="8afc5-120">basic</span></span>|<span data-ttu-id="8afc5-121">2</span><span class="sxs-lookup"><span data-stu-id="8afc5-121">2</span></span>|<span data-ttu-id="8afc5-122">Отправляет данные телеметрии для базовой.</span><span class="sxs-lookup"><span data-stu-id="8afc5-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="8afc5-123">Enhanced</span><span class="sxs-lookup"><span data-stu-id="8afc5-123">enhanced</span></span>|<span data-ttu-id="8afc5-124">3</span><span class="sxs-lookup"><span data-stu-id="8afc5-124">3</span></span>|<span data-ttu-id="8afc5-125">Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.</span><span class="sxs-lookup"><span data-stu-id="8afc5-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="8afc5-126">Полный</span><span class="sxs-lookup"><span data-stu-id="8afc5-126">full</span></span>|<span data-ttu-id="8afc5-127">4</span><span class="sxs-lookup"><span data-stu-id="8afc5-127">4</span></span>|<span data-ttu-id="8afc5-128">Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.</span><span class="sxs-lookup"><span data-stu-id="8afc5-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




