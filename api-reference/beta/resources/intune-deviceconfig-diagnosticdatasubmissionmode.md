---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e749d2fc7a1eb191c62fbc9db389887cdd901c27
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175222"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="9d1f4-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="9d1f4-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="9d1f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d1f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d1f4-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="9d1f4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9d1f4-107">Members</span></span>
|<span data-ttu-id="9d1f4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9d1f4-108">Member</span></span>|<span data-ttu-id="9d1f4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9d1f4-109">Value</span></span>|<span data-ttu-id="9d1f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d1f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d1f4-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="9d1f4-111">userDefined</span></span>|<span data-ttu-id="9d1f4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9d1f4-112">0</span></span>|<span data-ttu-id="9d1f4-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-113">Allow the user to set.</span></span>|
|<span data-ttu-id="9d1f4-114">Нет</span><span class="sxs-lookup"><span data-stu-id="9d1f4-114">none</span></span>|<span data-ttu-id="9d1f4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9d1f4-115">1</span></span>|<span data-ttu-id="9d1f4-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="9d1f4-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="9d1f4-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="9d1f4-119">Основное</span><span class="sxs-lookup"><span data-stu-id="9d1f4-119">basic</span></span>|<span data-ttu-id="9d1f4-120">2</span><span class="sxs-lookup"><span data-stu-id="9d1f4-120">2</span></span>|<span data-ttu-id="9d1f4-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="9d1f4-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="9d1f4-122">enhanced</span></span>|<span data-ttu-id="9d1f4-123">4</span><span class="sxs-lookup"><span data-stu-id="9d1f4-123">3</span></span>|<span data-ttu-id="9d1f4-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="9d1f4-125">полный</span><span class="sxs-lookup"><span data-stu-id="9d1f4-125">full</span></span>|<span data-ttu-id="9d1f4-126">4</span><span class="sxs-lookup"><span data-stu-id="9d1f4-126">4</span></span>|<span data-ttu-id="9d1f4-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="9d1f4-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




