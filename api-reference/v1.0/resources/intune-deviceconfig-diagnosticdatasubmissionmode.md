---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 15abccb0bf2171e62c2b468ecf5c3078e052ea75
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359378"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="03f57-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="03f57-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="03f57-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03f57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03f57-105">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="03f57-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="03f57-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="03f57-106">Members</span></span>
|<span data-ttu-id="03f57-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="03f57-107">Member</span></span>|<span data-ttu-id="03f57-108">Значение</span><span class="sxs-lookup"><span data-stu-id="03f57-108">Value</span></span>|<span data-ttu-id="03f57-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03f57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f57-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="03f57-110">userDefined</span></span>|<span data-ttu-id="03f57-111">нуль</span><span class="sxs-lookup"><span data-stu-id="03f57-111">0</span></span>|<span data-ttu-id="03f57-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="03f57-112">Allow the user to set.</span></span>|
|<span data-ttu-id="03f57-113">none</span><span class="sxs-lookup"><span data-stu-id="03f57-113">none</span></span>|<span data-ttu-id="03f57-114">1,1</span><span class="sxs-lookup"><span data-stu-id="03f57-114">1</span></span>|<span data-ttu-id="03f57-115">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="03f57-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="03f57-116">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="03f57-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="03f57-117">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="03f57-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="03f57-118">Основное</span><span class="sxs-lookup"><span data-stu-id="03f57-118">basic</span></span>|<span data-ttu-id="03f57-119">2</span><span class="sxs-lookup"><span data-stu-id="03f57-119">2</span></span>|<span data-ttu-id="03f57-120">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="03f57-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="03f57-121">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="03f57-121">enhanced</span></span>|<span data-ttu-id="03f57-122">4</span><span class="sxs-lookup"><span data-stu-id="03f57-122">3</span></span>|<span data-ttu-id="03f57-123">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="03f57-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="03f57-124">полный</span><span class="sxs-lookup"><span data-stu-id="03f57-124">full</span></span>|<span data-ttu-id="03f57-125">SP4</span><span class="sxs-lookup"><span data-stu-id="03f57-125">4</span></span>|<span data-ttu-id="03f57-126">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="03f57-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




