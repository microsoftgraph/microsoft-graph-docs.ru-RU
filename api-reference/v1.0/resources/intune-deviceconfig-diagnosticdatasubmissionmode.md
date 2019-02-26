---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251036"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="81453-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="81453-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="81453-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81453-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81453-105">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="81453-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="81453-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="81453-106">Members</span></span>
|<span data-ttu-id="81453-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="81453-107">Member</span></span>|<span data-ttu-id="81453-108">Значение</span><span class="sxs-lookup"><span data-stu-id="81453-108">Value</span></span>|<span data-ttu-id="81453-109">Описание</span><span class="sxs-lookup"><span data-stu-id="81453-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81453-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="81453-110">userDefined</span></span>|<span data-ttu-id="81453-111">нуль</span><span class="sxs-lookup"><span data-stu-id="81453-111">0</span></span>|<span data-ttu-id="81453-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="81453-112">Allow the user to set.</span></span>|
|<span data-ttu-id="81453-113">Нет</span><span class="sxs-lookup"><span data-stu-id="81453-113">none</span></span>|<span data-ttu-id="81453-114">1,1</span><span class="sxs-lookup"><span data-stu-id="81453-114">1</span></span>|<span data-ttu-id="81453-115">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="81453-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="81453-116">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="81453-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="81453-117">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="81453-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="81453-118">Основное</span><span class="sxs-lookup"><span data-stu-id="81453-118">basic</span></span>|<span data-ttu-id="81453-119">2</span><span class="sxs-lookup"><span data-stu-id="81453-119">2</span></span>|<span data-ttu-id="81453-120">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="81453-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="81453-121">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="81453-121">enhanced</span></span>|<span data-ttu-id="81453-122">4</span><span class="sxs-lookup"><span data-stu-id="81453-122">3</span></span>|<span data-ttu-id="81453-123">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="81453-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="81453-124">полный</span><span class="sxs-lookup"><span data-stu-id="81453-124">full</span></span>|<span data-ttu-id="81453-125">4</span><span class="sxs-lookup"><span data-stu-id="81453-125">4</span></span>|<span data-ttu-id="81453-126">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="81453-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



