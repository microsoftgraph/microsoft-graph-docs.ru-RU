---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 788da8fd9a239bf26dfd2d9e8d8fbf308d059784
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004542"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="3bf38-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="3bf38-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="3bf38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bf38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3bf38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bf38-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="3bf38-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="3bf38-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3bf38-107">Members</span></span>
|<span data-ttu-id="3bf38-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3bf38-108">Member</span></span>|<span data-ttu-id="3bf38-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3bf38-109">Value</span></span>|<span data-ttu-id="3bf38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3bf38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bf38-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="3bf38-111">userDefined</span></span>|<span data-ttu-id="3bf38-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3bf38-112">0</span></span>|<span data-ttu-id="3bf38-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="3bf38-113">Allow the user to set.</span></span>|
|<span data-ttu-id="3bf38-114">none</span><span class="sxs-lookup"><span data-stu-id="3bf38-114">none</span></span>|<span data-ttu-id="3bf38-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3bf38-115">1</span></span>|<span data-ttu-id="3bf38-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="3bf38-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="3bf38-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="3bf38-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="3bf38-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="3bf38-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="3bf38-119">Основное</span><span class="sxs-lookup"><span data-stu-id="3bf38-119">basic</span></span>|<span data-ttu-id="3bf38-120">2</span><span class="sxs-lookup"><span data-stu-id="3bf38-120">2</span></span>|<span data-ttu-id="3bf38-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="3bf38-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="3bf38-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="3bf38-122">enhanced</span></span>|<span data-ttu-id="3bf38-123">4</span><span class="sxs-lookup"><span data-stu-id="3bf38-123">3</span></span>|<span data-ttu-id="3bf38-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="3bf38-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="3bf38-125">полный</span><span class="sxs-lookup"><span data-stu-id="3bf38-125">full</span></span>|<span data-ttu-id="3bf38-126">SP4</span><span class="sxs-lookup"><span data-stu-id="3bf38-126">4</span></span>|<span data-ttu-id="3bf38-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="3bf38-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





