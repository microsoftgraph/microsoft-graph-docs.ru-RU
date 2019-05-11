---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ba90c6cbbd8e242e4cd5902a938d5e670d7d2d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946877"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="0e835-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="0e835-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="0e835-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e835-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e835-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="0e835-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="0e835-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0e835-107">Members</span></span>
|<span data-ttu-id="0e835-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0e835-108">Member</span></span>|<span data-ttu-id="0e835-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0e835-109">Value</span></span>|<span data-ttu-id="0e835-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e835-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e835-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="0e835-111">userDefined</span></span>|<span data-ttu-id="0e835-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0e835-112">0</span></span>|<span data-ttu-id="0e835-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="0e835-113">Allow the user to set.</span></span>|
|<span data-ttu-id="0e835-114">none</span><span class="sxs-lookup"><span data-stu-id="0e835-114">none</span></span>|<span data-ttu-id="0e835-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0e835-115">1</span></span>|<span data-ttu-id="0e835-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="0e835-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="0e835-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="0e835-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="0e835-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="0e835-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="0e835-119">Основное</span><span class="sxs-lookup"><span data-stu-id="0e835-119">basic</span></span>|<span data-ttu-id="0e835-120">2</span><span class="sxs-lookup"><span data-stu-id="0e835-120">2</span></span>|<span data-ttu-id="0e835-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="0e835-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="0e835-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="0e835-122">enhanced</span></span>|<span data-ttu-id="0e835-123">4</span><span class="sxs-lookup"><span data-stu-id="0e835-123">3</span></span>|<span data-ttu-id="0e835-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="0e835-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="0e835-125">полный</span><span class="sxs-lookup"><span data-stu-id="0e835-125">full</span></span>|<span data-ttu-id="0e835-126">SP4</span><span class="sxs-lookup"><span data-stu-id="0e835-126">4</span></span>|<span data-ttu-id="0e835-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="0e835-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




